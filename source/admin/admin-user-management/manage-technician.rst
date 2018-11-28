*******************
Managing Technician
*******************

A Technician is a person who delivers IT services by having certain
rights to perform activities spanning across product administration,
request handling, knowledge management, problem handling, change
management, reporting, remote deployment, project management and asset
monitoring. The extent of activities depends on the role/roles of a
Technician.

.. note:: Managing Technician requires you to have admin rights.

.. _add-technician:

Add/View Technicians
====================

1. Log in to your Dashboard and click **Admin** from the Navigation
   tabs.

2. Click on **Technicians** in Users. You are directed to the
   Technicians page. Here you can view all current Technicians in the
   system if any. By default, the superuser is on the list before you
   even start adding anyone.

.. _adf-23:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-23.png
    :align: center
    :alt: figure 23

3. Click **Add Technician** button situated in the top right corner of
   the page. The **Add Technician** dialog box opens.

.. _adf-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-24.png
    :align: center
    :alt: figure 24

4. In the Add Technician dialog box you have to input the following
   information:

   a. Name of the Technician.

   b. Email ID of the Technician.

   c. Password for the Technician to log in to the system.

   d. The department to which the Technician is associated. This is not
      a mandatory field. Departments are added from a drop-down menu.
      Learn how to add a :ref:`department <departments>` to the
      product.

   e. Roles of the Technician. This defines the rights and permissions
      of the Technician. Learn how to :ref:`create custom
      roles <technician Roles>`.

   f. There are four support levels to choose from; you can select all
      four. Defining the levels of a Technician is a way to quantify
      his/her capabilities. Some tickets have a defined tier which tells
      that only a Technician of that tier (level) should handle it. This
      is not a mandatory field.

   g. Add the location of the Technician. Learn :ref:`how to add a
      location <location>` to the product. Adding location here will put the technician in a location scope as a requester. 

      .. important:: (Note that Location Authorization and Location are two different concept.)

   h. The **Authorization Location** puts the technician in the location scope. The field is populated from the location list, but
      unlike the location field above, the Authorization Location only allows the technicians to view objects (tickets, Assets, etc) for
      the selected location and those with no location details. Learn more about :ref:`Location Scope <Data Segregation with Location Scope>`. 

   i. You can further filter what the technician can view using the Access Level control. You can assign three types of access level.

      .. _adf-24.1:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-24.1.png
            :align: center
            :alt: figure 24.1

      i. **Global Access**: Assigns location specific rights as per :ref:`Location Scope <Data Segregation with Location Scope>`.

      ii. **Group Access**: This puts an additional restriction on top of Global Access. A technician with Group Access permission
          will be able to see only Requests tickets with unassigned Technician Group, and if assigned, then he/she has to be
          part of the group in order to see the tickets.

      iii. **Restricted Access**: This puts an additional restriction on top of Global Access. Technicians with this permission 
           won't be able to view and create Request tickets.

      Learn about a :ref:`use case <Creating a HR Technician Using Authorization>` on using Authorization for technicians.

5. Hit **Add** to register a new Technician.


Update a Technician’s Info
==========================

Flotomate provides the **Edit Technician** dialog box for easy
modification of a Technician’s info.

:ref:`Learn who is Technician? <managing Technician>`

.. note:: You need to have administrative rights to view and modify Technician details.

-  .Go to **Admin** (A Navigation tab) >> **Technicians** (Users)

-  Click the Edit Icon (refer :numref:`adf-23`) adjacent to the Technician, or
   click on the name, that you want to edit. The **Edit Technician**
   dialog box opens.

-  In the Edit Technician dialog box, edit the fields that you want to
   change. Update your changes before closing the dialog box.

.. _adf-25:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-25.png
    :align: center
    :alt: figure 25

Convert a Technician into Super-User
------------------------------------

A superuser is a user with privilege levels far beyond those of most user accounts. 
Superuser account is necessary for the platform management functions but also to control and oversee them.

A superuser can convert an existing  Technician into a superuser after giving up his/her rights.

**To Convert a Technician into Superuser**

- He goes to **Admin** (A Navigation Tab) >> **Technician** (under User).

- In the Technician page, an **Action Menu** Icon is visible against people who are not
  superusers. This **Action Menu** Icon is visible to the superuser only.

.. _adf-25.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-25.1.png
    :align: center
    :alt: figure 25.1

- Superuser clicks on the option **Convert to Super Admin** in the Action Menu of a Technician. 
  This opens a dialog box with the following fields:

  a. **My Email**: The email ID of the existing superuser.

  b. **Roles**: The roles of the existing superuser when he/she is no longer the superuser.

  c. **Location**: The location of the existing superuser when he/she is no longer the superuser.

  .. _adf-25.2:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-25.2.png
    :align: center
    :alt: figure 25.2

- He clicks on **Proceed** that takes him to another dialog box where he has to confirm the migration by entering
  his account password. 

.. _adf-25.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-25.3.png
    :align: center
    :alt: figure 25.3

- On success, the existing superuser is logged out, and he is no longer the superuser.        

Role of a Technician
--------------------

A Technician can have multiple roles. Each role has its rights. Click
the Roles field in Edit Technician dialog box (:numref:`adf-25`)\ **;** select
the roles applicable to the person and hit **Update** to make the
changes.

Learn :ref:`how to add new roles <technician roles>`.

Change Support Level
--------------------

There are four support levels to choose from; you can select all four.
Defining the levels of a Technician is a way to quantify his/her
capabilities. Some tickets have a defined tier which tells that only a
Technician of that tier (level) should handle it.

A Technician can have support levels. Click the Support Level field in
Edit Technician dialog box (:numref:`adf-25`)\ **;** select the tiers
applicable to the person and hit **Update**.

Reset Password of a Technician
------------------------------

Resetting the password of a Technician is very easy. Click the **Reset Password button** (refer :numref:`adf-25`). 
Click **yes** to confirm; a password reset link is sent to the Technician’s email address.