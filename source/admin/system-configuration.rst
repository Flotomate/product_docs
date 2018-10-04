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

Initiating an Upgrade Request:
------------------------------

-  Go to the **Admin** (A Navigation Tab) >> **All Computers**
   (Systems).

.. _adf-149:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-149.png
    :align: center
    :alt: figure 149

-  The Agent Self Upgrade page opens. Here you can view all your
   existing requests. To create a new one, click on **Create Upgrade
   Request** situated in the top right corner.

-  A new dialog box opens with the following fields:

    .. _adf-150:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-150.png
        :align: center
        :alt: figure 150

    a. In section A, you give a name to the request. You can search for a
       request by its name in the Agent Self Upgrade page.

    b. You write the Agent version in section B that you are going to
       deploy.

    c. In section C, you select a platform (either Windows or Linux).

    d. Select an architecture in section D.

    e. You attach the exe file of the Agent in section E.

    f. Write a description of the new Agent in section F.

   When you are done, click on **Create**. The main server immediately
   activates the request.

Rejecting an Upgrade Request
----------------------------

You can reject an already published upgrade request in the following
way:

-  Open Agent Self Upgrade page from Admin.

-  Click on the **Reject** button adjacent to the request that you want
   to stop.

.. _adf-151:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-151.png
    :align: center
    :alt: figure 151

-  On confirmation, the server stops sending the command for upgrade to
   all computers in the scope. Computers that have already upgraded stay
   unaffected.

Periodic DB Upgrade
===================

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
