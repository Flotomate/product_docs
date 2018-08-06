******************************************
Creating Relationships in a Purchase Order
******************************************

A Technician can relate a Purchase Order with a Request and an Asset. He/she can create multiple relationships in a PO. 
Some of the use cases where a relationship is created are as follows:

- If a PO is created against a Request for new Assets then a relationship is created between them.

- If a PO has created new Assets in the CMDB (with the status In Stock) then a relationship is created automatically between them.
  When an Asset (In Use) is reconciled with an Asset (In Stock) then the Asset (In Use) inherits the relationships of the Asset (In Stock).

- Manually creating a relationship in a PO with an Asset already in use. 

**To Create a Relationship:**

- Go to the :ref:`Details View <Open Purchase Order Details View>` of a PO.

- Click on the **Relations** tab. The tab gives you an option to create relationships
  between Requests and Assets.

  You can view the present connections of the PO on the left hand side.

  You can create a new Request and an Asset and link it to
  the PO using the **Create and Relate** option.

  The **Add Relation** option lets you add one or more relationships with
  existing Requests and Assets.

  a. Clicking on **Add Relation** shows you a popup menu where you have to
     select either Request or Asset.

  b. A dialog box opens with a search box (it supports Advanced Search)

  c. Search for the right entry and click **Link** to add a relationship
     between your selection/selections and the PO.

.. _pur-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-28.png
    :align: center
    :alt: figure 28     

