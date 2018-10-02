********************
Manage Asset Details
********************

Another vital component of the interface is the Details View. Every
Asset in the CMDB has a Details View that shows all the information
available on an Asset. Apart from viewing, it also lets you perform CRUD
operations on a stored Asset (CI).

An Asset in our system has many properties and components; all of them
can be viewed on the Details View of an Asset. The available fields in
Details View depends on the Asset Type; for example, the Details View of a
Desktop has more fields compared to a SNMP device.

Details View lets you create maps that tell you about the relations an
Asset has with other CIs (Configuration Items).

To Access the Asset Details View:

1. Go to the :doc:`Asset List View<asset-list-view>` of any class.

2. Clicking on the ID or Name of an Asset from the list area takes you
   to the Asset Details View of the Asset.

.. _amf-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-14.png
    :align: center
    :alt: figure 14

Understanding the Details View is the first step towards managing a
single Asset in Flotomate.

-  Section-A houses the :ref:`Change Name and Description of an Asset<change-name-description-asset>`.

-  Section B & C houses the :ref:`classifiers <classifying assets>`.

-  Section-D showcases Properties, Components, Details and other
   information. Visibility of a tab depends upon the Asset Type.

    a. **Properties**: These are general information about the Asset.
       Properties do not contain information traceable to an individual
       component of an Asset; for example, OS version is identified with
       an Asset, whereas a 2 GB DDR3 RAM is a component level information
       and part of an Asset.

       The Properties are auto-populated during discovery, but you can
       edit the information. You can add Properties that haven’t been
       added by the Probe. In case, you are adding an Asset manually you
       have to add all the Properties.

        .. _amf-15:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-15.png
            :align: center
            :alt: figure 15

        There are four categories of Properties in Flotomate:

            i.  Computer Properties

            ii.   Hardware

            iii.  Software

            iv. Cloud

    b. **Hardware**: Some IT Assets are made up of hardware and software
       components. The Hardware tab lists all information on individual
       components of those Assets. The information may come from Discovery
       or Manual addition.

    c. **Software**: The Software tab lists all information on all
       individual Software in Assets that are made up of Hardware and
       Software components. You can add new Software and edit existing
       information. Discovered Assets have this section auto-populated by
       the Probe.

    d. **Details**: The Details tab contains information on a Software Asset
       concerning cost, validity, and license.

    e. **Consolidated Software**: Learn more about :doc:`Software Consolidation <consolidating-software>`.

    f. **History**: The History Tab of an Asset shows the following:

        i. :ref:`Audit Trail <am-viewing-audit-trail>`

        ii. :doc:`Scan and Change log. <asset-logs>`

    g. **Relationships**: Learn about :doc:`Managing Relationships <prohibited-software>`.

    h. **Linked Events**: Learn about :ref:`Linked Events <am-linked-events>`.   

    i. **Installation**: The Installation tab of a Software lists all the
       machines using the Software or have it installed.

    j. **Metering**: Learn about :doc:`Software Metering <software-metering>`.

    k. **Notes**: Technicians can add notes in an Asset. Notes are visible to all Technicians
       who are allowed to view the CMDB. :ref:`Learn more <adding notes>`.

    l. **Agent Information**: Assets that have been discovered via an Agent have this tab. The tab shows
       important information about he Agent, for example Agent ID.

-  Section-E is the Display Pane where all the Properties, Components,
   relationships, editing options, adding options and other information
   are visible.

-  Section-F shows the unique Barcode of an Asset. If there’s no
   Barcode, you can generate a new Barcode by clicking on **Add
   Barcode** and then **Generate New Barcode**. By clicking on an
   existing Barcode, you can perform the following operations:

   a. View Barcode

   b. :ref:`Print Barcode <print asset barcode>`

   c. :ref:`Copy Barcode <copying an asset barcode to the clipboard>`

   d. :ref:`Change Barcode <changing an assets barcode>`.

-  Section-G is the Action Menu of the Details View. The available
   options in this menu depend on the Asset Type. Some of the Options are:

   a. Add Attachments (available in all Asset Class).

   b. Scan Now (Only in Hardware Assets).

   c. Exclude from Scanning (Only in Hardware Assets).

   d. View Audit Trail (available in all Asset Class).

   e. Export Asset (available in Hardware and Software).

   f. Remote Desktop (only in Hardware Assets).

   g. Reconcile (only in Hardware Assets).

   h. Mark for Notification (only in Software Assets).

   
.. _change-name-description-asset:

Change (Host) Name and Description of an Asset
=======================================

Section-A (:numref:`amf-14`) shows the ID and Name (by default host name in case of Hardware Asset) of the Asset. The ID
Uniquely identifies an Asset whereas the Name is a human readable Asset
identifier. You can change the Display Name, HostName (in case of a Hardware Asset) and Description of the Asset using
the Edit Icon.

.. _amf-16:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-16.png
    :align: center
    :alt: figure 16

.. _amf-17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-17.png
    :align: center
    :alt: figure 17

Classifying Assets
==================

You can classify an Asset using predefined and custom identifiers. Go to
the :doc:`Details View <manage-asset-details>` of any Asset, and you would
have the following classifying options.

.. _amf-18.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-18.1.png
    :align: center
    :alt: figure 18.1

.. _amf-18.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-18.2.png
    :align: center
    :alt: figure 18.2

-  **Asset Type**: It is the primary form of classification of an Asset.
   All Asset Types are part of the Asset Type Hierarchy. Based on the
   Asset Type, property fields of an Asset are set. You can manually
   modify Asset Type of any Asset.

.. _amf-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-19.png
    :align: center
    :alt: figure 19

-  **Status**: You can classify an Asset based on usability by using the
   following statuses:

    .. _amf-20:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-20.png
        :align: center
        :alt: figure 20

    a. **In Use**: This means that the Asset is in use.

    b. **Missing**: The Asset had been purchased and used, but the location
       of the Asset is unknown now.

    c. **Retired**: The Asset is no longer in use.

    d. **In stock**: The Asset has been purchased but not in use.

    e. **In Transit**: The Asset has been purchased and in transit.

   You can have custom statuses. Learn more about :ref:`custom status <ad-add-custom-status>`.

-  **Discover status** (:numref:`amf-18.2`): The system classifies all discovered
   Assets with the label **Discovered**. The Assets that are manually
   created have the **Manually Created** label.

-  **IP Address** (:numref:`amf-18.2`): You can set IP address of a manually
   added Asset.

-  **Hostname**: You can set Hostname of a manually added Asset.

-  **Tags** (:numref:`amf-18.2`): It is a convenient way to classify an Asset by
   Technicians when existing options are not enough.

-  **Impact** (:numref:`amf-18.2`): It lets Technicians to define the impact of
   the Asset as either low, on self, department or business.

-  **Used By** (:numref:`amf-18.2`): Here a Technician can add the email of the
   user of the Asset from the Requester list.

-  **Business Service** (:numref:`amf-18.2`): You can associate the Asset with a
   predefined Business Service.

-  **Department** (:numref:`amf-18.2`): You can associate the Asset with a
   particular department by setting this field.

-  **Location** (:numref:`amf-18.2`): You can associate the Asset with a
   particular location by setting this field.

-  **Managed By** (:numref:`amf-18.2`): You can add the email address of the
   Technician who is responsible for the Asset from Technician list.

Add/Modify Asset Group:
-----------------------

Asset Groups help you to categorize an Asset. You can add an Asset Group
to an Asset or modify an existing one. By clicking on the Asset Group
field (:numref:`amf-18.2`) opens a drop-down menu where you make your selection.

.. _amf-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-21.png
    :align: center
    :alt: figure 21

Asset Groups are important for adding
:ref:`subscribers <managing subscribers>` to Hardware Asset related
:ref:`notifications <different types of notifications>`. Learn more about Asset Group.

Add/Modify Product
------------------

Every Asset in the CMDB is an instance of a Product. Having a Product
unlocks additional functionalities. You can add/modify the Product field
of all Assets (:numref:`amf-18.2`)). By clicking on the Product field you get
access to all available Products to choose from.

Add/Modify Vendor
-----------------

You can add/modify the Vendor field (:numref:`amf-18.2`) of any Asset from a
predefined list.

Asset Attachments
=================

You can add attachments to an Asset. The attachment can be anything
below 5 MB size.

Adding an Attachment
--------------------

Go to the :doc:`Asset Details View <manage-asset-details>` of the Asset to
which you want to add an attachment.

.. _amf-22:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-22.png
    :align: center
    :alt: figure 22

Click on the Action Menu of the Asset, and then select **Add
Attachment**.

You are asked to select the location of the file. Specify the
location and upload the file.

Viewing the Attachments
-----------------------

In the Details View, you can view the attachment/attachments of the
Asset in the More Details section.

.. _amf-23:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-23.png
    :align: center
    :alt: figure 23

.. _am-linked-events:

Linked Events
=============

The **Linked Events** tab gives you an option to create a link between
an Asset and other Requests, Problems, Knowledge and Changes. Learn to
access the :ref:`Linked Events <manage-asset-details>` tab.

The purpose of creating links is to build contextual information about
an Asset; for example, a faulty cooling system in a server (CI) have
generated incidents that lead to the identification of the Problem. If
the events have been linked with the Asset (server) then Technicians can
drill down to the root cause (faulty cooling system) by understanding
the context.

.. _amf-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-24.png
    :align: center
    :alt: figure 24

-  You can view the present links of an Asset from the Item list (lift
   side of the pane). You can filter for Problems, Changes, Requests and
   KB posts.

-  You can create a new Request, Problem, or Change and link it to an
   existing Asset using the **Create and Relate** option. Using this
   option, you can directly access the create dialog box of Requests,
   Changes, and Problems.

-  The **Add Relation** option lets you add one or more links to
   existing Requests, Problems, and Changes.

    .. _amf-25:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-25.png
        :align: center
        :alt: figure 25

    a. Clicking on **Add Relation** shows you a menu where you have to
       select either Request, Problem, or Change.

    b. A dialog box opens with a search bar. The search bar supports Advance
       Search.

    c. Search for the right entry and click **Link** to create a linkage
       with the Asset.

-  You can view all your linked events, and you can unlink them anytime
   you want.

.. _amf-26:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-26.png
    :align: center
    :alt: figure 26

Adding Notes
============

Notes are a brief record of points or ideas written down as an aid to memory. 
Technicians can record brief information in an Asset. One use case of this feature is that a technician can mention
a possible fault in an Asset via a Note; other Technicians can view the note before working with the Asset.

**To add a Note:**

- Go to the :doc:`Details View <manage-asset-details>` of the Asset where you want to add a Note.

- Click on the Note tab.

.. _amf-26.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-26.1.png
    :align: center
    :alt: figure 26.1

- Click on Add Note to add a new note. A new dialog box opens.

.. _amf-26.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-26.2.png
    :align: center
    :alt: figure 26.2

- Write a name and description and then click on **Add**.


Relationships
=============

You can create an exciting topology of Assets showing the nature of
their relationship with one another. Currently, only Hardware, Services,
Cloud, and Other Asset Types have the **Relationship** tab.

While creating a topology, the Assets are shown as nodes on a map. You
start with a single node, the Asset whose **Relationship** tab you are
using; then you add relationships; with each addition a new node is
created. The relationship between two nodes can be of two types:
**Direct** and **Indirect**.

The relationships created between nodes (Assets) are saved in the system
and can be viewed in their respective **Relationship** tabs. However,
such relationships have no bearing on the CMDB.

You can access the **Relationship** tab from the :ref:`Details
View <manage-asset-details>` of a Non-Software Asset.

.. _amf-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-27.png
    :align: center
    :alt: figure 27

-  You can zoom in & out using your scroll wheel while placing the
   pointer on the View Area.

-  You have to use the Create a Relationship dialog box to create a
   relationship between two nodes. Click on a node to open the Create a
   Relationship dialog box, or you could click on **Create a
   Relationship** button while keeping a node selected.

    .. _amf-28:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-28.png
        :align: center
        :alt: figure 28

    .. note:: Please refer to* :numref:`amf-28`.

    a. The relationship operation happens between two nodes at a time.
       Section-A shows the name of the first node (Asset), and the second
       node you have to select.

    b. Section-B lets you select the Relationship Type and Relationship
       Direct Type.

        i.  Relationship Types are two: Direct and Inverse. The two types
            represent two directions of a relationship.

        ii. Relationship Direct Type describes the nature of a relationship
            from a predefined list. There are two lists; one for the Direct
            and other for Inverse.

        **Example of a direct relationship:**

        A PC is dependent on a Server is a Direct relationship. We
        select **Depends On** from the Relation Direct Type List.

        .. _amf-29:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-29.png
            :align: center
            :alt: figure 29

        In :numref:`amf-29`, the arrow shows the direction of the dependency.

        **Example of an Inverse relationship:**

        A server receives data from a PC is an inverse relationship. We select
        **Received Data from** from the Relation Direct Type List in this case.

        .. _amf-30:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-30.png
            :align: center
            :alt: figure 30

    c. Section-C has the search bar for searching Assets in the CMDB. It
       supports the Advanced Search (refer the search bar of :doc:`List
       View <asset-list-view>`) feature.

    d. In section-D, you can view all the Assets or the list of Assets
       filtered by search. Here you make the selection for the second node.
       You can make only one selection.

   After making the selections in the Create a Relationship dialog box,
   clicking on **Create** makes the new relationship visible on the View
   Area.

-  The **View Relationship** button lets you view all the relationships
   in a list form of the node whose Relationship tab you are viewing.
   Here you can delete a relationship using the Delete Icon.

.. _amf-31:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-31.png
    :align: center
    :alt: figure 31

-  The **View Full-Screen** button expands the View Area to the entire
   page.

Reconciliation of Assets
========================

When new Assets are purchased and received, the related :doc:`Purchase Order <introduction-purchase-management>` is closed. The Assets that are received are automatically added to the
CMDB with the status **In Stock**. 

When these Assets are discovered during an Asset Scanning (could be Agent-less or Agent Based), duplicate entires are
created in the CMDB. A Technician has to manually reconcile each Asset with an **In Stock ** Asset. Reconciliation facilitates proper
inventory management where a Technician knows exactly which Assets are available for assignment.  

Only two Assets can be reconciled at a time.

Conditions for Asset Reconciliation:

- Only two Assets can be reconciled at a time.

- Any one of them has to have an Origin: Purchase Order.

What happens after Reconciliation of two Assets ?

- The Asset with Origin: Purchase Order is deleted.

- The Asset that is not deleted gets the following information added from the deleted Asset:

  a. Product info.

  b. Purchase Order details.

  c. The associated Purchase Order is linked (Relation) with the Asset.

  d. Used By and Manage By fields are updated, if any.

Learn how to perform :ref:`Asset Reconciliation <Manual Reconciliation of Assets>`.  
