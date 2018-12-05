******
System 
******

Agent Self Upgrade
==================

Developing our Agent application is an ongoing process, which is why we
release a new version periodically. In every version, the application is
better compared to the previous either in terms of performance,
capabilities or both.

The Agent Self Upgrade feature allows for a smooth transition from one
version of the Agent to another. Using this feature, an admin can
centrally deploy an Agent.msi/exe from the main server, which is received
by all the (active) computers having :ref:`Remote Monitoring <Flotomate Agent Monitor Installation Guide>`.

Some of the benefits of using the latest version of the Agent
application:

-  Newer versions of the Agent are more stable and give better
   performance.

-  Upgrading gives you more capabilities/features.

-  Upgrading to a newer version eliminates possible security flaws.

Uploading a New Agent Application File (Step 1)
-----------------------------------------------

-  Go to the **Admin** (A Navigation Tab) >> **All Computers**
   (Systems).

.. _adf-149:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-149.png
    :align: center
    :alt: figure 149

-  The All Computers page opens. Here you can view all your
   existing Computers (with the Agent application) along with their active status. 
   Step one is to upload the new Agent application file; click on **Upload New Agent** from the Action Menu.

   .. _adf-149.1:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-149.1.png
        :align: center
        :alt: figure 149.1

-  A new dialog box opens where you have to enter the following inputs:

    .. _adf-150:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-150.png
        :align: center
        :alt: figure 150

    a. Name of the upgrade.

    b. Version of the Agent installation file.

    c. Supported OS platform of the Application file (either Windows or Ubuntu).

    d. Supported architecture either 32bit or 64bit.

    e. Lastly, attache the installation file of the latest Agent.

   When you are done, click on **Create**. This updates the uploaded agent list.

   .. _adf-150.1:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-150.1.png
        :align: center
        :alt: figure 150.1

Initiating an Upgrade (Step 2)
------------------------------

-  Go to the **Admin** (A Navigation Tab) >> **All Computers**
   (Systems).

-  :ref:`Search <Searching Assets>` and select the computers that you want to upgrade, and click the **Upgrade** button.

.. _adf-151:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-151.png
    :align: center
    :alt: figure 151

-  On confirmation, the server will deploy the latest version of the Agent from the uploaded agent list.

Periodic DB Backup
==================

Users can create backups of the database of the Main (Product) Server. The database contains all the user generated data from all the 
modules. Once a backup is created, a (Admin) user can download the backup to his local machine. 

A backup can be initiated manually and scheduled for automatic creation. 

**Some benefits of doing Periodic Backups:**

- Backups give protection against data lose incase of product failure or corruption.

- Backups provide flexibility in data migration. 

- Ability to hold data for a longer period of time. 

- Ability to give legal response related to compliance.

Manually Initiate & Download a backup
=====================================

- Go to **Admin** >> **Database Backup** (under System).

.. _adf-151.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-151.1.png
    :align: center
    :alt: figure 151.1

- The Database Backup page opens. Here you can view all your current backups. Click on **Backup Now** to create a new backup.

- Once backup is created, click on **Download Backup** which will locally install the backup.

.. _adf-151.2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-151.2.png
    :align: center
    :alt: figure 151.2

Scheduling a Backup
===================

A schedule will automatically create a backup at a specified interval. 

- Go to **Admin** >> **Database Backup** (under System).

- Click on **Schedule Backup** to specify a interval. 

- A dialog box opens where you set a schedule Frequency and configure email notification.

  .. _adf-151.3:
  
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-151.3.png
      :align: center
      :alt: figure 151.3

  a. **Schedule Frequency**: Currently there are five types of frequencies:
     
     .. note:: Proper time tracking depends on appropriate Time Zone selection. 

     i. **Once**: Backup will happen at a specific date and time.

     ii. **Daily**: Backup will happen everyday after a certain date & time at a specific time.

     iii. **Weekly**: Discovery happens on a specific day/days of a week at a specific time.

     iv. **Monthly**: Discovery happens in selected month/months of a year on a particular day at a specific time.

     v. **Interval**: Discovery happens every specified Minutes, Hours, Days or Months.

  b. You can add recipients (email addresses) who will receive an email when a backup attempt fails.

- Once a backup happens, you can download it locally.   
