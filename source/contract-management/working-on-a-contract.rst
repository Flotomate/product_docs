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
    
   c. :ref:`Child Contracts`

   d. :ref:`Notify Settings`

   e. :ref:`Attachments`

   f. :ref:`Notification`

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

Contract Type
-------------

A Contract Type shows the nature of relationship between two or more parties. Every Contract has a type, and we give four types
out of the box. You can add more types (Learn how to add more :doc:`contract-types`). Following are the pre-defined types:

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

A Contract is created around an Asset/Assets, and it defines the obligation of the seller and duties of the buyer. A Contract always
has an association with an Asset/Assets;

You can link an Asset/Assets with a Contract is the following way:

- Go to the :ref:`contract details view` of a Contract.

- You can find all existing association under the **Assets** tab. To add a new Asset, click on **Associate Asset**.

.. _con-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-24.png
    :align: center
    :alt: figure 24

- A new dialog box opens, where you can search and associate multiple Assets. 

    .. _con-25:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-25.png
        :align: center
        :alt: figure 25

  You can add the following class of Assets:

  .. _con-26:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-26.png
        :align: center
        :alt: figure 26

  Based on the selected Asset class the list area is populated. 

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

Acme Inc has purchased Alienware Servers from Vendor Beebon Inc. Beebon Inc is contractually obligated to provide service to Acme Inc. 
Acme Inc has a Service Contract with Beebon that is going to expire within six months. Acme Inc decides to renew the Contract 
and extends it for another year. 

The assigned Technician of the Contract has to update the Contract. Now he has to create a renewal.

- He goes to the :ref:`contract details view`  of the Contract.

- 


