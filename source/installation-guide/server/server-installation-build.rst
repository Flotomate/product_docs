******************************************************
Flotomate Service Desk – Server Installation via Build
******************************************************
Describes Server (2.7.0) Installation Steps via product build

System Requirements
===================

Hardware Requirement:

-  4GB System RAM

-  Dual Core Processor

-  Space: 100 GB Hard Drive

Downloading Base OS
===================

You need ubuntu-16.04.1 desktop OS to run our product. Follow the link
to download the OS:

https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/share/ubuntu_server_os.iso

.. note:: Ignore the above steps if you’re coming from the Product ISO
          installation setup.


Product Installer
=================

Download product build/installer from following link :

`Download Link <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/main/linux/service_desk_master_CI>`_

Fresh Installation Guide : 
==========================

After installing the Base OS, follow the below steps to install the
product on to your server:

1. Copy release build installer (flotomate_master_CI) to target machine.

2. Make Sure you have execute permission to build file. If it does not
   have execute permission then you can change it by following command,

   **sudo chmod 777 service_desk_master_CI**

3. Run Installer by following command

   **sudo ./service_desk_master_CI**

    .. _sib-1:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-1.png
        :align: center
        :alt: figure 1

   During Installation, Installer will prompt for Password. Please
   provide following password : whatpassword

    .. _sib-2:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-2.png
        :align: center
        :alt: figure 2

   Next, you have to select whether you want a standalone installation or a High Availability setup. Option 1 is for a standalone
   installation, and 2 & 3 are for a High Availability setup. In case, you are opting for HA then you have to install the build in two
   separate servers one as Master and other as Slave. Learn more about :ref:`HA setup <Flotomate High Availability Server Setup>`.

    .. _sib-3:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-3.png
        :align: center
        :alt: figure 3

   Once you see below screen, that means you have successfully installed
   the product.

.. _sib-4:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-4.png
    :align: center
    :alt: figure 4

4. After Installation, wait of five minutes.

   Navigate to http://{server_IP}/register, It will open Registration form
   as below :

.. _sib-5:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-5.png
    :align: center
    :alt: figure 5

5. The registration form is for the first user, who is by default the Super User. The Super User has all the rights. 
   Register a user, and use the credentials to login to the ITSM portal. 

6. You can access the ITSM portal from a web-browser on **http://{server_IP}/login**. Use the tab to switch between Customer and
   Technician portal (:numref:`sib-6`). 

.. _sib-6:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-6.png
    :align: center
    :alt: figure 6