***************
User Management
***************

Manage Requestors
=================

The Requestors are people who are seeking information, change or
solution to a problem through our platform. They are the users of the
product, and almost all of the product features are geared towards
delivering IT services to Requestors. So it is important to manage their
information in the product.

Flotomate allows you to add Requestors individually and bulk upload
through LDAP server synchronization. Once uploaded, you can manage them
from the Admin section.

.. note:: All Technician are Requestors by default and enjoy their rights and permissions, and even more.

.. _view-requestor:

**Open Requestors Page**

The Requestors page is where you can add, view, update and delete
Requestors in the product.

.. note:: You need to have admin rights or be a Super User to add and modify Requestors.

1. Log in to Flotomate, and go to **Admin** from the Navigation Tabs

.. _adf-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-3.png
    :align: center
    :alt: figure 3

2. Search Requestors in the search bar or you can directly go to
   **Requestors** under Users. Clicking on **Requestors** opens the
   Requestors page.

3. Here you see all the Requestors in the product if any.

.. _adf-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-4.png
    :align: center
    :alt: figure 4

You see only the Super User in the Requestor list when you log in for
the first time; new names get populated in the list as you add more
Requestors.

Add Requestors Individually
---------------------------

You can add Requestors individually by entering their details.

:ref:`Who are Requestors? <manage requestors>`

-  Go to **Admin** >> **Requestors** (Users).

-  On the **Requestors** page, click **Add** **Requestor** situated in
   the top right corner of the page. You get the **Add** **Requestor**
   dialog box.

-  Fill in the details of the new Requestor along with a password. You
   can mark a Requestor as VIP if he/she is a critical person in the
   organization. This gives him/her the following benefits:

   a. Tickets created by him/her have the VIP label. They are treated
      with priority by the Technicians.

   b. Specific Workflows, SLAs, and Reports can be created for VIPs.

-  You can create custom fields that allow you to store additional information. :doc:`Learn More (see Custom Fields) <admin-customization>`    

-  When you are done filling in the details, hit **Add**.

.. _adf-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-5.png
    :align: center
    :alt: figure 5

You can edit the details of Requestors created manually or imported
through CSV. You cannot edit Requestors imported via LDAP.

-  In the Requestors page, :ref:`Search <search for a requestor>` for the
   Requestor that you want to edit.

-  Click on the Edit Icon adjacent to the Requestor. The Edit Requestor
   dialog box opens.

    .. _adf-6:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-6.png
        :align: center
        :alt: figure 6

-  Perform your edits and hit **Update**.

You can delete Requestors created manually, imported through CSV or
imported via LDAP.

-  :ref:`Search <search for a requestor>` for the Requestor that you want to
   delete.

-  Click on the Delete Icon adjacent to the Requestor. On Confirmation,
   the Requestor is deleted.

.. _adf-7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-7.png
    :align: center
    :alt: figure 7

Import Requestors Using CSV
---------------------------

In an organization there could be hundreds or thousands of Requestors;
in that case, adding them individually is not feasible. The tool allows
you to import Requestors from a CSV (Comma Separated Values) file into
the system; this makes the uploading process much faster.

To upload Requestors from a CSV follow the below steps:

-  Create a CSV file with the following property names in the first row
   (heading).

   a. Department

   d. Location

   c. Name

   d. Contact No.

   e. Email

   f. Password

   If you do not use the property names mentioned above, then you
   have to manually match your names with the system property names
   mentioned above.

   Name, Email, and Password are required columns.

-  In the CSV file, input the Requestor details under their respective
   heads. Each row should represent a single Requestor.

-  Go to the :ref:`Requestors <manage requestors>` page. Click on settings
   and select **Import from CSV**.

.. _adf-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-8.png
    :align: center
    :alt: figure 8

-  Import page opens. Upload the CSV file and click **Next**.

.. _adf-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-9.png
    :align: center
    :alt: figure 9

-  Now you are in the **Column Mapping** stage. Every item in the first
   row (heading) is a name of a property. The system automatically
   matches the names in the file heading with the property names in the
   system.

   In :numref:`adf-9`, the left side column has the system property names and
   right side column has the property names in the CSV file.

   In case a property name does not have a match, the right-hand side
   field of the name remains empty. Here you have to manually select the
   matching name from a drop-down list by clicking on the field.

    .. _adf-10:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-10.png
        :align: center
        :alt: figure 10

   It is not necessary that all the property names have to have a match;
   you can still upload your Requestors as long as required fields are
   taken care off. Click **Next** to continue to the next stage.

   You can create custom property names using Custom Fields. You can create n number of such fields, and they appear
   along side the default ones. :doc:`Learn more (head to Custom Fields) <admin-customization>`. 

-  Now you are in the **Unmatched Value Mapping** stage. The given
   property names in the header have values (rows). The system checks
   for property values that aren’t in the system.

    .. _adf-11:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-11.png
        :align: center
        :alt: figure 11

   You can manually assign a value from the Possible Values (system values)
   to an Unmatched Value (value in the file). Click **Next** to continue to
   the next step.

-  Now you are in the **Review** stage. Here you see the number of
   Requestors being uploaded. Click **Import** to finish the import
   process.

.. _adf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-12.png
    :align: center
    :alt: figure 12

Import Requestors Using LDAP
----------------------------

Some organizations maintain their employee information in a distributed
directory information service. Microsoft Active Directory. If your
organization uses one, then you can import Requestors directly into the
product using the LDAP protocol.

.. note:: You need admin rights to add Requestors using LDAP.

Once :ref:`LDAP server is configured <ldap configuration>`, you can start
importing Requestors:

1. Go to **Admin** >> **LDAP Configuration** (IT Infrastructure).

2. Select the LDAP server from where you want to import. You see an
   option called **Import** **Users**, click it.

.. _adf-13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-13.png
    :align: center
    :alt: figure 13

3. On clicking **Import Users**, you get a confirmation dialog box
   stating whether the import was successful or not.

Search for a Requestor
----------------------

The :ref:`Requestors <manage requestors>` page has a search box for
searching Requestors. The search box uses Advanced Search features.

-  Go to :ref:`Requestors <manage requestors>`.

-  In the search box, you can search for a Requestor using five search
   options. Click on the search box to access the search options.

.. _adf-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-14.png
    :align: center
    :alt: figure 14

-  You can create a filter using multiple search options. For example,
   we have the following search query for finding all the VIP Requestors
   in the marketing department.

    .. _adf-15:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-15.png
        :align: center
        :alt: figure 15

   Some search options have predefined values to choose from.

Convert a Requestor to Technician
---------------------------------

You can convert an existing Requestor into a Technician; this is the
fastest way to add Technicians into the product. It works on Requestors
created manually, imported through CSV or imported via LDAP. In case of
Requestors from LDAP, you cannot edit their details after converting
them to Technicians.

-  Go to **Admin** >> :ref:`Requestor <manage requestors>` (Users).

-  :ref:`Search <search for a requestor>` for the Requestor that you want to
   convert.

-  Click on the Action Menu adjacent to the Requestor. Select **Convert
   to Technician** from the pop-up menu. Add Technician dialog box
   opens.

.. _adf-16:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-16.png
    :align: center
    :alt: figure 16

.. _adf-17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-17.png
    :align: center
    :alt: figure 17

-  In the Add Technician dialog box, the Technician details are
   pre-populated in their respective fields (Name, Email, and
   Department); apart from these fields, you have to enter the following
   information:

   a. Role/Roles as a Technician. This determines the rights and
      permissions of the Technician. Learn more about :ref:`Roles of a
      Technician <technician roles>`.

   b. You can explicitly mention the support level. Technicians are
      grouped into four levels (tiers) based on their degree of
      expertise.

   c. :ref:`Location <location>` of the Technician.

-  When you are done, hit **Add**.

Block a Requestor
-----------------

Sometimes it may happen that you want to prevent certain Requestors from
accessing the product. You can block a Requestor and also who is a
Technician.

You can block Requestors created manually, imported through CSV or
imported via LDAP. Blocked Requestors cannot log in to the system.

-  Go to **Admin** >> :ref:`Requestor <manage requestors>` (Users)

-  :ref:`Search <search for a requestor>` for the Requestor that you want to
   block.

-  Click on the Block Icon adjacent to the Requestor. On Confirmation,
   the Requestor is blocked.

.. _adf-18:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-18.png
    :align: center
    :alt: figure 18

**Unblock Requestor**

-  In the Requestor page, you know a Requestor is blocked when you see
   that the Block Icon is red.

-  Click on the red Block Icon. On confirmation, the Requestor is
   unblocked.

Delete Requestors in Bulk
-------------------------

You can delete multiple Requestors at once from the :ref:`Requestors
page <view-requestor>`. Select one or more Requestors. The
**Archive** button appears above the display pane.

.. _adf-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-19.png
    :align: center
    :alt: figure 19

Clicking on Archive deletes the selected Requestors after confirmation.

Requestor Groups
================

Flotomate allows you to create groups of Requestors. Grouping is a way
to classify Requestors based on certain criteria.

One use of creating groups is in communication:

-  You can send an email notification to a Requestor Group about a
   ticket. All members of the group receives the email.

-  You can email an Announcement to a Requestor Group.

-  You can keep a Requestor Group as a watcher for a ticket (Request or
   Problem). Watchers receive ticket related emails.

-  You can send a Knowledge Article/FAQ to a Requestor Group.

.. note:: You need admin rights to create and modify Requestor Groups.

Add a Requestor Group
---------------------

1. Go to **Admin** >> **Requestor Groups** (Users).

2. The Requestor Groups page opens. Here you get to see all the groups
   in the product if any. Click on **Create a Requestor Group** situated
   in the top right corner of the page.

.. _adf-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-20.png
    :align: center
    :alt: figure 20

3. In the new page, give a name and a description of the group. You can
   manually add group members from the Select Users field. In case there
   are many members, we have the option of setting conditions using the
   **Select a Parameter** field based on that Requestors are added
   automatically. You can set conditions based on three criteria:

    +----------------------+----------------------------------+
    | Requestor Department | Department info from LDAP server |
    +----------------------+----------------------------------+
    | Department ID        | System departments               |
    +----------------------+----------------------------------+
    | Location             | System locations                 |
    +----------------------+----------------------------------+

.. _adf-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-21.png
    :align: center
    :alt: figure 21

4. You can set a single condition or have multiple conditions in
   different condition groups. A condition group can have maximum two
   conditions.

   You have to define the relationship between conditions in a group
   using either AND or OR. In case there are multiple groups, then you
   have to define the relationship between them as well.

   Use **Add Condition Group** button to add groups. The plus icon adds
   conditions to a group, and the delete icon deletes them.

   Use the **Preview** button to preview Requestors who are going to be
   added to a different page.

5. Click on **Create** to add the group.

Go to Requestor Groups page. Click the Edit Icon adjacent to the group
that you want to edit. Make the changes and hit **Update**. You can
delete the group by clicking **Delete**.

You can also delete a group using the Delete Icon from the Requestors
Groups page.

.. _adf-22:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-22.png
    :align: center
    :alt: figure 22

Managing Technician
===================

A Technician is a person who delivers IT services by having certain
rights to perform activities spanning across product administration,
request handling, knowledge management, problem handling, change
management, reporting, remote deployment, project management and asset
monitoring. The extent of activities depends on the role/roles of a
Technician.

.. note:: Managing Technician requires you to have admin rights.

Add/View Technicians
--------------------

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
      location <location>` to the product.

5. Hit **Add** to register a new Technician.


Update a Technician’s Info
--------------------------

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^

A Technician can have multiple roles. Each role has its rights. Click
the Roles field in Edit Technician dialog box (:numref:`adf-25`)\ **;** select
the roles applicable to the person and hit **Update** to make the
changes.

Learn :ref:`how to add new roles <technician roles>`.

Change Support Level
^^^^^^^^^^^^^^^^^^^^

There are four support levels to choose from; you can select all four.
Defining the levels of a Technician is a way to quantify his/her
capabilities. Some tickets have a defined tier which tells that only a
Technician of that tier (level) should handle it.

A Technician can have support levels. Click the Support Level field in
Edit Technician dialog box (:numref:`adf-25`)\ **;** select the tiers
applicable to the person and hit **Update**.

Reset Password of a Technician
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Resetting the password of a Technician is very easy. Click the **Reset Password button** (refer :numref:`adf-25`). 
Click **yes** to confirm; a password reset link is sent to the Technician’s email address.

Technical Groups
================

You can group Technicians into separate **Technician Groups.** It is a
way to classify Technicians; for example, people who work with databases
can be grouped into a Technician Group called Database. There’s no limit
to the number of **Technician Groups** you can create.

Few use cases of having Technician Groups are:

-  You can associate a ticket (Request, Problem or Change) with a
   particular Technician Group; this tells the product/users that the
   ticket should be handled by a Technician of that group.

-  You can send notifications to a Technician Group regarding a ticket.

-  You can send an Announcement through email to a Technician Group.

-  Change in Technician Group of a Request can trigger an automatic
   process.

.. note:: You need to have administrative rights to view and modify Technician Group details.

Create a New Technical Group
----------------------------

-  Log in to your Dashboard and click **Admin** from the Navigation
   Tabs.

-  Click on Technician Groups in Users. The Technician Groups page
   opens.

.. _adf-26:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-26.png
    :align: center
    :alt: figure 26

-  Click on **Create a Technician Group** button situated in the top
   right corner of :numref:`adf-26`.

-  In the new dialog box, give the group a name, description and add the
   technicians in the Users field.

-  Click on **Create** to create the group.

Modify Technician Group
-----------------------

Flotomate provides an easy way to modify existing **Technician Groups**.

To modify an existing group:

-  Go to **Admin** >> **Technician Groups** in Users.

-  Click the Edit icon adjacent to the group that you want to edit
   (refer :numref:`adf-26`)

-  In the Edit Technician Group dialog box, edit the information that
   you want to change and save your changes before closing the dialog
   box.

You can delete any group by hitting the Delete icon adjacent to the
group that you want to delete.

Technician Roles 
================

Every Technician is different, so we have roles to give them different
rights and permissions. Each role is unique, and out of the box we have
seven roles in the system; you cannot modify the permissions and rights
of these roles. However, you can add custom roles where you can set the
permissions and rights; there’s no limit to the number of custom roles
that you can create.

Using Roles you can control the CRUD operations a Technician can perform
across the following modules:

-  Request

-  Problem

-  Change

-  Project

-  Patch

-  Knowledge

-  Asset

-  Admin

- Contract

- Purchase

- Report

Default Roles
-------------

Flotomate offers eight default roles with predefined permissions
covering major ITSM processes.

+-------------------------------+-------------------------------+------------------------------+
| Contract Manager              | Purchase Manager              | Patch Specialist Technician  |
+-------------------------------+-------------------------------+------------------------------+
| Junior Technician             | Asset Specialist Technician   | Change Specialist Technician |
+-------------------------------+-------------------------------+------------------------------+
| Problem Specialist Technician | Request Specialist Technician | Service Desk Technician      |
+-------------------------------+-------------------------------+------------------------------+
| Admin                         |                               |                              |
+-------------------------------+-------------------------------+------------------------------+

Add/View Roles
--------------

-  In the **Admin** section, you can view all the roles in Roles
   (under Users) page. Click any one role to view its permissions and rights.

.. _adf-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-27.png
    :align: center
    :alt: figure 27

-  You add a custom role by going back to the **Roles** page and
   clicking **Create a Role** situated in the top right corner of the page.
   We have the permissions and rights grouped module wise. Click any one
   module to see its rights and permissions.

-  Add a name to the role and a description. You can set the permissions
   and rights for every module.

   We have the following rights and permissions:

    +-----------+--------------------------------------------------+
    | Project   | -  Only view details of Projects                 |
    |           |                                                  |
    |           | -  Create & Update Projects                      |
    |           |                                                  |
    |           | -  Delete Projects                               |
    |           |                                                  |
    |           | -  Manage Project milestones                     |
    |           |                                                  |
    |           | -  Closing a Project                             |
    |           |                                                  |
    |           | -  Manage Project Attachments                    |
    |           |                                                  |
    |           | -  Create Tasks in Project.                      |
    |           |                                                  |
    |           | -  Cancel a Project                              |
    +-----------+--------------------------------------------------+
    | Knowledge | -  Create, update and delete Knowledge.          |
    +-----------+--------------------------------------------------+
    | Request   | -  View, create, update and delete a Request.    |
    |           |                                                  |
    |           | -  Communicate with Requestors.                  |
    |           |                                                  |
    |           | -  Mark a Request as spam.                       |
    |           |                                                  |
    |           | -  Assign a Technician to a Request.             |
    |           |                                                  |
    |           | -  Update status of a Request.                   |
    |           |                                                  |
    |           | -  Close a Request                               |
    |           |                                                  |
    |           | -  Manage relationship in a Request.             |
    |           |                                                  |
    |           | -  Add solution and tasks in a Request.          |
    |           |                                                  |
    |           | -  Merge multiple Requests.                      |
    |           |                                                  |
    |           | -  Resolve a Request.                            |
    |           |                                                  |
    |           | -  Re-open a closed Request.                     |
    |           |                                                  |
    |           | -  Update priority of a Request.                 |
    +-----------+--------------------------------------------------+
    | Problem   | -  View, create, update and delete a Problem.    |
    |           |                                                  |
    |           | -  Add solution to a Problem.                    |
    |           |                                                  |
    |           | -  Assign Technician to a Problem.               |
    |           |                                                  |
    |           | -  Resolving a Problem.                          |
    |           |                                                  |
    |           | -  Re-opening a closed Problem.                  |
    |           |                                                  |
    |           | -  Create tasks in a Problem.                    |
    |           |                                                  |
    |           | -  Update status and priority in a Problem.      |
    |           |                                                  |
    |           | -  Managing relationships in a Problem.          |
    +-----------+--------------------------------------------------+
    | Change    | -  View, create, update and delete a Change.     |
    |           |                                                  |
    |           | -  Creating tasks in a Change.                   |
    |           |                                                  |
    |           | -  Assign a Technician to a Change.              |
    |           |                                                  |
    |           | -  Updating status and priority of a Change.     |
    |           |                                                  |
    |           | -  Managing relationships in a Change.           |
    |           |                                                  |
    |           | -  Closing and Re-opening a Change               |
    +-----------+--------------------------------------------------+
    | Patch     | -  Manage Patches & Packages                     |
    |           |                                                  |
    |           | -  View Patches & Package.                       |
    |           |                                                  |
    |           | -  View Remote Deployment.                       |
    |           |                                                  |
    |           | -  View/Manage Computer Group                    |       
    |           |                                                  |
    |           | -  Manage Remote Deployment Policy.              |
    |           |                                                  |
    |           | -  View Auto Patch Deployment Task.              |
    |           |                                                  |
    |           | -  Manage Auto Patch Deployment Task.            |
    |           |                                                  |
    |           | -  View Auto Patch Test Task.                    |
    |           |                                                  |
    |           | -  Manage Auto Patch Test Task.                  |
    |           |                                                  |
    |           | -  View Decline Patch Configuration.             |
    |           |                                                  |
    |           | -  Manage Decline Patch Configuration.           |
    |           |                                                  |
    |           | -  Manage Remote Deployment.                     |
    |           |                                                  |
    |           | -  Permission to ignore Patches.                 |
    |           |                                                  |
    |           | -  Permission to configure Packages for Patches. |
    +-----------+--------------------------------------------------+
    | Asset     | -  Managing Asset discovery and Administration.  |
    |           |                                                  |
    |           | -  View, create, update and delete an Asset.     |
    |           |                                                  |
    |           | -  Update status of Assets.                      |
    |           |                                                  |
    |           | -  Manage relationships of Assets.               |
    +-----------+--------------------------------------------------+
    | Admin     | -  Manage organization.                          |
    |           |                                                  |
    |           | -  Manage automation in the product.             |
    |           |                                                  |
    |           | -  Ignore approvers in an Approval process.      |
    +-----------+--------------------------------------------------+ 
    | Contract  | - View Contracts                                 |
    |           |                                                  |
    |           | - Update and Create Contracts                    |
    |           |                                                  |
    |           | - Delete Contracts                               |
    |           |                                                  |
    |           | - Manage attachments of Contracts                |
    |           |                                                  |
    |           | - Contract Renewal                               |
    |           |                                                  |
    |           | - Manage relationships of Contracts              |
    +-----------+--------------------------------------------------+
    | Purchase  | - View Purchase Order                            |
    |           |                                                  |
    |           | - Create and update Purchase Order               |
    |           |                                                  |
    |           | - Delete Purchase Orders                         |
    |           |                                                  |
    |           | - Manage invoice and payments                    |
    |           |                                                  |
    |           | - Manage relationships of PO                     |
    |           |                                                  |
    |           | - Closing POs                                    |
    |           |                                                  |
    |           | - Cancel Purchase Order                          |
    +-----------+--------------------------------------------------+
    | Report    | - View and manage Reports                        |
    +-----------+--------------------------------------------------+

-  Once you are done with the permissions and rights, hit **Create** to
   create your new role.

**Modify Roles**

You can go to the **Roles** page anytime and change the permissions and
rights of the roles that you have created using the Edit Icon. Default
roles cannot be modified.

Helpdesk Security
=================

This section of Admin controls how users log in to the product and the
necessity of their credential when submitting a ticket.

You can make sure that users can securely log into the customer portal
with third party credentials using a SSO login . You can even make
login an optional action before submitting a Request from the customer
portal.

Single Sign-On Configuration
----------------------------

Single Sign-On feature in Flotomate enables users to log in to the
customer portal with third-party credentials. It creates a unifying
experience for some users and saves time by not having to maintain
multiple accounts.

.. note:: SSO Configuration requires administrative rights.

Activate Create Request through SSO Login
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Go to **Admin** (A Navigation tab) >> **Helpdesk Security** (Users).

.. _adf-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-28.png
    :align: center
    :alt: figure 28

- In the new page, turn on the **Allow Single Sign-On for User**. Now
  you have to configure the SSO settings to use this feature.

Configure Simple SSO:
^^^^^^^^^^^^^^^^^^^^^

-  Go to **Admin** >> **Helpdesk Security** (Users).

.. _adf-29:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-29.png
    :align: center
    :alt: figure 29

-  In the Simple SSO section, click on edit which makes the fields
   editable. Input the following information.

   a. **SSO Login URL**: This is the URL of the third party web server
      where the authentication happens.

   b. **SSO Logout URL**: Sending the Guest Requestor to this URL clears
      all session cookies, and the Guest is logged out.

   c. **SSO Shared Key**: The key authenticates the identity of
      Flotomate during communication with third-party servers. You have
      to copy and put the key in the third party server.

-  Save your changes by hitting **Update**.

Configure Google SSO
^^^^^^^^^^^^^^^^^^^^

People can log in to the customer portal using Google credentials.

-  Go to **Admin** >> **Helpdesk Security** (Users).

.. _adf-30:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-30.png
    :align: center
    :alt: figure 30

-  Once you connect your AuthO client with Google, you are required to
   generate a Client ID. You need to put that Client ID in the Google
   Client ID field.

-  Save your changes by clicking **Update**.

On enabling SSO, an SSO Login button appears on your customer login
page. You can enable/disable an SSO configuration anytime.

.. _adf-31:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-31.png
    :align: center
    :alt: figure 31

Understanding Flow of an SSO Login
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

-  A Requester who intends to log in to your customer portal and clicks
   on "**SSO Login**."

-  The requester is redirected to the Login URL (A SSO login page
   opens).

-  Requester enters his/her application credential in the SSO login
   page.

-  The SSO Login page authenticates credential from the application
   server.

-  If the application server finds given credentials valid, it sends a
   generated "Hash" with a pre-shared key.

-  Now, the Login page makes an authentication call against Flotomate
   server to obtain SSO Token.

-  If authentication is successful, then the Flotomate server issues SSO
   token, and it redirects to Support portal as a logged in user.

Allow Request without Login
---------------------------

Do you want your requesters to be logged in when they make a request, or
you want them to create a request as a guest? Flotomate has the guest
login feature for the latter.

Guests, without a Requestor account, cannot view and manage their
submitted Requests. Guest, with a Requestor account, can view their
Requests in the **My Request** section.

.. note:: Changing this option requires administrative rights.

To enable/disable this option:

- Go to **Admin** >> **Helpdesk Security** (Users).

.. _adf-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-32.png
    :align: center
    :alt: figure 32

- Toggle **Allow to Report Request without login** to turn on/off the
  feature.

Allow Technicians to Submit Requests of Non-Requestors
-----------------------------------------------------

Flotomate has the option to allow Technicians to submit requests in the
name of people who are not requestors. The product doesn't demand for authentication.

.. note:: Changing this option requires administrative rights.

To enable/disable this option:

- Go to **Admin** >> **Helpdesk Security** (Users).

.. _adf-32.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-32.1.png
    :align: center
    :alt: figure 32.1

- Toggle **Allow Technician to report a ticket for non-exist requestor** to turn on/off the
  feature.

User Story
==========    

Ravi is the IT manager at Acme Inc. He is implementing Flotomate
Helpdesk in his company. Ravi has logged into the Dashboard as a
superuser. For now, he wants to add 10 technicians to Flotomate.

-  He goes to the admin section by clicking **Admin** from the
   Navigation tabs.

-  He searches for **Technicians** in the search bar; he sees the
   **Technicians** option in Users and clicks it.

-  He begins by adding Suraj; he fills the fields for Suraj.

.. _adf-33:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-33.png
    :align: center
    :alt: figure 33

-  He adds rest of the team by following the same process.

Ravi realizes that he has accidentally added Mohan as a Technician.
Again he goes to **Technicians** in Users. He finds Mohan and hits the
Delete icon adjacent to his name; he has successfully deleted Mohan from
the system.

He has another task to do. He needs to change the Roles of a Technician
name Naren. He quickly goes to the **Edit Technician** dialog box and
updates his role.

.. _adf-34:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-34.png
    :align: center
    :alt: figure 34

Ravi knows that all his technicians are not the same. He wants to group
them into different groups. Ravi remembers that Flotomate offers
**Technician Groups**; he goes to **Technicians Groups** (Users) from
**Admin**. He quickly adds a database group name Database and adds Naren
and Amartya.

.. _adf-35:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-35.png
    :align: center
    :alt: figure 35

He can efficiently manage all the groups from the **Technician Groups**
page. Now he is confident that he has aligned his company’s resources to
meet its IT requirements.

.. _ad-requestor-accounts:

Requestor Accounts
=================

We have users who use our Helpdesk to serve their external clients from different organization. In such cases, it becomes important to track the source
of a request. With the Request Accounts feature, users of our product can bifurcate incoming Requests based on the organization
of the Requestor. Before using this feature, a user (with admin rights) has to manually add the client organizations in the product.

**Adding a Requestor Account**

- Go to Admin (A Navigation Tab) >> Request Accounts (under User).

.. _adf-35.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-35.1.png
    :align: center
    :alt: figure 35.1

- The Requestor Accounts page opens. Here you can view all your existing accounts. You can search for an account
  using the search bar. To create a new account, click on **Create Requestor Account** situated in the top right corner of the
  page.

- A dialog box opens. Type in a Name and Description and hit **Create**.

.. _adf-35.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-35.2.png
    :align: center
    :alt: figure 35.2

- The new account is added to the Requestor Accounts page.

**Edit/Delete an Account**

- Go to the :ref:`Requestor Accounts<requestor accounts>` page.

- The edit icon allows you to edit an Account and the delete icon lets you delete one.

.. _adf-35.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-35.3.png
    :align: center
    :alt: figure 35.3

.. note:: When you delete an Account, the Account label disappears from Requests that have already been created.     