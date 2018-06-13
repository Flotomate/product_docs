****************
Asset Management
****************

Adding Custom Asset Types
=========================

We have introduced the concept of Asset Type Hierarchy to make
cataloging of Assets simple. It is a predefined catalog of Asset Types,
which serves the purpose of giving you a generic umbrella term for every
Asset in the CMDB.

.. _adf-134.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-134.1.png
    :align: center
    :alt: figure 134.1

.. _adf-134.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-134.2.png
    :align: center
    :alt: figure 134.2

.. _adf-134.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-134.3.png
    :align: center
    :alt: figure 134.3

Flotomate allows you to add custom Asset Sub-Types in the Asset Type
Hierarchy. You can create sub-types up to two levels.

To add an Asset Type:

-  Go to **Admin** (A Navigation Tab) >> **Asset Types** (Asset
   Management).

.. _adf-135:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-135.png
    :align: center
    :alt: figure 135

-  The Asset Types page opens. Here you can add your sub-types in level
   two and three using the **Add** button.

**Editing Custom Types**

-  Go to **Admin** >. **Asset Types**.

-  You can change the name of any custom type using the Edit Icon or
   delete any type using the Delete Icon.

.. _adf-136:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-136.png
    :align: center
    :alt: figure 136

Adding an Asset Group
=====================

Flotomate allows you to categorize Assets in the CMDB into groups.
Groups are a convenient way to compartmentalize Assets based on certain
similarities.

Some of the benefits of using Asset Groups are:

-  Asset Groups help Technicians to manage Assets in the CMDB. For
   example: if a Technician is responsible for an Asset Group called
   DATA CENTER ASSETS then he can easily search for the Assets with the
   group name.

-  Groups are used in Hardware Asset notification. For example: in case
   there is a Hardware change in a specific Asset Group then a
   notification is sent to certain users.

**To Create an Asset Group:**

.. note:: This operation requires Admin rights.

1. Go to **Admin** >> **Asset Group** (Asset Management)

2. The Asset Groups page opens. Here you can view all your Groups and
   their Assets.

.. _adf-137:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-137.png
    :align: center
    :alt: figure 137

.. note:: You can access the Asset Groups page from Admin >> Asset Groups
          (under Asset Management).

3. Click on **Create an Asset Group** situated in the top right corner
   of the page. A dialog box opens with the following fields:

    a. **Name**: Provide a suitable name for the group.

    b. **Owner**: Select an owner of the group from the Technician list.

    c. **Description**: Write the purpose of the group.

.. _adf-138:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-138.png
    :align: center
    :alt: figure 138

4. When you are done hit **Create**. Your Asset Group is added to the
   Asset Groups page.

Software Type
=============

A Software Type tries to define the nature of existence of a Software
Asset. By default, Flotomate provides six Software Types out of the box.
They are as follows:

-  **Excluded**: These are all Software that does not need any managing.

-  **Managed**: These are all Software that needs managing with regards
   to License and Compliance.

-  **Freeware**: These are Software that is free to use.

-  **Prohibited**: These are Software that is not allowed to be used.

-  **Shareware**: These are Software that is running on a free Trial.

-  **Unidentified**: As the name suggests, these are unidentified
   Software with unknown source.

Adding a Software Type:
-----------------------

.. note:: This operation requires administrative rights.

Apart from the default Types, you can add more Software Type/Types. To
add a Software Type:

1. Go to **Admin** (A Navigation Tab) >> **Software Types** (Asset
   Management).

.. _adf-139:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-139.png
    :align: center
    :alt: figure 139

2. The Software Types page opens. Here you can view all your default
   and custom types. Click on **Add Software Type** situated in the top
   right corner.

.. _adf-140:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-140.png
    :align: center
    :alt: figure 140

3. The Add Software Type dialog box opens. Type in the details and
   click **Add**.

Adding a Manufacturer
=====================

Before adding a Manufacturer’s name to a Product, you have to add it in
Flotomate. In Flotomate you can maintain a list of manufacturers’ names
that you can associate with various Products in the system.

To Add a Manufacturer:

1. Go to **Admin** (A Navigation Tab) >> **Manufacturers** (Asset
   Management).

.. _adf-141:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-141.png
    :align: center
    :alt: figure 141

2. The Manufacturers page opens. Here you can view all the
   Manufacturers that you have added. Click on **Add Manufacturer**
   situated in the top right corner of the page.

.. _adf-142:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-142.png
    :align: center
    :alt: figure 142

3. The Add Manufacturer dialog box opens. Type in the Name of the
   Manufacturer and a Description, and you can maintain a record of
   sysOIDs (System OID) using the **ADD System OID** (:numref:`adf-142`)
   button.

   The sysOID is for SNMP devices. The product matches SNMP devices
   with Manufacturers using the sysOID. The first 12 characters of a
   sysOID gives enough information to perform the match. The
   matchmaking happens even when the manufacturer is not explicitly
   mentioned in a SNMP device.

4. When you are done, hit **Save** to add the Manufacturer.

**Editing Manufacturer**

1. Go to **Admin** >> **Manufacturers**.

2. In the Manufacturers page, click on the Edit Icon adjacent to the
   Manufacturer that you want to edit.

3. Perform your edits in the Edit Manufacturer dialog box and hit
   **Update**.

Barcode Configuration
=====================

You can have a variety of barcode prefixes when you are generating
barcodes for printing. In Barcode Configuration page is where you add
your own barcode prefixes.

**To Add New Barcode Prefix:**

-  Go to **Admin** (A Navigation tab) >> **Barcode Configuration**
   (Asset Management).

-  Barcode Configuration page opens, there you can see all the existing
   prefixes. Click on Add Prefix.

.. _adf-143:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-143.png
    :align: center
    :alt: figure 143

-  Add Prefix dialog box opens. There type a four character prefix and
   hit **Add**.

**To Delete a Prefix:**

-  In Barcode Configuration page, click on the Delete Icon adjacent to a
   prefix that you want to delete. On confirmation, the prefix gets
   deleted.

Adding a Product Type
=====================

A Product can be further categorized into Product Types. A Product Type
is a generic category to group Products. For example, Router is a
Product Type that describes Products like Asus, TP-Link, etc. In
Flotomate, you get a list of Product Types out of the box, but you can
also add more types.

**To Add a Product Type:**

1. Go to **Admin** (A Navigation Tab) >> **Product Types** (Asset
   Management).

.. _adf-144:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-144.png
    :align: center
    :alt: figure 144

2. The Product Types page opens. Here you can view all the Product
   Types added by you along with the predefined types. Now click on
   **Add Product Type** situated in the top right corner of the page.

.. _adf-145:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-145.png
    :align: center
    :alt: figure 145

3. You see the Add Product Type dialog box. You have to fill the
   following fields:
   
    a. **Name**: Type an appropriate Type name. For example, Desktop is
       a proper Product Type name.

    b. **Type**: It is a subdivision of a Product Type. There are four
       main Types to choose from:

        i.  **Asset**: It is a thing that can provide value
            generally for more than a year. For example, a Laptop
            computer.

        ii. **Component**: It refers to a functional part of an
            Asset. For example, a GPU card is a component that goes
            into a Desktop.

        iii. **Consumable**: It is a thing whose ability to deliver
             value gets exhausted within a short period, generally
             less than a year. For example, a Printer’s toner
             cartridge.

        iv.  **Others**: Anything that doesn’t fall in the above
             three Types.

    c. **Category**: Here you have to make a selection between an IT and
       Non-IT Asset. Learn :doc:`the difference between an IT and Non-IT Asset <asset-management-intro>`.

    d. **Description**: A short description of the Product Type.

  After filling the details hit **Save** to create the Product
  Type.

**Editing a Product Type**

.. _adf-146:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-146.png
    :align: center
    :alt: figure 146

.. note:: You can only change the description of the predefined Product
          Types. None of the predefined Product Types can be deleted.

-  Go to **Admin** (A Navigation Tab)>> **Product Types** (Asset
   Management).

-  In the Product Types page, click on the Edit Icon adjacent to the
   Product Type you want to edit.

-  Perform your edits in the Edit Product Type dialog box and hit
   **Update**.

In the Product Types page, click on the Delete Icon adjacent to the
Product Type that you want to delete. On confirmation, the Product Type
gets deleted.

RDP Configuration
=================

Remote Desktop is the ability of a computer to remotely connect to
another computer and control it as if the user were in front of the
remote machine. Remote access is generally done utilizing an
application.

You can remotely connect and control workstations in the CMDB using our
Agent application. Currently, Remote Desktop works on workstations
having either Windows or Ubuntu OS and brought in by an Agent.

Turning RDP On
--------------

Before you can initiate a remote session, you have to turn on the RDP
from Admin:

-  Go to **Admin** >> **RDP Configuration** (Asset Management).

.. _adf-147:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-147.png
    :align: center
    :alt: figure 147

-  The RDP Configuration dialog box opens. There toggle **Enable RDP**
   on.

.. _adf-148:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-148.png
    :align: center
    :alt: figure 148

-  If you are facing a problem in establishing a connection with some
   Agents then you can use the Fix RDP option in RDP Configuration
   dialog box to fix all available connections.