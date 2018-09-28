******************************
File Server Installation Guide
******************************

A file server is a computer responsible for central storage of data. A file server works in conjunction with our main server, 
and it's the backbone for Remote Deployment. A file server is a must in the following usage scenarios:

- Deployment of Patches.
- Deployment of Packages.
- Self-upgrade of Flotomate Agent application.

Shared drive configuration in our product has been deprecated, and the architecture allows 
delivery of Patch/Packages to Agent/Relay via File Server only.

How File Server Works
=====================

.. _FSC-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/file-server-configuration/FSI-1.png
    :align: center
    :alt: figure 1

Installing Flotomate File Server
================================

Prerequisite
------------

- Separate Linux server for File Server installation.
- You need ubuntu-16.04.1 desktop OS to run. Follow the link
  to download the OS:

  https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/share/ubuntu_server_os.iso

Installation Steps
------------------

In order to initiate a file server you need to configure in three places (Main Server , Relay server (if required), and File Server).

.. note:: We provide a single build for Relay and File Server.

In File Server
^^^^^^^^^^^^^^

- Install :ref:`Relay server <Flotomate Relay Server Installation Guide>` as per instruction.

- Acquire root access: **sudo -i**.

- Change directory: **cd/opt/flotomate/relay-server/config**

.. _FSC-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/file-server-configuration/FSI-2.png
    :align: center
    :alt: figure 2

- change under main-server : **URL={your main server url}**

.. _FSC-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/file-server-configuration/FSI-3.png
    :align: center
    :alt: figure 3

- Now restart services: **systemctl restart ft-relay-server** (Do not forgot this)

In Relay Server (If in use)
^^^^^^^^^^^^^^^^^^^^^^^^^^^
Type the following commands in the terminal of the relay server (a separate server altogether) to change **Service-conf.yaml** file.

- Get root access: **sudo -i**

- Change directory: **cd /opt/flotomate/relay-server/config**

- Open: **nano services-conf.yaml**

- Change under main-server : **URL={your main server url}**

- Restart services: **systemctl restart ft-relay-server** (Do not forgot this).

In Main Server
^^^^^^^^^^^^^^

Do following step to change  Service-conf.yaml file in the Main Server.

- Get root access: **sudo -i**

- Change directory: **cd /opt/flotomate/main-server/config**

- Open: **nano application-hosted.properties**

- Change the following field: **com.flotomate.fileServer.url=http://{file Server Ip}:7070/api** (change port if you have changed port of file server)

.. _FSC-4:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/file-server-configuration/FSI-4.png
    :align: center
    :alt: figure 4
  
- Restart services: **systemctl restart ft-main-server** (Do not forgot this)