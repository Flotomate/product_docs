**********************************************************
Flotomate Service Desk – Server Installation via ISO Guide
**********************************************************

Describes ISO Installation Steps

System Requirements
===================

Hardware Requirement:

-  4GB System RAM

-  Two Core Processor

-  Space: 100 GB Hard Drive


Product ISO Link
================

Download product ISO containing Ubuntu 16.04 from following link:

`Download Link <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/main/linux/service_desk.iso>`_

Installation Process:
=====================

1. Boot ISO.in your target machine

2. Select language:

.. _sii-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-1.png
    :align: center
    :alt: figure 1

3. Select installation type, “\ *Install IT Service Desk*\ ”.

.. _sii-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-2.png
    :align: center
    :alt: figure 2

4. The installation process will start.

.. _sii-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-3.png
    :align: center
    :alt: figure 3

5. After installation is completed, log in with the credentials
   mentioned below:

..

   **Username**: Jarvis

   **Password**: marvel

6. Go to product directory using the below command:

..

   **cd /opt**

7. Make Sure you have execute permission to build file. If it does not
   have execute permission then you can change it by following command.

   **sudo chmod 777 service_desk_master_CI**

8. Run Installer by following command

   **sudo ./service_desk_master_CI**

    .. _sii-4:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-4.png
        :align: center
        :alt: figure 4

   During Installation, Installer will prompt for Password. Please
   provide following password : mypassword.

    .. _sii-5:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-5.png
        :align: center
        :alt: figure 5

   During Installation, Installer will prompt for Tenant Name. You can set
   any name (must be all small letters without any special characters or
   spaces.)

    .. _sii-6:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-6.png
        :align: center
        :alt: figure 6

    .. _sii-7:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-7.png
        :align: center
        :alt: figure 7

  Once you see below screen, that means you have successfully installed
  the product.

9. After Installation,

   Navigate to http://localhost/register, It will open Registration form
   as below :

.. _sii-8:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-8.png
    :align: center
    :alt: figure 8

10. Please provide super admin user details there.

11. In Personalize URL field, make sure you put exact same name which
    you given as tenant name during installation process.

12. Now you can login to http://localhost with super admin user, Setup
    your organization, users and configure important setting to start
    using a product.

.. _sii-9:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SII-9.png
    :align: center
    :alt: figure 9

13. Note that:

    a. You can login to Technician Portal by selecting ‘Technician
       Portal’ tab and,

    b. You can login to Customer Portal by selecting ‘Support Center’
       tab.

14. You can login to Customer Portal by selecting ‘Support Center’ tab.


