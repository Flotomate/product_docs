.. _ad-custom-fields:

*************
Custom Fields
*************

When creating a ticket or CI (Configurable Item), our system captures certain data.
Apart from the default types, we give users the flexibility to capture custom data types using the 
custom field feature. For example, some of our product users are capturing employee id using a custom field. 

Custom fields are additional fields added by a user. They can appear
while creating a ticket, and in the details view of a ticket and CI.
Custom fields can be added to Requests, Problems, Changes, Contract, Feedback, Purchase, Project and Assets.

.. note:: Adding Custom Fields requires administrative rights.

.. _ad-types-of-fields:

Types of Fields
===============

We have four field types and one formatting option which you can use. The fields support a host of input types. Using the
formatting option you can build interesting forms. The various options are as follows:

- **Text Field**: This is a basic field that allows users to input a small amount of text. Supported value types   
  are: Text, Number and Date.

.. _adf-94.5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.5.png
    :align: center
    :alt: figure 94.5 

- **Dropdown**: This field is populated from a predefined list. You get the option to defined the list.

.. _adf-94.6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.6.png
    :align: center
    :alt: figure 94.6 

- **Section**: Adding a section allows you to group fields. You can group similar fields together and align them in split form
  inside the section.  

.. _adf-94.7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.7.png
    :align: center
    :alt: figure 94.7 

- **Checkbox**: It is a predefined checklist. You select by the checking the options. 

.. _adf-94.8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.8.png
    :align: center
    :alt: figure 94.8 

- **Radio Button**: Similar to checklist, but supports only one selection.

.. _adf-94.9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.9.png
    :align: center
    :alt: figure 94.9

- **Text Area-input**: It is a multi line text input area. 

.. _adf-94.9.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.9.1.png
    :align: center
    :alt: figure 94.9.1

- **Labels**: This are static, immutable chunks of text.

.. _adf-94.9.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.9.2.png
    :align: center
    :alt: figure 94.9.2

- **Attachment**: This field allows you to attache a file of size up to 5 MB. 

.. _adf-94.9.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.9.3.png
    :align: center
    :alt: figure 94.9.3

Working with Custom Fields
==========================

The product has a simple drag and drop UI to create and arrange fields. 

.. _ad-create-custom-fields:

create a custom field
---------------------

- Go to **Admin** >> **(Request, Problem, Change, Contract, Purchase, Feedback, Project or Asset) Custom Fields**.

.. note:: Each module has a separate custom fields page.

.. _adf-95:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-95.png
    :align: center
    :alt: figure 95

- In the **Custom Fields** page, you can view your existing custom
  fields, if any.

.. _adf-96:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-96.png
    :align: center
    :alt: figure 96

- To create a new field, drag and drop a field type from the Form Control section to the Preview section. 

.. _adf-97:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-97.png
    :align: center
    :alt: figure 97

- The field is immediately created, and you can edit the field in its Glance View. 
  You can open the Glance view by clicking on the field.

    .. _adf-98:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-98.png
        :align: center
        :alt: figure 98

  Depending on the field type you can edit the following things: 

  a. **Form Label**: This refers to the title of the field.

  b. **Input Type**: Available for Text Input field. This field supports three types of inputs: Text, Number and Date (Sat, Jul 21, 2018 4:39 PM).

  c. **Hint Text**: Available for Text Input and Drop-down. Hint text appears pre-filled in the input area; hinting the user what to
     input.  

  d. **Default Value**: Applicable in all field types. You can choose what value to be pre-selected or pre-filled by default.
     In case there are multiple options, you can select any one as the default value. 

    .. _adf-98.1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-98.1.png
        :align: center
        :alt: figure 98.1 

  e. **Add Option**: For Checkbox and Radio-button type fields, you can add n number of options.

    .. _adf-98.2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-98.2.png
        :align: center
        :alt: figure 98.2

  f. **Label value**: Refers to a static chunk of text which is immutable and available only in a Label field.        

Additional Custom Field Options
-------------------------------
Clicking on a field opens the glance view where you will get additional options depending on the field type and module selected. 

.. _ad-cus-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-1.png
    :align: center
    :alt: figure 1

1. **Required**: This option makes the field compulsory on a form.

2. **System Managed field**: This option makes the field uneditable, and the field will show only system generated values.

3. **Show on Requester form**: This option is only available in Request fields and allows to control what field to show on the 
   Requester form.

Rearrange Custom Field
----------------------

You can arrange the fields using drag and drop. You can group fields in to sections (this feature is available for Request, 
Requestor, Feedback, Purchase, Contract, Project and Problem custom fields), and
you can arrange custom fields in to a matrix using the section feature.

.. _adf-94.7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-94.7.png
    :align: center
    :alt: figure 94.7

.. note:: The rearrange feature doesn't work when a field is in edit mode (Glance View is open). 
          The fields are movable when the move icon is visible. 

.. _adf-98.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-98.4.png
    :align: center
    :alt: figure 98.4

You can delete a field using the adjacent trash icon.     

Custom Field Behavior
=====================

The behavior and outlook of custom fields is different for each module.

.. _custom-field-request:

Request
-------

Custom fields appear on the **Create a Request** form. The fields appear by default in the Technician portal, but you have
to specifically toggle an option to make them appear in the Customer portal.

.. _adf-98.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-98.3.png
    :align: center
    :alt: figure 98.3
            
.. _adf-99:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-99.png
    :align: center
    :alt: figure 99

You can view and edit custom fields from the :ref:`details view <request details view>` of a Request. You can find the fields
under the **Custom Fields** tab. 

.. _adf-100:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-100.png
     :align: center
     :alt: figure 100

You can make a field compulsory for certain Statuses. For example, if a field is compulsory in Open Status, then you cannot
keep the field empty when changing to another Status.

.. _adf-100.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-100.1.png
     :align: center
     :alt: figure 100.1    
    
You can make a field as system field, which shows only system generated value. Such fields are not editable from the user interface.

.. _ad-cus-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-3.png
    :align: center
    :alt: figure 3

You can control the visibility of some default fields on the (Requestor Form) Customer portal; they are:

.. _adf-100.1.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-100.1.1.png
     :align: center
     :alt: figure 100.1.1

Custom fields in Request also appear in the :ref:`Report module<create-tabular-report>`. Technicians can use custom fields in generating reports. 

.. _adf-100.1.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-100.1.2.png
     :align: center
     :alt: figure 100.1.2

Custom fields in Request appear as part of the Workflow conditions.

.. _ad-cus-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-2.png
    :align: center
    :alt: figure 2

Problem
-------

Problem custom fields are available to Technicians on the **Create a Problem** page.

.. _adf-100.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-100.2.png
     :align: center
     :alt: figure 100.2

Technicians can view and edit custom fields from the :ref:`details view <problem details view>` of a Problem. 
You can find the fields under the **Custom Fields** tab. 

.. _adf-101:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-101.png
        :align: center
        :alt: figure 101

You can make a field compulsory for certain Statuses. For example,
if a field is compulsory in Open Status, then you cannot keep the
field empty when changing to another Status. Please refer to the above :ref:`section <custom-field-request>`.

You can make a field as system field, which shows only system generated value. Such fields are not editable from the user interface.

.. _ad-cus-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-3.png
    :align: center
    :alt: figure 3

Custom fields in Problem also appear in the :ref:`Report module<create-tabular-report>` (as part of the column selection). 
Technicians can use custom fields in generating reports. 

Custom fields in Problem also appear as part of the Workflow conditions.

Change
------

Custom fields in the case of a Change, appears only in the :ref:`Details View <change details view>` under the **Custom Fields** tab.
While creating custom fields, you can specifically mark a field as belonging to a particular stage.

.. _adf-102:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-102.png
     :align: center
     :alt: figure 102

.. _adf-102.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-102.1.png
     :align: center
     :alt: figure 102.1

.. _adf-103:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.png
     :align: center
     :alt: figure 103

.. note:: Stage specific fields can be edited in their respective stages.     

You can mark a field as compulsory at a particular stage. You can even mark a field as a system field that only shows system 
generated data. 

.. _adf-102.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-102.2.png
     :align: center
     :alt: figure 102.2

You can make a field as system field, which shows only system generated value. Such fields are not editable from the user interface.

.. _ad-cus-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-3.png
    :align: center
    :alt: figure 3

Custom fields in Change also appear in the :ref:`Report module<create-tabular-report>` (as part of the column selection). 
Technicians can use custom fields in generating reports.     

Custom fields in Change also appear as part of the Workflow conditions.


Asset
-----

You add a custom field either to an Asset Type (all sub-types will have the field) or a particular sub-type (specific).

Within a type, you can either make the field appear in Property section or Component section. Please refer to the Asset
Management manual to :ref:`learn more <Asset Management>`.

.. _adf-102.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-102.3.png
     :align: center
     :alt: figure 102.3

.. _adf-102.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-102.4.png
     :align: center
     :alt: figure 102.4

.. _adf-102.5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-102.5.png
     :align: center
     :alt: figure 102.5

You can make a field as system field, which shows only system generated value. Such fields are not editable from the user interface.

.. _ad-cus-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-3.png
    :align: center
    :alt: figure 3

Custom fields in Asset also appear in the :ref:`Report module<create-tabular-report>` (as part of the column selection). 
Technicians can use custom fields in generating reports. Remember, custom fields are specific to an Asset Type and a sub-type.               

.. _requestor-custom-field:

User Custom Field
-----------------
       
Here Custom fields allow you to create new variables to store additional information about requestors.

You can create n number of text fields.

.. _adf-103.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.1.png
        :align: center
        :alt: figure 103.1
        
You can make a field as system field, which shows only system generated value. Such fields are not editable from the user interface.

.. _ad-cus-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-4.png
    :align: center
    :alt: figure 4

Such fields appear on the :ref:`form for creating <add requestor individually>` Requestors.

.. _adf-103.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.2.png
        :align: center
        :alt: figure 103.2

Requestor Custom fields also appear while mapping field names during LDAP Configurations.

.. _adf-103.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.3.png
        :align: center
        :alt: figure 103.3

Custom fields are considered when mapping columns during CSV import of Requestors.

.. _adf-103.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.4.png
        :align: center
        :alt: figure 103.4

Contract Custom Fields
----------------------

Users can add Custom Contract Fields in the Contract module. Some of the use cases of having custom fields are:

- Custom fields can be used for capturing additional information about a Contract.

- Custom fields appear in the :ref:`Reporting module<new-custom-report>`, where you can generate reports using custom fields.

- Custom fields are supported in CSV import of Contracts (as one of the header property values). Custom fields can be used to capture additional information during Contract
  :doc:`CSV import <upload-contracts-csv>`.

You can make a field as system field, which shows only system generated value. Such fields are not editable from the user interface.

.. _ad-cus-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/ad-custom-field/AD-CUS-5.png
    :align: center
    :alt: figure 5

You can view and edit values of such fields from the Custom Fields tab in the :ref:`contract details view` of a Contract.

.. _adf-103.5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.5.png
     :align: center
     :alt: figure 103.5

Feedback Form
-------------

A Feedback form captures the experience of a Requestor with the Helpdesk. A Feedback form is always specific to a particular
Request. Using Custom fields, administrators can add more fields to capture additional information. Values captured by custom fields 
are visible under the Feedback tab in the Details View of a Request.

Things to Remember:

- A Feedback form is specific to a particular Request.

- A link to the Feedback form is sent with the Resolved and Closure Email, and an Email sent manually.
  (:ref:`Learn More <To Activate Feedback>`).

.. note:: You can make a field as system field, which shows only system generated value. 
          Such fields are not editable from the user interface. :ref:`Learn more <Additional Custom Field Options>`.

The Actual Feedback Form:

.. _adf-103.6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.6.png
     :align: center
     :alt: figure 103.6

The information captured by a Feedback form is visible in the following places. 

.. _adf-103.7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.7.png
     :align: center
     :alt: figure 103.7

Purchase Custom Field
---------------------

Custom fields appear on the :ref:`Edit a PO page <Open Edit a Purchase Order Page>`.  Custom fields can be accessed from 
**Admin** >> **Purchase Custom Fields**.

.. _pur-50:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-50.png
    :align: center
    :alt: figure 50

There are two class of Purchase Custom Fields:

- **General Details**: This class of custom fields appear under the Additional Information section of :ref:`Edit a PO page <Open Edit a Purchase Order Page>`.
 
- **Purchase Items**: These are Text fields that support only numbers, and they either add or subtract to the Net Total price of a 
  Purchase Order (excluding or including shipping). 

Learn More about :ref:`Purchase Custom Fields`. 

Project Custom Field
--------------------

Custom fields appear under the **Custom Field** tab in the details view of a project.

.. _adf-103.8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-103.8.png
     :align: center
     :alt: figure 103.8

Vendor Custom Field
-------------------

Custom fields appear in the add vendor form.

.. _adf-152:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-152.png
     :align: center
     :alt: figure 152

Product Custom Field
--------------------

Custom field appear in the add product form. 

.. _adf-153:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-153.png
     :align: center
     :alt: figure 153