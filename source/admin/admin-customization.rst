*************
Customization
*************

.. _ad-status

Status 
======

Status show the stage of a Request, Problem, Change and an Asset in
their respective process flow. Statuses are essential in managing the
life-cycle of tickets and CIs in the Flotomate. A lot of automatic
processes can be created based on the Status of a ticket.

We have predefined Statuses for each of the ticket types and Assets.
Along with pre-defined Statuses, you can add custom Statuses.

.. note:: Setting Custom Status requires administrative rights.

.. _adf-85.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-85.1.png
    :align: center
    :alt: figure 85.1

.. _adf-85.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-85.2.png
    :align: center
    :alt: figure 85.2


Predefined Status 
-----------------

Flotomate has predefined Statuses which are immutable. They coexist with
custom Statuses. They are as follows:

-  **Request**:

   Here Statuses show the life-cycle of a Request.

   a. Open

   b. Pending On Requestor

   c. Pending in Approval

   d. Pending On Technician

   e. Resolved

   f. Closed

-  **Problem**:

   Here Statuses show the life-cycle of a Request.

   a. Open

   b. Pending On Requestor

   c. Pending in Approval

   d. Pending On Technician

   e. Resolved

   f. Closed

-  **Change**:

   Here each status is part of a stage in a Change process.

   a. Submitted:

      i. Requested

      ii.  Rejected

      iii. Accepted

   b. Planning:

      i.  In Progress

      ii. Canceled

      ii. Completed

   c. Approval:

      i. Pending

      ii. Rejected

      iii. Approved

   d. Implementation:

      i. In Progress

      ii. Rejected

      iii. Completed

   e. In Review:

      i. In Progress

      ii. Failed

      iii. Completed

-  **Asset**:

   Here statuses reflect the state of an Asset.

   a. In Use

   b. Missing

   c. Retired

.. _ad-add-custom-status:

Add Custom Status 
-----------------

-  Go to **Admin** >> **(Request, Problem, Change or Asset) Custom
   Status**.

.. _adf-86:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-86.png
    :align: center
    :alt: figure 86

-  Select a Status Type.

.. _adf-87:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-87.png
    :align: center
    :alt: figure 87

-  Use the Plus Icon to add a custom Status. You can add multiple
   Statuses.

.. _adf-88:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-88.png
    :align: center
    :alt: figure 88

Rearrange Custom Status 
-----------------------

-  Go to the **Custom Status** page.

-  You can change the order of custom Statuses in all type by drag and
   drop.

.. _adf-89:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-89.png
    :align: center
    :alt: figure 89

Business Services in Problem Management
=======================================

Flotomate allows you to add a list of business deliverables (services)
of your organization. You can describe each and every business service
that you add.

In the product, a Technician can highlight the impact of a Problem by
associating it with a Business Service.

.. note:: Managing Business Services requires administrative rights.

**View Business Services**

-  Go to **Admin** >> **Business Services** (Problem Management).

-  In the **Business Services** page, you can view all your existing
   business service descriptions, if any.

.. _adf-90:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-90.png
    :align: center
    :alt: figure 90

Add Business Services
---------------------

-  Go to the **Business Services** page.

-  Click **Add Business Service** button situated in the top right
   corner of the page.

.. _adf-91:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-91.png
    :align: center
    :alt: figure 91

-  Fill the Name and Description fields and click on **Add**.

-  In the **Business Services** page, you can edit any business
   description using the Edit Icon or delete using the Delete icon.

.. _adf-92:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-92.png
    :align: center
    :alt: figure 92

.. _ad-templates:

Templates
=========

Templates in Flotomate allows you to quickly fill the create form of
Request, Problem, and Change. You can create templates for each of the
ticket types, and your users (only on Technician portal) can use them while creating a Request,
Problem or Change.

.. note:: Managing templates requires administrative rights.

Add a Template
--------------

-  Go to **Admin** >> (Request, Problem or Change) Templates.

.. _adf-93:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-93.png
    :align: center
    :alt: figure 93

-  In the new page, you can view your existing templates. To add a new
   one, click on **Create a (Request, Problem, or Change) Template** in
   the top right corner.

-  A dialog box opens where you can pre-define the following things:

   a. **Request**:

        .. _adf-94:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.png
            :align: center
            :alt: figure 94

       i.  The subject of a Request.

       ii. Urgency, and Impact of a Request.

       iii. Tags of a Request.

       iv.  Category of a Request.

       v.   Requestor Accounts.

       vi.  Description of a Request.

   b. **Problem**:
        .. _adf-94.1:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.1.png
            :align: center
            :alt: figure 94.1

       i.  Subject to a Problem

       ii.  Whether a Problem is known or not.

       iii.  Priority, Urgency, Nature of Problem and Impact of a Problem.

       iv. Tags of a Problem.

       v.  Mark the Problem as a known error.

       vi.  Category of a Problem.

       vii.  Description of a Problem.

   c. **Change**:

        .. _adf-94.2:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.2.png
            :align: center
            :alt: figure 94.2

       i.  The subject of a Change.

       ii.  Priority, Urgency, Risk, Change Type and Impact of a Change.

       iii.  Tags of a Change.

       iv.  Category of a Change.

       v.  Description of a Change.

Edit Request Templates
----------------------

-  Go to **(Request, Problem or Change) Templates** page

-  Click the Edit-Icon adjacent to a template to open a dialog box.

-  Make your changes and hit **Update**. You are taken back to the
   **Templates** page

-  Delete any template using the Delete Icon next to the Edit Icon.

.. _ad-response-template:

Response Template
=================

While handling Requests, Technicians have to do a lot of repetitive work. We have isolated two such work: asking Requestors and 
giving a Solution. You can now create templates to deliver canned response and solution to Requestors having similar problems.
You can create n number of templates and access them directly from Ask Requestor and Solution input box in a Request.

**To Create a Template:**

- Go to **Admin** (A Navigation Tab) >> **Response Template** (under Request Management).

.. _adf-94.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.1.png
    :align: center
    :alt: figure 94.1
 
- The Response Templates page opens. Here you can view all your existing templates. Click on **Create Response Template**
  situated in the top right corner of the page.

- A new page opens where you get the following fields:

    .. _adf-94.2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.2.png
        :align: center
        :alt: figure 94.2

    a. Section A (:numref:`adf-94.2`) is where you give a name to the template.

    b. In section B, you decide where the template will be used. It can either be used while asking Requestors or giving a solution to
       a Request.

    c. There is a toggle button to turn on/off the template in section C.

    d. Section D is the text area to add your response.

    e. While writing your response , you can add placeholders from a predefined list which you can access from Section E.
       Placeholders can fetch specific data; for example, the placeholder {#Ticket Id#} fetches the ticket id of the Request 
       on which you are working.

    .. _adf-94.5:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.5.png
        :align: center
        :alt: figure 94.5   

  Fill all necessary fields and click on **Create**. Your template is added to the Response Template page. 

.. _adf-94.6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.6.png
    :align: center
    :alt: figure 94.6

**Using the templates**

You can access the response templates while working on a Request. You can directly add a template while asking a Requestor and
adding a solution.

.. _adf-94.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.3.png
    :align: center
    :alt: figure 94.3

.. _adf-94.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.4.png
    :align: center
    :alt: figure 94.4        

.. _ad-custom-fields:

Custom Fields
=============

Custom fields are additional fields added by a user. They can appear
while creating a ticket, and in the details view of a ticket and CI.
Custom fields can be added to Requests, Problems, Changes, and Assets.

.. note:: Adding Custom Fields requires administrative rights.

Add a Custom Field
------------------

-  Go to **Admin** >> **(Request, Problem, Change or Asset) Custom
   Fields**.

.. _adf-95:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-95.png
    :align: center
    :alt: figure 95

-  In the **Custom Fields** page, you can view your existing custom
   fields for each module, if any.

.. _adf-96:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-96.png
    :align: center
    :alt: figure 96

-  Regardless of the module, you can only have two types of fields: Text
   Field and Selection Field. A Text field has a label and an input area
   for a value, and a Selection Field has a label and an input area
   with a drop-down list of values.

   Anywhere, you can have both Text-Field and Selection-Field. You start
   adding fields using the **Add** button.

    +-----------------------------------+------------------------------------------+
    | Text Field                        | -  Field Label is the name of the        |
    |                                   |    field and appears above the           |
    |                                   |    field.                                |
    |                                   |                                          |
    |                                   | -  Default Value always appears          |
    |                                   |    in the field before being             |
    |                                   |    edited.                               |
    |                                   |                                          |
    |                                   |    .. _adf-97:                           |
    |                                   |    .. figure:: https://bit.ly/2t1fs3u    |
    |                                   |        :align: center                    |     
    |                                   |        :alt: figure 97                   |  
    |                                   |                                          |        
    |                                   |                                          |
    +-----------------------------------+------------------------------------------+
    | Selection Field                   | -  You can have one Field Label          |
    |                                   |    but multiple options.                 |
    |                                   |                                          |
    |                                   | -  Use the Plus Icon to add more         |
    |                                   |    options                               |
    |                                   |                                          |
    |                                   | -  The options are shown as a            |
    |                                   |    list.                                 |
    |                                   |                                          |
    |                                   | -  You can select an option to be        |
    |                                   |    the default value. Default            |
    |                                   |    Value always appears in the           |
    |                                   |    field before being edited.            |
    |                                   |                                          |
    |                                   | -  You can change the Default            |
    |                                   |    Values’.                              |
    |                                   |                                          |
    |                                   |     .. _adf-98:                          |
    |                                   |     .. figure:: https://bit.ly/2JBPyOI   | 
    |                                   |        :align: center                    |
    |                                   |        :alt: figure 98                   |  
    +-----------------------------------+------------------------------------------+

-  The behavior and outlook of custom fields change across the module types.

    a. **Request**:

      i. You can show a custom field in **Create a Request** form.

            .. _adf-99:
            .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-99.png
                :align: center
                :alt: figure 99

         For example, we have created a field called Employee ID in :numref:`adf-99`.

      ii. New fields appear in the Work tab of a Request.

        .. _adf-100:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-100.png
            :align: center
            :alt: figure 100

      iii. You can make a field compulsory for certain Statuses. For
           example, if a field is compulsory in Open Status, then you cannot
           keep the field empty when changing to another Status.

    b. **Problem**:

      i. All custom fields appear in the **Custom Fields** tab under
         **Analysis**.

        .. _adf-101:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-101.png
            :align: center
            :alt: figure 101

      ii. You can make a field compulsory for certain Statuses. For example,
          if a field is compulsory in Open Status, then you cannot keep the
          field empty when changing to another Status

    c. **Change**:

      i. You can add a field to a particular stage of a Change.

        .. _adf-102:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-102.png
            :align: center
            :alt: figure 102

      ii.  You can mark a field as compulsory at a particular stage.

      iii. Fields appear in a separate section called Custom Fields.

        .. _adf-103:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.png
            :align: center
            :alt: figure 103

    d. **Asset**:

      i. You add a field either to an Asset Type or a particular
         sub-type.

      ii. Within a type, you can either make the field appear in Property
          section or Component section. Please refer to the Asset
          Management manual to learn more.

    e. **Requestor**
       
       i. Here Custom fields allow you to create new variables to store information about requestors.

       ii. You can create n number of text fields.

        .. _adf-103.1:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.1.png
            :align: center
            :alt: figure 103.1
        
       iii. Such fields appear on the :ref:`form for creating <add-requestor-individually>` Requestors.

        .. _adf-103.2:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.2.png
            :align: center
            :alt: figure 103.2

       iv. Custom fields appear while mapping field names during LDAP Configurations.

        .. _adf-103.3:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.3.png
             :align: center
             :alt: figure 103.3

       v. Custom fields are considered when mapping columns during CSV import of Requestors.

        .. _adf-103.4:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.4.png
             :align: center
             :alt: figure 103.4              

Edit Custom Fields
------------------

-  Go to the :ref:`Custom Fields <add-a-custom-field>` page.

-  .You can change the name of a custom field using the Edit Icon or
   delete it using the Delete Icon.

.. _adf-104:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-104.png
    :align: center
    :alt: figure 104

.. _ad-category:

Category
========

The category is one of many categorization features we have. You can use
category for delegation, workflow design, or any other categorization
function required by your organization. You can have Categories for
Request, Problem, Change, Project, and Software.

Predefined categories
---------------------

Flotomate comes pre-loaded with the following Categories:

+-----------------------------------+-----------------------------------+
| **Request**                       | -  Service Request                |
|                                   |                                   |
|                                   | -  Incident                       |
|                                   |                                   |
|                                   | You can change the name of the    |
|                                   | above categories but not the      |
|                                   | Category Key.                     |
+-----------------------------------+-----------------------------------+
| **Problem**                       | -  General                        |
|                                   |                                   |
|                                   | -  Hardware                       |
|                                   |                                   |
|                                   | -  Software                       |
|                                   |                                   |
|                                   | -  Network                        |
|                                   |                                   |
|                                   | -  IT Administration              |
|                                   |                                   |
|                                   | You can change the name of the    |
|                                   | above Categories.                 |
+-----------------------------------+-----------------------------------+
| **Change**                        | -  General                        |
|                                   |                                   |
|                                   | -  Process                        |
|                                   |                                   |
|                                   | -  Hardware                       |
|                                   |                                   |
|                                   | -  Software                       |
|                                   |                                   |
|                                   | -  Network                        |
|                                   |                                   |
|                                   | -  Security                       |
|                                   |                                   |
|                                   | You can change the name of the    |
|                                   | above Categories.                 |
+-----------------------------------+-----------------------------------+
| **Project**                       | -  Business                       |
|                                   |                                   |
|                                   | -  Maintenance                    |
|                                   |                                   |
|                                   | -  Infrastructure                 |
|                                   |                                   |
|                                   | -  Research                       |
|                                   |                                   |
|                                   | You can change the name of the    |
|                                   | above Categories.                 |
+-----------------------------------+-----------------------------------+
| **Software**                      | -  A/C                            |
|                                   |                                   |
|                                   | -  DB                             |
|                                   |                                   |
|                                   | -  Development                    |
|                                   |                                   |
|                                   | -  Game                           |
|                                   |                                   |
|                                   | -  Graphics                       |
|                                   |                                   |
|                                   | -  Internet                       |
|                                   |                                   |
|                                   | -  Multi-Media                    |
|                                   |                                   |
|                                   | -  Operating System               |
|                                   |                                   |
|                                   | -  Others.                        |
|                                   |                                   |
|                                   | You can modify or delete the      |
|                                   | above categories.                 |
+-----------------------------------+-----------------------------------+

Add a Category
--------------

.. note:: Adding a category requires you to have access to the Admin section.

-  Go to **Admin** >> **(Request, Problem, Change, Project or
   Software)** **Categories**.

.. _adf-105:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-105.png
    :align: center
    :alt: figure 105

-  In Request, Problem, Change, and Project, you can add a Category and
   its Sub-Categories up to level three. In Software, you can have only
   standalone Categories.

-  In the leftmost column, you can add a level one Category using the
   **Add** button. Clicking on a Category activates its right side
   Sub-Category column where you can add another Category.

-  In Request, you are asked for a Category Key when adding a new
   Category. This is used as a prefix to the ID of a Request.

.. _adf-106:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-106.png
    :align: center
    :alt: figure 106

Edit Category
-------------

-  Go to **Categories** page\ **.**

-  You can change the name of a Category using the Edit icon.

.. _adf-107:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-107.png
    :align: center
    :alt: figure 107

-  You can only delete Categories in Software. In other types, you have
   to turn a Category off.

.. _ad-custom-rule:

Custom Rules
============

Using Custom Rules, you can set pre-requisites that need to be done
before performing certain actions. You can have Custom Rules for
Request, Problem, Change, Knowledge and Remote Deployment.

To Open Custom Rules:

-  Go to **Admin** >> **(Request, Problem, Change, Knowledge or Patch)
   Custom Rules**.

.. _adf-108.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-108.1.png
    :align: center
    :alt: figure 108.1

.. _adf-108.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-108.2.png
    :align: center
    :alt: figure 108.2

Current Custom Rules are as follows:

Request
-------

-  **Before resolving a Request**:

   a. User Interaction:

      i.   Should have at least one message in Ask Requestor tab.

      ii.  A Request should have at least one note.

      iii. Should have at least one solution.

   b. Mandatory fields:

      i. Should have an assigned Technician.

      ii.   Should have a Location.

      iii.    Should have an Estimated Time.

      iv.   Should have a Diagnosis.

      v.  Should have a Source.

      vi. Should have Approval status as either Approved or Pre-Approved.

   c. Should have all Tasks as closed.

-  **Before closing a Request**:

   a. Same as before resolving a Request.

   b. Should not skip Resolve status.

-  **Required to add a Note before**:

   a. Should add a Note to a Request before performing the following
      actions:

      i.   Changing assigned Technician of a Request.

      ii.    Changing Support Level of a Request.

      iii.   Changing Due Date of a Request.

      iv.  Changing Category of a Request.

      v. Changing Department of a Request.

      vi.   Changing Priority of a Request.

Problem
-------

-  **Before resolving a Request**:

   a. User Interaction:

      i.  A Request should have at least one note.

      ii. Should have at least one solution.

   b. Mandatory fields:

      i.  Should have an assigned Technician.

      ii. Should have a Location.

      iii.  Should have a Root Cause.

      iv.   Should have a Symptom.

      v.  Should have an Impact.

      vi. Should have Approval status as either Approved or Pre-Approved.

   c. Should have all Tasks as closed.

-  **Before closing a Request**:

   a. Same as before resolving a Request.

   b. Should not skip Resolve status.

-  **Required to add a Note before**:

   a. Should add a Note before performing the following actions:

      i. Changing assigned Technician.

      ii.   Changing Due Date.

      iii.    Changing Category.

      iv.   Changing Department.

Change
------

You can set rules for each stage of a change process.

-  **Submit**:

   a. Should have a Change Manager.

   b. Should have an assigned Technician.

   c. Should have a Location.

-  **Planning**:

   a. Should have schedule and rollout dates.

   b. Should have a rollout plan.

   c. Should have an assigned Technician.

   d. Should have set impact.

   e. Should have a Backout plan.

-  **Implementation**:

   a. Should have a change implementer.

   b. All task must be closed before moving to the next stage.

   c. Should have an assigned Technician.

-  **In Review:**

   a. Should have a change reviewer.

   b. Should have an assigned Technician.

-  **Require Note befor**\ e:

   a. Changing category.

   b. Changing assigned Technician.

   c. Changing Department.

   d. Changing Location.

Asset
-----

-  Manual Update:

   .. note:: Asset rules are applicable for both discovered and manually created Assets.

   a. Whether to allow Technicians to update Hardware Components of an
      Asset.

   b. Whether to allow Technicians to update Software Components of an
      Asset.

   c. Whether to allow Technicians to update Users details of an Asset.

Knowledge
---------

Whether Knowledge should be approved by approvers before publishing.

Remote Deployment:
------------------

Whether a deployment of Patches and Packages needs to go through an
Approval process.