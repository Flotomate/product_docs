*********************
Working on a Contract
*********************

Once a Technician decides to work on a Contract, he heads to the Details
View of the Contract. There he/she uses the product features and
capabilities to manage the Contract.

Contract Details View
=====================

The Contract Details view organizes and manages all information related
to a Contract. Each Contract has its own Details View having features that
Technicians use to resolve a Contract.

**To open Contract Details View:**

- Go to :doc:`contract-list-view`.

- Click on the Contract (name) of which you want to see the Details View. It doesn't matter whether you are in Grid or Table View.

The Details View opens with the following fields:

.. _con-18:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-18.png
    :align: center
    :alt: figure 18

1. Section A is where you view the ID and Name of the Contract. Here you get the option to edit the Name and Description of the Contract.
   Related topic: :ref:`modify contract name and description`.

2. Section B is where you :ref:`classify a contract`. 

3. In section C, you get six tabs and the following options under them:

   a. :ref:`con-associate-assets`

   b. :ref:`Contract Renewal`
    
   c. :ref:`Child Contract`

   d. :ref:`custom contract Field` (visible when there are custom fields)

   e. :ref:`con-attachments`

   f. :ref:`con-notifications`

4. Section D houses the :ref:`Renew Contract Option <creating a renewal>`, :doc:`Assign Owner option <assigning-a-contract>` and 
   Action Menu. In the Action Menu we have the following options:

   a. :doc:`Cancel <cancelling-a-contract>`

   b. :ref:`Notify Settings`

   c. :ref:`Send Email <con-notifications>`

   d. :doc:`Print <printing-a-contract>`

   e. :doc:`View Audit Trail <contract-audit-trail>`

   f. :doc:`Delete a Contract <archive-and-delete>`           

Modify Contract Name and Description
====================================

The Contract module allows you to change the Name and Description of a Contract from its :ref:`contract details view`.

To Change the Name and Description:

- In the Details View of a Contract, click on the edit icon in section A of :numref:`con-18`. 

- A dialog opens where you can edit the Name and Description of the Contract.

.. _con-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-19.png
    :align: center
    :alt: figure 19

Classify a Contract
===================

There are many avenues to classify a Contract. You can manage all the classifications from the :ref:`contract details view`.
The system allows the following categories for classification:

- Status

- Contract Type.

- Vendor info.

- Duration of the Contract (Start and End date).

- Department

- Parent Contract

- Cost and Currency

.. _con-status:

Status
------

.. _con-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-20.png
    :align: center
    :alt: figure 20

Status shows the life-cycle of the Contract. There are four statuses, and they are set automatically by the system. 
The statuses are as follows:

- **Not Started**: Contracts that are yet reach their start date show this status.

- **Open**: Active Contracts show this status.

- **Expired**: Contracts that have reached or crossed their End date show this status.

- **Cancelled**: As the name suggests, cancelled Contracts show this status.

.. note:: You cannot change Status manually.

.. _con-contract-type:

Contract Type
-------------

A Contract Type shows the nature of relationship between two or more parties. Every Contract has a type, and we give four types
out of the box. You can add more types (Learn how to add more :doc:`contract-type`). Following are the pre-defined types:

- **Lease**: A lease is a contractual arrangement calling for the lessee to pay the lessor for use of an asset. Property, 
  buildings and vehicles are common assets that are leased. Industrial or business equipment is also leased (wikipedia). 

- **Warranty**: In contract law, a warranty has various meanings but generally means a guarantee or promise which provides assurance 
  by one party to the other party that specific facts or conditions are true or will happen (wikipedia).

- **Support**: A contractual obligation to provide support in the form of troubleshooting, maintenance, and Repair.  

- **Maintenance**: An agreement between parties covering the maintenance of an Asset/Assets over a specified period of time.

Vendor
------

A Vendor is an entity that offers something for sale. A Contract generally defines the terms and conditions between a buyer and seller
(Vendor). While adding a Contract you can directly associate a Vendor from the system Vendor list or add it later. Learn how to add a :ref:`ad-vendor`.

Duration
--------

A Contract is valid for a defined period. You can show the validity of a Contract using the Start and End fields (input: date and time) in the Details View
of a Contract.

.. _con-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-21.png
    :align: center
    :alt: figure 21

Department
----------

You can associate a Department with a Contract from the system Department list. Learn how to add :ref:`ad-departments`.

Parent Contract
---------------

A Contract can be a child of another Contract, also referred to as sub-contract. This field shows the name of the primary Contract
as a parent.

.. note:: An assigned owner can set this field.

.. _con-22:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-22.png
    :align: center
    :alt: figure 22

Cost and Currency
-----------------

You can record the associated cost with a Contract in the Details View. The cost can be recorded in a particular currency; 
you can access the system currency list from the field. Learn how to add a :ref:`pur-currency`.

.. _con-23:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-23.png
    :align: center
    :alt: figure 23

.. _con-associate-assets:    

Associate Assets
================

A Contract is generally created around an Asset/Assets, and it defines the obligation of the seller and duties of the buyer. A Contract can
have relationship with an Asset/Assets;

You can link an Asset/Assets with a Contract is the following way:

- Go to the :ref:`contract details view` of a Contract.

- You can find all existing association under the **Assets** tab. Here you have two options: create a new Asset and Relate (**Create and Relate**), and 
  relate a existing Asset (**Add Relation**) in the CMDB.

.. _con-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-24.png
    :align: center
    :alt: figure 24

- Clicking on **Click and Relate** >> **Asset** opens the Add Asset dialog box (:ref:`Learn More <Manually Creating an Asset in the CMDB>`). 
  Use this option when the associated Asset/Assets is/are not in the CMDB.    

- Clicking on **Add Relation** >> **Asset** opens the *Create a Relationship with Asset* dialog box, where you can search and associate multiple Assets. 

    .. _con-25:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-25.png
        :align: center
        :alt: figure 25

  You can add the following class of Assets:

  .. _con-26:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-26.png
        :align: center
        :alt: figure 26

  Based on the selected Asset class, the list area is populated. 

  The search bar supports the Advance Search feature where you can use search options and keywords to create a filter.
  Learn how to use the :ref:`search bar<am-using-search-bar>`.

- Once you are done selecting the Asset/Assets, click on **Associate**.

Contract Renewal
================

A Contract is time bound; it has a start date and end date. A Technician can extend this period by reissuing the Contract (with different date and time) which is
termed as Renewal. When a Contract is Renewed, the original Contract expires and a duplicate Contract is created with different start and
end time. 

Renewal date and time conditions
--------------------------------

The below table shows the conditions that you need to keep in mind when setting the date and time of a Contract renewal. 

+-------------------+-----------------------------------------------+-------------------------------------------+
|                   | Start Date&Time                               | End Date&Time                             |
+-------------------+-----------------------------------------------+-------------------------------------------+
| Original Contract | 13/07/2018/6:00 PM                            | 13/07/2019/6:00 PM                        |
+-------------------+-----------------------------------------------+-------------------------------------------+
| Renewed Contract  | The start date&time cannot be less            | The end date&time cannot be less than the |
|                   | than start date&time of the original contract | end date&time of the original Contract.   |
+-------------------+-----------------------------------------------+-------------------------------------------+

Creating a Renewal
------------------

.. note:: A Contract can have only one renewal. Only the assigned Technician of a Contract can initiate a renewal. 

Acme Inc has purchased Alienware laptops from Vendor Beebon Inc. Beebon Inc is contractually obligated to provide service to Acme Inc. 
Acme Inc has a Service Contract with Beebon that is going to expire after a year. Acme Inc decides to renew the Contract 
and extend it for another year. 

The assigned Technician of the Contract has to update the Contract. Now he has to create a renewal.

- He goes to the :ref:`contract details view`  of the Contract.

.. _con-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-27.png
     :align: center
     :alt: figure 27

- He clicks on **Renew**.

.. _con-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-28.png
     :align: center
     :alt: figure 28

- A dialog box opens where he gets the following fields:

    .. _con-29:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-29.png
        :align: center
        :alt: figure 29

  a. **Contract Start and End date&time**: The time period of the new Contract.      

  b. **Currency and Cost**: Currency selection from the system currency list (Learn how to add :ref:`currency<pur-currency>`) and
     the total cost of the renewal.

  c. **Description**: Details of the renewal if any.

- He fills the details of the new Contract and clicks on **Renew**. The start and end time of the Contract is set considering the
  :ref:`Renewal date and time conditions`.  

- The new Contract will start after the expiry of the current active Contract. When the new Contract starts, the old Contract will expire 
  and the Renewed status will change to Yes. The Renewed Contract is visible under the Renewals tab.

.. _con-30:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-30.png
    :align: center
    :alt: figure 30

Child Contract
==============

A Contract can have multiple sub-contracts. In the product, a sub-contract is referred to as a Child Contract. 
A sub-contract is a contract between a party to an original contract and a third party. An original Contract is referred to as a 
Parent Contract. 

The relationship between a Parent Contract and its children can be defined as follows:

-  There's a direct relationship between a Parent and its children with regards to expiry and cancellation. 

-  When a Parent Contract expires, all its child Contracts also expire.

-  When a Parent Contract is cancelled, all its child Contracts are also get cancelled.

**To add a Child Contract**

While :doc:`creating a Contract <create-a-contract>`, you get the option to select a Parent Contract. If you select a Parent Contract, 
then the Contract that you are creating becomes a Child Contract. You can view all Child Contracts of a Parent Contract under the
**Child Contracts** tab on the Details View. 

.. _con-31:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-31.png
    :align: center
    :alt: figure 31


.. _con-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-32.png
    :align: center
    :alt: figure 32

.. _con-notifications:

Notifications
=============

The Contract module has pre-defined Notifications and also the option to send custom Notification. Currently, there are four
pre-defined Notifications out of the box. They are as follows:

You will find the pre-defined Notifications in **Admin** (A Navigation tab) >> **Email Notifications** (under Automation) >> under **Contract**. 

.. _con-33:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-33.png
    :align: center
    :alt: figure 33

+------------------------------------------------------+-------------------------------------------------------+
| Notify When Contract is Cancelled                    | The assigned Technician gets an email                 |
|                                                      | notification when a Contract is Cancelled.            |
+------------------------------------------------------+-------------------------------------------------------+
| Notify When Contract is Renewed.                     | The assigned Technician gets an email                 |
|                                                      | notification when a Contract is Renewed.              |
+------------------------------------------------------+-------------------------------------------------------+
| .. _notify-settings:                                 | Notify a select set of people by an email about       |
|                                                      | the expiry of a Contract before a set number of days. |
| Notify When Contract is about Expire before 15 days. | The recipients are added from the Notify Settings     |
|                                                      | in the Details View of a Contract.                    |
+------------------------------------------------------+-------------------------------------------------------+
| Notify When Contract is Expired                      | The assigned Technician gets an email                 |
|                                                      | notification when a Contract expires.                 |
+------------------------------------------------------+-------------------------------------------------------+

Notify Settings
---------------

A Technician can add recipients to a Contract who will receive an :ref:`email notification<notify-settings>` telling them that the Contract is going to
expire after a certain number of days. The Technician can control who receives the email and the number of days before (the email
is sent) expiry.

**To Configure Notify Settings:**

- Go to the :ref:`Contract Details View` of the Contract of which you want to configure Notify Settings.

- Click on **Notify Settings** from the Action Menu.

.. _con-34.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-34.1.png
    :align: center
    :alt: figure 34.1

.. _con-34.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-34.2.png
    :align: center
    :alt: figure 34.2    

- When you are done Configuring, hit **Update** to save your settings.

Custom Notification
-------------------

A Technician can generate a notification instantaneously from the :ref:`Contract Details View` of a Contract. He can add multiple recipients and add a 
custom message body. 

**To send a custom notification:**

- Go to the :ref:`Contract Details View` of a Contract.

- Select **Send Email** from the Action Menu.

.. _con-35:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-35.png
    :align: center
    :alt: figure 35

- A dialog box opens where you can create a custom notification.

.. _con-36:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-36.png
    :align: center
    :alt: figure 36

- When you are done creating a custom notification, hit **send**.

.. note:: You can view all sent Custom Notifications under the Notifications tab. 

.. _con-37:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-37.png
    :align: center
    :alt: figure 37

.. _con-attachments:

Attachments
===========

A Technician can add Attachments to a Contract. A Contract can have multiple Attachments. To add a Attachment:

- Go to the :ref:`Contract Details View` of a Contract.

- You will find all existing Attachments under the **Attachments** tab. Click on **Add an Attachment**.

.. _con-38:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-38.png
    :align: center
    :alt: figure 38

- A dialog box opens where you have to add a name and description, and attach a file. 

.. _con-39:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-39.png
    :align: center
    :alt: figure 39

-  Click on **Add** when you are done. The attached file will be added to the Contract.




 
