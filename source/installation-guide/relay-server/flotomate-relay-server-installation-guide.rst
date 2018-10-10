*****************************************
Flotomate Relay Server Installation Guide
*****************************************

Describes Relay Server (2.7.0) Installation Steps via build.

Downloading Base OS
===================

You need ubuntu-16.04.1 desktop OS to run our product. Follow the link
to download the OS:

https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/share/ubuntu_server_os.iso

Product Installer
=================

Download product build/installer from following link :

`Download Link <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/relay+server/linux/relay_server_CI>`_

Installation Steps : 
====================

After installing the Base OS, follow the below steps to install Relay Server:

1. Copy release build installer (relay_server_CI) to target machine.

2. Make Sure you have execute permission to build file. If it does not
   have execute permission then you can change it by following command,

   **sudo chmod 777 relay_server_CI**

3. Run Installer by following command

   **sudo ./relay_server_CI**

    .. _rsib-1:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/relay-server-installation/RSIB-1.png
        :align: center
        :alt: figure 1
   
4. Type in your system pass and hit enter to start the installation process. 

5. Once you see below screen, that means you have successfully installed
   the relay server.

    .. _rsib-2:
    
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/relay-server-installation/RSIB-2.png
         :align: center
         :alt: figure 2