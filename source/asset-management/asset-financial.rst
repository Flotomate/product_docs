***************
Asset Financial
***************

All Assets in a business carry an Accounting obligation; IT Assets are no different. Currently, we support financial data for 
Hardware and Non-IT Assets to meet the following requirements:

.. _amf-fin-0:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-0.png
    :align: center
    :alt: figure 0

.. note::  The above view can be accessed from the :ref:`Details View <Manage Asset Details>` of an Hardware/Non-IT Asset.

- Total Cost of an Assets and its break-up into the followings:

  a. **Purchase Cost**: The value at which the Asset was purchased including all taxes.

  b. **Operational Cost**: Additional cost associated in making the Asset operational/working. 

  c. **Other Cost**: Miscellaneous cost. 

  d. **Disposal Cost**: These are additional costs incurred when disposing the Asset.

- **Book Value**: Current value of the Asset as recorded after accounting for Depreciation. 

- **Depreciation**: Depreciation refers to the decrease in the value of an Asset. The cost of an Asset in allocated over the
  period in which the Asset is used. Here we support four types of Depreciation:

  a. **Straight Line**: In this method, a fixed amount is deducted every year from the cost (after accounting for Salvage Cost) over the useful life of the Asset.
     Depreciation expense = (Cost of Asset - Salvage Cost)/Useful life of the Asset.

  b. **Declining Balance**: It's an accelerated method of depreciation where there's a rate of depreciation rather than a fixed about. 
     A fixed rate is deducted every year over the useful life of the Asset. Depreciation per annum = (Net Book Value - Residual Value) x rate of Depreciation%.

  c. **Sum of the Years Digit**: A higher expense is deducted early on in the life of an Asset and a lower expense is deducted in the
     later part of the Asset's life. Depreciation Expense = (Remaining life / Sum of the years digits) x (Cost – Salvage Cost)

  d. **Double Declining Balance**: In this method a larger expense is allocated early on in the life of an Asset and gradually lower expense is allocated
     as the Asset reaches the end of its useful life. With the double-declining-balance method, the depreciation factor is 2x that of a straight line expense method.
  

How Costs and Depreciation are Recorded in an Asset?
===================================================

A user can record costs in an Asset in the following ways:

- Manually adding costs from the Details View.

- Creating an Asset from a :ref:`Purchase Order <Introduction to Purchase Management>`; here the purchase cost details are automatically imported from the PO.

- Importing Depreciation config from a :ref:`Product <Configure Depreciation>` through association.

- Directly adding Depreciation Configuration to the Asset, rather to the associated Product. 

Adding Costs to an Asset
------------------------

Financial of an Asset shows the **Total Cost** which is the sub-total of Purchase Costs, Operational Costs, Other Costs and 
Disposal Costs. To add a cost:

- Go to the :ref:`Details View <Manage Asset Details>` of a Hardware/Non-IT Asset.

- Under the Financial tab, click on **Add Cost**. 

    .. _amf-fin-1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-1.png
        :align: center
        :alt: figure 1

- A dialog box opens where you have to input the following.

    .. _amf-fin-2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-2.png
        :align: center
        :alt: figure 2
  
   a. Type of Cost.

   b. Date and time of the entry.

   c. Cost value.

   d. Description of the cost.

.. note:: You can add n number of cost items; they all will be added to the total cost.
  
- When done, click on **Create**. The process is same for adding other types of costs.

Purchase Cost from PO
^^^^^^^^^^^^^^^^^^^^^

An Asset can be created from a Purchase Order. If the Asset is a Hardware or Non-IT Asset then the Purchase Cost is automatically fetched.
Learn about Purchase Orders (:ref:`Use Case <pur-use-case>`)

.. _amf-fin-2.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-2.1.png
    :align: center
    :alt: figure 2.1

Setting Up Depreciation Configuration
-------------------------------------

Depreciation is systematic deduction in Total Cost (of an Asset) over the useful life of the Asset. In order to perform such deductions, the Asset needs
a Depreciation Configuration. 

If the associated :ref:`Product has Depreciation config set up <product-depreciation>`, then it will be inherited by the Asset; else, one has to set it. You can set
up Depreciation Configuration with the associated product or with the Asset. 

To set up Depreciation Configuration:

- Go to the :ref:`Details View <Manage Asset Details>` of a Hardware/Non-IT Asset.

- Under the Financial tab, click on **Configure Depreciation**. 

    .. _amf-fin-3:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-3.png
            :align: center
            :alt: figure 3

- A dialog box opens, where you have to select whether you want to import the config from Product (in the catalog), set up a config
  specifically for the Asset or no depreciation. 

  .. _amf-fin-4:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-4.png
        :align: center
        :alt: figure 4

- If you select to set up a Depreciation Configuration specifically for the Asset, then you have to enter the following inputs:

    .. _amf-fin-5:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-5.png
          :align: center
          :alt: figure 5
  
   a. A Depreciation method.

   b. A **Depreciation Type**: Giving a useful life helps to ascertain the rate of Depreciation or explicitly you can mention 
      a rate of Depreciation.

   c. **Salvage Amount**: The value of the Asset at the end of its life.

- When done, click on **Configure**. Lean more about `Depreciation <https://corporatefinanceinstitute.com/resources/knowledge/accounting/types-depreciation-methods/>`_.
  
Viewing Depreciation Schedule
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Once Depreciation Configuration is set up, you can view the Depreciation Schedule under the Financial (of the :ref:`Asset Details <Manage Asset Details>`); it shows three important
data points:

- Total Depreciation for a month or year.

- Accumulated Depreciation up-to a particular point in time.

- Book of value (Asset cost adjusted for depreciation) of the asset at a particular point in time.

- Remaining life.

You can change the view of the schedule from monthly to yearly.

.. _amf-fin-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-FIN-6.png
    :align: center
    :alt: figure 6
