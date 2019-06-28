***************
Asset List View
***************

The Asset Management interface shows relevant data whenever required.
This is achieved with the help of filters, search options, and
predefined hierarchies.

The Asset List View is an essential component of the interface. It is
the visual part of the CMDB, which gives a point and click interface to
manage all Assets. It provides you the option to import Assets and
export individual Asset details on to a local machine, and many more.
The List View is divided across four class of Assets:

-  Hardware Assets

-  Software Assets

-  Other IT Assets

-  Non-IT Assets

Click on **Asset**, a Navigation Tab, which takes you to the Asset List
View. The default filter is **All Hardware IT Assets**.

.. _amf-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-1.png
   :align: center
   :alt: figure 1

You can switch to other classes using the class filter in :numref:`amf-1`. The
view differ across classes in terms of filters and options.

.. _amf-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-2.png
   :align: center
   :alt: figure 2

.. note:: Kindly refer to :numref:`amf-2`.

-  Section A, B, C & D are the :ref:`search features <Searching Assets>`.

-  Section-E is the checkbox which you can use to select all the Assets
   currently viewable in the list area.

-  Section-F is the list area that shows all the Assets. The view is
   tabular in form with each line containing seven properties of an
   Asset. These properties are:

   a. **ID**: Unique identifier of an Asset.

   b. **Name**: A human given identifier of an Asset.

   c. **Asset** **Type**: It tells us where the Asset belongs in the
      Asset Type Hierarchy. This field supports quick edit which means
      you can change the value by clicking on the field value.

   d. **Status**: The current state of the Asset in terms of usability.
      This field supports quick edit. Learn how to add :ref:`custom statuses <ad-add-custom-status>`. 

   e. **Used by**: It tells us about the person who uses the Asset. This
      field supports quick edit.

   f. **IP Address**: The IP address of the device/machine. It does not
      support quick edit.

   g. **Host**: Hostnames are human-readable nicknames that correspond
      to the address of a device/machine connected to a network. The
      field does not support quick edit.

      **Software Asset Specific Properties:**

   h. **Version**: The version of the Software Asset as stated by the
      vendor.

   i. **Software Type**: Types generally define the nature of usage. A
      Software Asset has either a predefined type or a custom one.

   j. **Software Category**: One of the many ways of categorization.

   k. **Installation Count**: It shows the total number of workstations (desktops and laptops) having the software. 

      Each Asset has an Action Menu (at far right) from where they can
      perform the following operations: :ref:`Scan Now<scanning-a-single-hardware-computer>`, 
      :ref:`Exclude from Scanning<excluding an asset from scanning>`, 
      :ref:`Viewing Audit Trail<am-viewing-audit-trail>`, 
      :doc:`Export Asset<export-asset-details>`, 
      :ref:`Remote Desktop <Remote Desktop>`,
      and Open Asset in new tab.

-  Section-G gives you the option to set the number of Assets visible
   per page; the highest is 100 per page. You can change the default
   number from your profile.

-  Section-H houses the following options:

   a. :ref:`Import Asset<importing assets in bulk using csv>`

   b. :ref:`Scan Barcode<opening asset using barcode>`

   c. :ref:`Generate Barcode <Generate Barcodes>`

   d. :ref:`Manage Asset Groups<managing asset groups>`

   e. :ref:`Asset in Stage<delete-assets>`

   f. :ref:`Software Normalization` (for software assets).

-  When you select one or more Assets you get the following bulk
   operations:

   a. :ref:`Bulk Update<am-bulk-update>`

   b. :ref:`Reconcile <Asset Reconciliation>` 

   c. :ref:`Delete<delete-assets>`

   d. :ref:`Generate Barcodes <Print Asset Barcode>`

   e. :ref:`Move to Stage<delete-assets>`

-  Other features specifically for Software Assets are:

   f. :ref:`Mark as Prohibited <manually flagging a software asset as prohibited>`

   g. :ref:`Mark as Managed Software <Setting Software Type as Managed>`

   h. :ref:`Mark for Notification <Marking Software Assets>`

   i. :ref:`Consolidate <consolidating software>`

Searching Assets
================

There are two broad ways to search Assets in the product:

-  Using Search Bar

-  Using Filters

.. _am-using-search-bar:

Using Search Bar
----------------

The way the search bar works is same across all the Asset Classes. The
only difference being is the available search options in each class.

Product allows you to perform Advanced Search using various combinations
of predefined search options and keywords. If you want to see the list
of available options, then click on the search bar. You can select a
single option or multiple options from the drop-down list.

.. _amf-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-3.png
   :align: center
   :alt: figure 3

You can search Assets with keywords in the search field. When you
provide a keyword, Motadata searches all the Assets with the keyword in
their ID, Description, Name, Tags, and Display Name field. An Asset has
to have at least one field matched (partial or full) with the keyword;
in case there are multiple keywords, the Asset has to have at least one
field matched for each keyword.

A search query can be made up of search options and keywords. In any
case, the output yields Assets that satisfy all the parameters of the
search query.

For example, you are looking for all Assets containing the keyword Sunil
in Name and have Status as **In Use**. You would have the following
search query:

.. _amf-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-4.png
   :align: center
   :alt: figure 4

Between two different conditions of the same option type OR logic is
followed. Between different option types AND logic is followed. An
example of same type contradiction is Status **In Use** vs. Status
**Missing**. Between inputted keywords and conditions AND logic is
followed.

Custom Filter
^^^^^^^^^^^^^

You can make a filter using search options and keywords and save it by
clicking on the star icon to the far left of the search bar. Saved
searches appear as filters in the header section (section-A) of the
Figure 2.

.. _amf-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-5.png
   :align: center
   :alt: figure 5

Using Filters
-------------

The available filters differ across Asset classes. Each having their own
set of filters:

Hardware Asset
^^^^^^^^^^^^^^

There are five predefined search filters in the header section of
:doc:`List View<asset-list-view>`:

      .. _amf-6:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-6.png
            :align: center
            :alt: figure 6

      You can pin a filter using the Pin Icon. The pinned filter is applied by
      default whenever someone clicks on **Asset** (A Navigation Tab) to go to
      the List View.

            a. **All Hardware IT Assets**: Shows you all the available Hardware
               Assets in the system.

            b. **All H/w Asset Managed By Me**: Shows all the Hardware Assets with
               your name in the Managed By field.

            c. **All H/w Asset In User**: All Hardware Assets with the status **In
               Use**.

            d. **All H/w Windows Assets**: All Hardware Assets with the Windows OS.

            e. **All H/w Ubuntu Linux Assets**: All Hardware Assets with the Ubuntu Linux OS.

There are filters based on Asset Type:

   a. **Computer**:

      i.   Laptop

      ii.  Server

      iii. Desktop

   b. **SNMP Devices**:

      i. Routers

      ii.  Printers

      iii. Switches

Software Asset
^^^^^^^^^^^^^^

There are four predefined search filters in the header section of
:ref:`Asset List View`.

      .. _amf-7:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-7.png
            :align: center
            :alt: figure 7

You can pin a filter using the Pin Icon. The pinned filter is applied by
default whenever someone clicks on **Asset** (A Navigation Tab) to go to
the List View.

      a. **All Software IT Assets**: Shows all the available Software Assets.

      b. **All Managed Software**: Shows all Software Assets with the Software Type set to Managed.

      c. **All Prohibited Software**: Shows all Software Assets with the Software Type set to **Prohibited**.  

      d. **All Software Managed By Me**: Shows all Software Assets with your name in the Managed By field.

There are filters to isolate an Asset Type:

   a. OS

   b. Web Server

   c. **Application**:

      i.  Managed

      ii. Prohibited

   d. Database

Other IT Assets
^^^^^^^^^^^^^^^

There are three predefined search filters in the header section of
:doc:`List View<asset-list-view>`:

      .. _amf-8:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-8.png
            :align: center
            :alt: figure 8

You can pin a filter using the Pin Icon. The pinned filter is applied by
default whenever someone clicks on **Asset** (A Navigation Tab) to go to
the List View.

      a. **All Other IT Assets**: Shows you all the available Other IT Assets.

      b. **All Other IT Assets Managed By Me**: Shows all Other IT Assets with your name in the Managed By field.

      c. **All Other IT Assets Added in 30 days**: Shows you Assets added in the last 30 days.

There are filters to isolate an Asset Type:

   a. Service

   b. Cloud

   c. Others

.. _am-bulk-update:

Bulk Update Assets
==================

Motadata supports bulk update of Asset information of multiple Assets
at once. The dialog box to perform this operation is same across all the
classes. To perform the bulk update:

1. Go to the :ref:`Asset List View` of any class.

2. Select Assets on which you want to perform Bulk Update. The Bulk
   Update button appears above the pane. Click on **Bulk Update**.

.. _amf-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-9.png
   :align: center
   :alt: figure 9

3. The Bulk Update Assets dialog box opens, You can update the following
   fields of the selected Assets:

   a. Asset Type: Based on Asset Type hierarchy.

   b. Asset Group; Learn :ref:`how to add Asset Groups<adding an asset group>`.

   c. Status: Learn about Status

   d. Impact: Either Low, Self, On Department or Business.

   e. Tags: You can replace the existing tags, or append tags by
      selecting **Append Tags to existing tags**.

   f. Product: Learn about :ref:`Product<am-product>`.

   g. Vendor: Learn about :ref:`Vendor<am-vendor>`.

   h. Used By: Update the user of the Assets.

   i. Managed By: The Technician who is going to manage the Assets. The
      field is populated from the Technician list in the system.

   j. Location: Locations of the Assets

   k. Business Service: Which business services do the Assets affect?

   l. Software Type: This field is available only for Software Assets. 

   Number of Assets that are going to be updated is visible in the
   Update button. When you are done hit **Update** to save your
   changes.

.. _delete-assets:

Delete/Stage Assets
===================

You can delete multiple Assets from the Asset List View. Archiving
permanently deletes the Assets from the CMDB. The process is same across
all the classes.

If you want to remove Assets from the CMDB but don’t want to delete them
permanently, then you can Stage the Assets. Staging an Asset removes it
from the CMDB and puts it in isolation. Staged Assets don’t reappear
after a discovery process.

**To Delete/Stage Assets:**

-  Go to the :doc:`Asset List View<asset-list-view>` of any class.

-  Select the Assets that you want to delete. The **Delete** button
   appears above the listing area.

.. _amf-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-10.png
   :align: center
   :alt: figure 10

-  Click on the **Delete** button. On confirmation, the Asset/Assets are
   deleted from the CMDB.

-  If you don’t want to delete the Asset/Assets then you can stage them.
   Select the Assets and click on the **Move to Stage** button (in Asset
   List View). On confirmation, the tool stages the Assets.

.. _amf-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-11.png
   :align: center
   :alt: figure 11

**Add an Asset Back to CMDB from Stage:**

-  Go to the :doc:`Asset List View<asset-list-view>`.

-  Click on **Asset in Stage** from the Action Menu.

.. _amf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-12.png
   :align: center
   :alt: figure 12

-  The Asset in Stage page opens; it lists all Staged Assets. You can
   add an Asset back to the CMDB by clicking on an Asset’s **Add**
   button.

.. _amf-13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-13.png
   :align: center
   :alt: figure 13
