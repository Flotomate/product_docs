****************
Modifying Assets
****************

Our Asset Management tool allows Technicians to edit the information of
an Asset in the CMDB. What a Technician can edit depends on the
following things:

-  `Asset Type <#adding-custom-asset-types>`__

-  Whether the Asset was added manually or discovered.

-  Technician Roles.

-  Custom Rules.

Modifying Properties, Components and Users of a Hardware Asset
==============================================================

Different Asset types have different Properties, and Components are only
in Hardware Assets. The below description tells you on how to go about
modifying an Asset, which is same for all the Asset types.

.. note:: Here a Hardware Asset is referred to a computer.

Add/Edit Properties:
--------------------

Go to the `Details View <#searching-assets>`__ of a Hardware Asset.

Scroll down to Properties. You get the following heads:

    a. **Computer Properties**:

        .. _amf-102:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-102.png
            :align: center
            :alt: figure 102

    b. **Hardware**:

        .. _amf-103:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-103.png
            :align: center
            :alt: figure 103

You can edit the fields by clicking on the Edit Icon.

Add / Edit /Delete Components:
------------------------------

Two tabs (Hardware and Software) represent the Components:

-  **Hardware**: It is a list of all hardware components of a computer
   along with the details. The details of each component are editable,
   and you can add additional components if you want.

    .. _amf-104:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-104.png
        :align: center
        :alt: figure 104

   Select a component type and then click on the Plus Icon. For example, on
   clicking the Plus Icon in the Ram type opens the following window:

    .. _amf-105:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-105.png
        :align: center
        :alt: figure 105

   After adding the RAM, the component appears under RAM. You can use the
   Edit Icon (:numref:`amf-104`) situated in the component’s details pane to
   change its fields.

   You can delete the component using the Delete Icon (:numref:`amf-104`).

-  **Software**: Here you can view all the installed Software on the
   computer.

    .. _amf-106:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-106.png
        :align: center
        :alt: figure 106

   Click on **Add Software**. The Add Software dialog box opens. You get
   the following fields.

   Fill in the required fields and hit **Add** to add the Software. If the
   name of the Software already exists in the CMDB, then it is linked with
   the existing one. Else, the entry has no effect on the CMDB.

    .. _amf-107:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-107.png
        :align: center
        :alt: figure 107

   You can edit and delete any Software using the Edit and Delete Icons.
   But a deleted Asset would reappear if it is discovered in the next
   discovery cycle.

Add/Edit/Delete Users
---------------------

The Users tab lists all the local user accounts in the computers.

.. _amf-108:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-108.png
    :align: center
    :alt: figure 108

-  You can add a new user by clicking on **Add Users**, and then fill
   the Add User dialog box. The new user is added to the **Users tab**.

.. _amf-109:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-109.png
    :align: center
    :alt: figure 109

-  In the Users tab, you can edit the fields (some fields may not be
   editable if the Asset is discovered) of any user using the Edit Icon
   adjacent to a user.

-  The Delete Icon, next to Edit, deletes a user from the Users tab.

Asset Custom Rules
==================

You can control what part of an Asset can be manually modified
regardless of the method of discovery. You do this using Custom Rules
pertaining to Assets. You would be needing admin rights to access the
options.

-  Go to **Admin** (one of the navigation tabs) >> **Asset Custom
   Rules** (Asset Management).

.. _amf-110:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-110.png
    :align: center
    :alt: figure 110

-  The Custom Rules page opens. There you get three options:

   a. Whether to allow manual updating of Hardware components.

   b. Whether to allow manual updating of Software components.

   c. Whether to allow manual updating of Users.

.. _amf-111:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-111.png
    :align: center
    :alt: figure 111

Asset Custom Fields
===================

You can add custom fields in the property and component section of an
Asset. Custom fields are excluded from the discovery process; you have
to enter data manually into these fields.

To Add a Field:

-  Go to **Admin** (A Navigation tab) >> **Asset Custom Fields** (Asset
   Management).

.. _amf-112:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-112.png
    :align: center
    :alt: figure 112

-  Custom Fields page opens. Here you can add two types of fields.

    a. **Text** **Field**: It is a type of field that accepts a
       user-defined value.

        .. _amf-113:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-113.png
            :align: center
            :alt: figure 113

       The Label is the visible name of the field. Default value is the
       pre-populated value in the input area.

    b. **Selection Field**: It is a type of field that accepts a user
       response from a predefined list.

        .. _amf-114:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-114.png
            :align: center
            :alt: figure 114

       The Label is the visible name of the field. You add the list items using
       the plus icon. You can edit/delete a list item using the Edit/ Delete
       Icon. You can make a list item the default value (pre-selected value)
       using the adjacent Default Value toggle. You can change the order of the
       items by drag-drop.

       Select a field type (:numref:`amf-112`) and click on Add.

-  Now you have to choose where to add the field. In the Asset
   Information section you decide on the following things:

    .. _amf-115:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-115.png
        :align: center
        :alt: figure 115

    a. **Asset Type**: Here you decide which Asset Type carries the field.
       The sub-types of the select type doesn’t carry the field. If Asset
       Property and Asset Component are left none, then the field appears
       under the head **Additional Fields** in **Properties**.

        .. _amf-116:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-116.png
            :align: center
            :alt: figure 116

    b. **Asset Property**: You can add the field to a particular property of
       an Asset type. The available properties are visible as a drop-down
       list. If the list is empty then the Asset type doesn’t have any
       properties.

        .. _amf-117.1:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-117.1.png
            :align: center
            :alt: figure 117.1

        .. _amf-117.2:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-117.2.png
            :align: center
            :alt: figure 117.2

    c. **Asset Component**: You can either put a field in property or
       component. In the same way, you can add the field to a particular
       component.

        .. _amf-118.1:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-118.1.png
            :align: center
            :alt: figure 118.1

        .. _amf-118.2:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-118.2.png
            :align: center
            :alt: figure 118.2
