*****************
Manage Requestors
*****************

The Requestors are people who are seeking information, change or
solution to a problem through our platform. They are the users of the
product, and almost all of the product features are geared towards
delivering IT services to Requestors. So it is important to manage their
information in the product.

Motadata allows you to add Requestors individually and bulk upload
through LDAP server synchronization. Once uploaded, you can manage them
from the Admin section.

.. note:: All Technician are Requestors by default and enjoy their rights and permissions, and even more.

.. _view-requestor:

Open Requestors Page
====================

The Requestors page is where you can add, view, update and delete
Requestors in the product.

.. note:: You need to have admin rights or be a Super User to add and modify Requestors.

1. Log in to Motadata, and go to **Admin** from the Navigation Tabs

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
===========================

You can add Requestors individually by entering their details.

:ref:`Who are Requestors? <manage requestors>`

-  Go to **Admin** >> **Requestors** (Users).

-  On the **Requestors** page, click **Add Requestor** situated in
   the top right corner of the page. You get the **Add** **Requestor**
   dialog box.

-  Fill in the details of the new Requestor along with a password. You
   can mark a Requestor as VIP if he/she is a critical person in the
   organization. This gives him/her the following benefits:

   a. Tickets created with the VIP label can be treated
      with priority by the Technicians.

   b. Specific Workflows, SLAs, and Reports can be created for VIPs.

-  The **Logon Name** is the Workstation user-name of the Requester. 
   The field value is used for auto-assigning the Requester's workstation to his/her name. The assignment happens during asset 
   discovery. :ref:`Learn more <Preference>`.

   .. note:: A requester can use the logon name instead of the email for portal login.  

-  You can create custom fields that allow you to store additional information. :ref:`Learn More (see Custom Fields) <requestor-custom-field>`    

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
===========================

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

Self-Registration of Requesters
===============================

An admin can allow a user to create a Requester account from the Customer Portal. Enabling Self-Registration adds a button on the
Customer Portal that can be used by anyone (who has access to the customer portal) to create a Requester account. 

.. note:: Self-Registration can be enabled from **Admin** >> **Requestors** (under Users) >> **Self Registration Config**.

.. _adf-12.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-12.1.png
    :align: center
    :alt: figure 12.1

While enabling Self-Registration you have two options:

- **Allow Everyone**: A **Sign Up** button appears on the Customer Portal. Anyone who has access to the Customer Portal can create a Requester
  account. 

- **Set of Domain**: A Sign Up button appears on the Customer Portal. But an admin can restrict who can register by defining
  domains. By adding a domain, only people with an email id belonging to that domain (or any other domain already being added) can register. 

.. _adf-12.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-12.2.png
    :align: center
    :alt: figure 12.2 

When you done configuring, click on **Update** to start Self-Registration.

Import Requestors Using LDAP
============================

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
======================

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
=================================

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

   c. :ref:`Location <ad-location>` of the Technician. This is different from the Authorized Location field.

   d. The **Authorized Location** field grants the permission to view the data of the selected location only. The feature is called
      :ref:`Location Scope <Data Segregation with Location Scope>`. 

-  When you are done, hit **Add**.

Block a Requestor
=================

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
=========================

You can delete multiple Requestors at once from the :ref:`Requestors
page <view-requestor>`. Select one or more Requestors. The
**Archive** button appears above the display pane.

.. _adf-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-19.png
    :align: center
    :alt: figure 19

Clicking on Archive deletes the selected Requestors after confirmation.