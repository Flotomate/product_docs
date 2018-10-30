******************
LDAP Configuration
******************

Flotomate allows batch upload of **Requestors** from an LDAP request.
LDAP is a protocol used by enterprises to access an Active Directory of
their employees. It is mainly used for email clients and other contact
search programs.

Flotomate establishes a connection with a distributed directory
information system using the user provided information, and it makes
queries using the LDAP protocol. It fetches the employee details from
the server into the product.

Configure LDAP
==============

1. Go to **Admin** >> **LDAP Configuration** (IT Infrastructure).

2. LDAP Configurations page opens. Here you can see all your existing
   LDAP servers if any. Click **Add LDAP Configuration** situated in the
   top right corner. You get the following dialog box:

.. _adf-73:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-73.png
    :align: center
    :alt: figure 73

.. _adf-74:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-74.png
    :align: center
    :alt: figure 74

3. Please refer :numref:`adf-73`. Give a name to the server. URL (field A) is
   the URL of the LDAP server which begins with ldap:// (ldaps:// if the
   connection is secured) followed by protocol components (IP address,
   and port number). A valid URL should look something like
   ldap://111.111.0.11:920. Base DN (field B) is an API reference for
   the LDAP object; basically, it tells us what to fetch from where to
   fetch from the LDAP server. Put you LDAP credentials in the User ID
   (field C) and Password (field D).

4. Please refer :numref:`adf-74`. Switch to the Mapping section of the dialog
   box. Here you have to enter the LDAP object attributes. There are
   two pre-defined fields (Name and Email). You can add more fields
   using the :doc:`Requestor Custom Field <admin-customization>` option. You can edit and delete a
   custom field in the :doc:`Custom Field <admin-customization>` section of Admin.

5. Hit **Add** to save your LDAP server.

The credentials required for LDAP configuration are of the LDAP Admin.
In case, credentials are not available then a new user can be created in
their Active Directory. Please refer the document LDAP Configuration by
Creating New User.

Edit LDAP Server
================

1. Open LDAP Configurations page and select the server that you want to
   edit.

.. _adf-75:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-75.png
    :align: center
    :alt: figure 75

2. Click **Edit** from the right-side details pane. The Edit LDAP
   Configuration dialog box opens. Make the changes and hit **Update**.

Please refer :numref:`adf-13`. Go to the LDAP Configurations page and select
the server name that you want to delete and click on Action Menu. Click
on **Delete** from the pop-up menu. On confirmation, the server gets
deleted.

LDAP Connection Test
====================

In the LDAP Configurations page, you can check an LDAP server’s
connection with the product by using the **Test Connection** option in
:numref:`adf-75`.

Setting LDAP Import Schedule
============================

Scheduling allows you to periodically import employee details from the
server. This feature helps you to keep the Requestor list up to date.

.. _adf-76:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-76.png
    :align: center
    :alt: figure 76

1. Open **LDAP Configurations** page and select the server that you want
   to schedule an import. Under **Import Schedule**, set a schedule
   cycle for importing the Requestors. Flotomate offers three options:
   Daily, Weekly, and Monthly.

   a. Importing daily requires a start date and time; after that, the
      importing happens every day at the set time.

   b. Importing weekly requires you to set the days in a week on which
      the importing happens.

   c. Importing monthly requires you to set a day of the month and the
      months in which the importing happens.

2. After setting the schedule, hit **Save Schedule** to save your
   changes.

Edit/ Disable LDAP Schedule
===========================

You can later edit the schedule using the **Edit Schedule** option. The
Scheduled toggle turns on/off a schedule.

.. _adf-77:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-77.png
    :align: center
    :alt: figure 77