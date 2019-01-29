********************
Asset Reconciliation
********************

A Purchase order is closed when ordered Assets are received and payment is done. The Assets that are received are automatically added to the
CMDB with the status **In Stock**. 

When these Assets are discovered during an Asset Scanning (could be Agent-less or Agent Based), duplicate entires are
created in the CMDB. A Technician has to manually reconcile each Asset with an **In Stock ** Asset. Reconciliation facilitates proper
inventory management where a Technician knows exactly which Assets are available for assignment.  

Maximum two Assets can be reconciled at a time.

Conditions for Asset Reconciliation:

- Two Assets can be reconciled at a time.

- Any one of them has to have an Origin: Purchase Order.

What happens after Reconciliation of two Assets ?

- The Asset with Origin: Purchase Order is deleted.

- The Asset that is not deleted gets the following information added from the deleted Asset:

  a. Product info.

  b. Purchase Order details.

  c. The associated Purchase Order is linked (Relation) with the Asset.

  d. Used By and Manage By fields are updated, if any.
     

Manual Reconciliation of Assets
===============================

**Reconciliator from Details View:**

- Go to the :doc:`asset-list-view` (of Hardware Assets).

- :ref:`Search <am-using-search-bar>` for the discovered Asset that you want to reconcile. Click on the Asset Name and go to its :doc:`Details View <manage-asset-details>`.

.. _am-rc-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-RC-1.png
    :align: center
    :alt: figure 1

- Click on **Reconcile** from the **Action Menu**. A dialog box opens which has a search box similar to the one on the
  :ref:`Asset List View <am-using-search-bar>`. 

- Search for an In Stock Asset with which you want the discovered Asset to be reconciled and select. 

.. _am-rc-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-RC-2.png
    :align: center
    :alt: figure 2

- Click on **Reconcile**. 

**Reconciliation from Asset List View:**

- Go to the :doc:`asset-list-view` (of Hardware Assets).

- In the list area, select one or more Assets. 

- The **Reconcile** button appears on the top. Click the button to begin the Reconciliation process. It will ask for a confirmation.

.. _am-rc-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-RC-3.png
    :align: center
    :alt: figure 3


Auto Reconciliation of Assets
=============================

If you update the Host Name of an Asset in the CMDB, created because of a PO, with the Host Name of the actual Asset in use, then during 
discovery the Assets will be auto-reconciled. 

You can update the Host Name of an Asset from its :ref:`Details View <change-name-description-asset>`.  




