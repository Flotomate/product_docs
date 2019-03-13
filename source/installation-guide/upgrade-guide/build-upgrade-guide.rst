.. _server-upgrade:

*********************************************
Flotomate Service Desk - Server Upgrade Guide
*********************************************

.. important:: The upgrade of the server has to be done incrementally. Meaning, from build 2.5 you cannot jump to 3.0; you have to
               download the in between versions. Know about the list of :ref:`releases so far <Flotomate Build Archive>`. 

1. It is recommended that you take snapshot of your
   existing virtual machine before proceeding with upgrade.

2. Download the latest release build from the below link:

   `Download Link <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/main/linux/service_desk_master_CI>`_

3. Copy release build installer (service_desk_master_CI) to target
   machine.

4. Make Sure you have execute permission to build the file. If it does not
   have execute permission then you can change it by using following command,

   **sudo chmod 777 service_desk_master_CI**

5. Run Installer by following command

   **sudo ./service_desk_master_CI**

   .. _sib-7:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-7.png
       :align: center
       :alt: figure 7

   Once you see below screen, that means you have successfully upgraded the
   product.

.. _sib-8:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-8.png
       :align: center
       :alt: figure 8

6. Now **wait** for at least **5 Minutes** to allow restart of all
   Flotomate services.

7. Now you can login to Flotomate as usual and start
   using product.

.. _sib-9:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/SIB-9.png
       :align: center
       :alt: figure 9  