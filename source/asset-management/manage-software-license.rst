**************************
Managing Software Licenses
**************************

A Software License is an instrument that governs the use and
redistribution of the Software. It exists in the form of an agreement
between the Software Vendor and the purchaser of the Software. The
License agreement is referred to as **End User License Agreement** and
contains information like expire date of the License, terms and
condition of usage, and redistribution clause.

We understand that managing Software Licenses is vital to stay
compliant. So we have developed a robust License management module that
aims to streamline all related processes. Using our module, you can
manage License usage and track compliance violation.

Understanding the License Types:
================================

We support ten types of Licenses out of the box. They are as follows:

-  **Single Machine**: Also referred to as Single User License. This
   type of License grants a single user to use the Software either on a
   single machine or multiple machines. Flotomate automatically sets the
   Purchase Count for this type to one.

-  **Multiple Machine**: This type of License grants multiple users to
   use the Software package on multiple machines.

-  **Enterprise (Perpetual)**: Typically granted to an organization,
   this type of License allows unlimited use of the Software in the
   organization for a continuous period. Activations are done using one
   master key rather than multiple keys.

-  **Unlimited Machines**: In this type of License, an organization buys
   the right to use the Software for a specific period. When the period
   is over, the License is renewed. During the usage period, the License
   can be used by an unlimited number of machines.

-  **OEM**: This type of License is applicable for Software that comes
   preinstalled with hardware. The License limits the use of the
   Software on a specific Hardware.

-  **Single User**: This is an exclusive License for a defined user who
   uses the Software. The License carries the name of the user.

-  **Node Lock**: A Node Lock License is an encrypted key that is locked
   to a specific machine. Flotomate automatically sets the Purchase
   Count for this type to one.

-  **Volume Users**: A Volume License denotes the product key used when
   installing software licensed in bulk, which allows a single product
   key to be used for multiple users.

-  **Unlimited Users**: This type of License allows unlimited use of the
   Software by users for a specific period.

-  **Free License**: This type of License allows the free use of the
   Software.

Adding a License 
================

1. Go to **Asset** (A Navigation Tab) >> **Software Licenses**.

.. _amf-123:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-123.png
    :align: center
    :alt: figure 123

2. The Software Licenses page opens. Here you can view all your
   existing Licenses. Click on **Add Software License** situated in the
   top right corner.

.. _amf-124:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-124.png
    :align: center
    :alt: figure 124

3. The Add Software License dialog box appears with the following fields:

    a. **Name**: A Proper name should identify the association of the
       License with a Software.

    b. **Product Name**: This refers to the Product for which the
       License is meant.

    c. **Version**: Type in the version of the License. This can be a
       user define or something mentioned in the License Agreement.

    d. **License Type**: Learn more about the :ref:`License Types <understanding the license types>`.

    e. **Description**: A short description of the License.

4. Type in the details and hit **Add**. You are taken to the License
   Details View where you can add additional information about the
   License.

Associating a Software License with a Software Asset
====================================================

.. note:: Here a Software Asset refers to any Asset having an Asset Type as
Software or any sub-type of Software.

The functional aspect of having a Software License in Flotomate starts
with linking a License with a Software Asset which has the same Product
Type as the License.

.. note:: A License can be associated with only one Software Asset.

**To make an association:**

1. Go to **Asset** (A Navigation Tab) >> :doc:`Asset List View <asset-list-view>`.

2. Select a Software Asset with the same Product Type as the License
   and head to its Details View.

.. _amf-125:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-125.png
    :align: center
    :alt: figure 125

3. The **License** tab only appears when the Software Type is set to
   **Managed**. Change the Software Type to **Manage** from the **More
   Details** section if you do not see the **License** tab under
   **Details**.

4. The **License** tab shows the associated License if any. In the
   **License** tab, click on the **Associate License** button.

5. The **Associate License with software** dialog box opens. Here you
   can view all un-associated Licenses. You can search for available
   Licenses using the search bar using search options. Click the search
   bar to access the search options.

    .. _amf-126:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-126.png
        :align: center
        :alt: figure 126

6. Select a License and click **Associate Selected License**. The
   License is added to the **License** tab of the Asset.

License Details View
====================

A Software License is a legal instrument that holds vital information
that forms the basis for compliance management. Flotomate allows users
to manage such information from the Details View of a License.

Every License in Flotomate has a Details View that shows all the
information about the License. You are taken to the Details View after
adding a License in the system, but that does not mean you cannot access
the Details View anytime later.

To Access the Details View:

1. Go to **Asset** (A Navigation Tab) >> **Software Licenses**.

.. _amf-127:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-127.png
    :align: center
    :alt: figure 127

2. Here you can view all existing Licenses. You can search Licenses
   using the search bar with search options. Click the search bar to
   access the search options.

.. _amf-128:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-128.png
    :align: center
    :alt: figure 128

3. In the Software Licenses page, click on the **Edit Icon** adjacent
   to a License to open its Details View.

.. _amf-129:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-129.png
    :align: center
    :alt: figure 129

Please refer to the sections in :numref:`amf-129` while reading the below
description:

-  Section-A houses the :ref:`Updating License Name and Description <updating license name and description>` feature.

-  Section-B shows you the License Type and to which Product the License
   is related. Learn more about :ref:`License Types <understanding the license types>`. You cannot modify these
   fields.

-  Section-C shows you the description of the License.

-  Section-D appears in Licences with the type either Single Machine,
   Multiple Machines, or Node Lock. It shows the following data points:

   a. **Allocations**: This shows the number of machines allocated to
      the License. Flotomate allows more Allocation than the Purchase
      Count.

   b. **Purchase Count**: This refers to the total allowable
      installation of the associated Software. Some License Types have a
      predefined count field that you cannot change, and there are types
      where the count field is not present.

   c. **Installation Count**: The number shows the actual installation
      of the Software associated with the License across all Assets
      irrespective of whether they are allocated or not.

-  Section-E has the :ref:`Details <updating license details>` and
   Allocation tabs. The **Allocation** tab shows all the machines that
   can install the Licensed Software. Allocations are done manually
   using the options available under the tab. Certain License Types
   allow you to add users instead of Assets. Learn more about
   :ref:`Allocation <allocating-machines-in-a-software-license>`.

-  Section-F houses the **Action Menu**. Using the menu, you can access
   the :ref:`Compliance Settings <managing license compliance>` of the
   License.

-  Section-G shows whether the License is associated with a Software or
   not.

Updating License Name and Description.
======================================

The License ID precedes the Name of the License in section-A of :numref:`amf-129`. 
The Description of the License can be viewed in More Details
(section-C of :numref:`amf-129`). You can edit both the Name and Description of
the License, but not the ID.

**To Edit Name and Description:**

-  Click on the Edit Icon next to the Name.

-  The Edit Software License Page opens. Type in the new Name and
   Description and hit **Update**.

.. _amf-130:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-130.png
    :align: center
    :alt: figure 130

Updating License Details
========================

The bulk of the information about the License is stored in the Details
tab (section-E of :numref:`amf-129`) across three heads: License Info,
Ownership, and Attachments.

Clicking on the Details tab makes the three heads visible in the display
pane below. Clicking on a head shows the available fields. Each head has
an Edit Icon that you can use to edit the fields.

.. _amf-131:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-131.png
    :align: center
    :alt: figure 131

-  **License Info**: You have the following fields in this section:

   a. **Purchase Date**: This is the purchase date of the License as
      mentioned on the invoice.

   b. **Expiry Date**: The expiry date is always as per License
      Agreement.

   c. **Cost**: This is the cost of acquiring the License as mentioned
      on the invoice.

   d. **License Key**: The actual key that is used to activate the
      Software.

   e. **Version**: The version details of the License.

   f. **Purchase Count**: This refers to the total allowable
      installation of the Software that is associated with the License.
      Some License Types have a predefined count field that you cannot
      change, and there are types where the count field is not present.

-  **Ownership**: All License Types support the editing of the following
   fields: Owner Name and Owner Email. The owner is the end user of the
   License.

-  **Attachments**: You can upload the Invoice and License Agreement in
   this section.

.. _allocating-machines-in-a-software-license:

Allocating Machines/Users in a Software License 
===============================================

.. note:: Here a machine is referred to either a Workstation, Laptop or Server Asset.

Allocation gives a machine/user, in the CMDB/product, the right to
install a Licensed Software. It lets Flotomate keep a count of all valid
installations of a Licensed Software. The count is vital for activating
compliance specific notifications relating to over and under usage of a
Licensed Software.

The Allocation is done manually on the Details View of a Software
License. In case the License is either Single User, Volume Users or
Unlimited Users, you have to add users instead of Assets.

**To perform Asset Allocation:**

1. Go to **Asset** (A Navigation Tab) >> **Software Licenses**.

2. Click on the **Edit Icon** adjacent to the License that needs
   Allocation, or just click the License name.

3. The Details View of the License opens. Scroll down to the
   **Allocation Tab**. Here you can view the list of all the existing
   Allocations.

.. _amf-132:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-132.png
    :align: center
    :alt: figure 132

4. Click on the **Allocate** button in the **Allocation** tab. The
   Allocate Assets dialog box opens.

.. _amf-133:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-133.png
    :align: center
    :alt: figure 133

5. The Allocate Assets dialog box shows you all the supported Assets
   (Workstations, Laptops, and Servers) in the CMDB. You can search
   supported Assets and allocate them.

   The search bar allows you to use various combinations of predefined
   search options and keywords. If you want to see the list of all
   available search options, then click on the search bar. You can
   select an option or multiple options from the drop-down list.

    .. _amf-134:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-134.png
        :align: center
        :alt: figure 134

   You can search supported Assets with keywords. When you provide a
   keyword, Flotomate searches all the supported Assets with the keyword in
   Name, Description, and Tags.

   You can make a filter using a chain of predefined search options and
   keywords.

   Perform search and find the Assets that you want to allocate.

6. Select the Assets and click on **Allocate** situated in the top
   right corner. The selected Assets are allocated to the License.

**To Perform User Allocation:**

1. Just like allocating Assets, certain License Types require you to
   allocate users instead of Assets. In the Details View of such a
   License type, click on the **User Allocation** tab.

    .. _amf-135:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-135.png
        :align: center
        :alt: figure 135

   The tab shows all current users added to the License if any.

2. To add a new user/users, click on the **Allocate License User**
   button. This opens the **Allocate License User** dialog box.

    .. _amf-136:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-136.png
        :align: center
        :alt: figure 136

3. In the dialog box, you can view the names of all the Requesters in
   the system. You can select multiple users (Requesters) by clicking
   on the checkbox against their names.

   The search bar allows you to search users based on the following
   options:

    a. Name

    b. Email

    c. Location

    d. Department

    e. VIP Requester status

   You can set multiple conditions using the options; you can access
   them by clicking on the search bar.

   Select the users whom you want to allocate the License and click
   on the **Allocate** button. Now you have successfully allocated
   the License.

Managing License Compliance
===========================

A company is exposed to different kinds of risks when it is not aware of
the Software that is being run on its machines. One such risk is
overutilization of a Licensed Software, and such risks come under the
umbrella term compliance management. It is a set of pre-agreed upon
conditions related to the usage of a Software.

Flotomate tracks all the Software that is installed on various Hardware
Assets, and the process helps in compliance management. Currently,
Flotomate supports the generation of notifications upon nine types of
violations.

There is a separate thread in Flotomate that checks all Licensed
Software and their installation instances against specific parameters;
those parameters are as follows:

-  Utilization

-  Purchase Count

-  Installation Count

-  Expiry Date of the License

-  Hostname (Node-Locked)

-  Software Type

-  Allocated Machines

Out of all the above parameters, Utilization Count, Purchase Count,
Expiry Date and Allocated Machines are License specific parameters.

.. _am-utilization:

Utilization
-----------

Utilization refers to the total utilization of the Licensed Software
across all managed IT Assets. The system denotes it as a percentage
where the numerator is the Installation Count and denominator, Purchase
Count.

Installation Count
------------------

Installation Count is the total number of installation of a Licensed
Software. It does not discriminate between licensed installation and
unlicensed installation.

Purchase Count
--------------

Purchase Count refers to the total allowable installation of a Licensed
Software.

+------------------------+-------------------------------------------+
| License Type           | Purchase Count                            |
+========================+===========================================+
| Single Machine         | Default value set to one                  |
+------------------------+-------------------------------------------+
| Multiple Machines      | Can be set to as many as possible         |
+------------------------+-------------------------------------------+
| Enterprise (Perpetual) | Not applicable                            |
+------------------------+-------------------------------------------+
| Unlimited Machines     | Not applicable                            |
+------------------------+-------------------------------------------+
| OEM                    | Not applicable                            |
+------------------------+-------------------------------------------+
| Single User            | The Count is equal to the number of users |
+------------------------+-------------------------------------------+
| Node Locked            | Default value set to one                  |
+------------------------+-------------------------------------------+
| Volume Users           | The Count is equal to the number of users |
+------------------------+-------------------------------------------+
| Unlimited Users        | Not applicable                            |
+------------------------+-------------------------------------------+
| Free License           | Not applicable                            |
+------------------------+-------------------------------------------+

Compliance Settings
-------------------

Flotomate allows you to set under and overutilization notifications for
Multiple Machines and Volume Users License Types. You have to define the
underutilization and overutilization threshold for above mentioned
License Types to enable utilization monitoring.

For every other License Types, except Free License, you have to add
Requester Groups and Emails to enable compliance violation
notifications.

1. Go to **Asset** (A Navigation Tab) >> **Software Licenses**.

2. Select a License and head to its Details View.

3. On the Details View, click the Action Menu (section-E of :numref:`amf-129`)
   and select **Compliance Settings**.

.. _amf-137:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-137.png
    :align: center
    :alt: figure 137

.. note:: Please refer to :numref:`137`.

.. note:: Section C in above figure is only available on Multiple Machines and Volume Users License Type.

-  Section-A allows you to add Requestor Groups that are going to
   receive notifications (group members are the :ref:`admin for the notification <different types of notifications>`).

-  Section-B is where you add emails of individuals who are going to
   receive notifications along with the groups (recipients are the
   :ref:`admin for the notification <different types of notifications>`).

-  In section-C is where you decide the threshold for overutilization
   and underutilization in percentage. For example, if Installation
   Count of a Licensed Software is equal to its Purchase Count then
   utilization is 100 percent.

   a. If over-utilization limit is set to 90%, then 91% utilization
      would trigger a notification to the admin.

   b. If under-utilization limit is set to 80% and utilization is 98%,
      then a fall of utilization below 80% would trigger a notification
      to the admin.