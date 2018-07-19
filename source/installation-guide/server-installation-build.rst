******************************************************
Flotomate Service Desk – Server Installation via Build
******************************************************
Describes Server Installation Steps via product build

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

https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/main/linux/service_desk_master_CI


Installation Steps : 
=====================

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
   provide following password : mypassword

    .. _sib-2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-2.png
        :align: center
        :alt: figure 2

   During Installation, Installer will prompt for Tenant Name. You can
   set any name (must be all small letters without any special
   characters or spaces.)

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

4. After Installation,

   Navigate to http://localhost/register, It will open Registration form
   as below :

.. _sib-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-5.png
    :align: center
    :alt: figure 5

5. Please provide super admin user details there.

6. In Personalize URL field, make sure you put exact same name which you
   given as tenant name during installation process.

7. Now you can login to http://localhost with super admin user, Setup
   your organization, users and configure important setting to start
   using a product.

.. _sib-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-6.png
    :align: center
    :alt: figure 6

8. Note that :

   Technician Portal will be available at :
   http://localhost

   Customer Portal will be available at : http://localhost/portal

9. You can also configure DNS entry which points domain name to
   machine’s IP address as you wish.

