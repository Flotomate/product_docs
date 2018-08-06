******************************
Editing Purchase Order Details
******************************

When a PO is created it is devoid of any details about the following:

- Vendor details (A PO can have only one Vendor)

- Product, quantity and price details.

- Shipping and billing Addresses.

- General information.

- Additional information

.. note:: If the PO is using a Template, certain fields are pre-populated (:ref:`Learn about the fields <Create PO Template>`)

Based on our :ref:`Use Case <pur-use-case>`. A Request was marked as a Purchase Request by a Technician. A Technician has created a PO from
the Purchase Request. Now he has to update the PO details. 

.. note:: Creating a PO from the :ref:`Purchase List View <Creating a PO from Purchase List View>`, automatically redirects the
          Technician to the Create a Purchase Order page, where he can edit the PO details.

Open Edit a Purchase Order Page
===============================

A Technician can edit a PO by clicking on **Edit** from the :ref:`Details View <Open Purchase Order Details View>`.

.. _pur-34:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-34.png
    :align: center
    :alt: figure 34

Filling Purchase Order Details
==============================


A Technician opens the PO (*Purchase 5 Laptops*) in edit mode and fills in the information not filled by the template.

.. _pur-35:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-35.png
    :align: center
    :alt: figure 35

- In Section A, the Technician can change the Name and Required-by-date of the PO; these fields were filled when the PO was
  first created (:doc:`Learn More <create-a-po>`) 

- Section B is already pre-filled by the template (:ref:`Purchase Template <Create PO Template>`) except Vendor. 
  The Technician selects a :ref:`am-vendor` and he can also change the Addresses from 
  the Location list (Learn how to add a :ref:`ad-location`). 

.. _pur-36:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-36.png
    :align: center
    :alt: figure 36

- The Technician can view all Products available with the Vendor in section C. He selects two Products (Dell XPS and ThinkPad T440) and sets 
  the quantity and tax info. The price is automatically calculated based on the given input. An Admin can add more fields to the price 
  column (:ref:`Learn more <custom price fields>`).

.. _pur-37:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-37.png
    :align: center
    :alt: figure 37

.. _pur-38:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-38.png
    :align: center
    :alt: figure 38

- The Technician completes the General Information section (D). Here he gets the following fields:

  a. **Requested By**: The Technician enters the name of the person (could be another Technician) who requires the Assets.

  b. **Owner**: Name of the person who will be the assigned Technician (:doc:`Learn More <assigning-a-PO>`).

  c. :doc:`cost-center` (already pre-filled by the :ref:`Purchase Template <Create PO Template>`).

  d. **Delivery Time**: Estimated delivery time of the goods. 

  e. :doc:`gl-code` (already pre-filled by the :ref:`Purchase Template <Create PO Template>`).

- All :ref:`General Custom Fields` are visible in section E.

.. _pur-39:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-39.png
    :align: center
    :alt: figure 39

- Section F is pre-filled by the :ref:`Purchase Template <Create PO Template>`. The Technician can modify the Description, Remark and
  Terms fields. 

- The name and place of the signing authority goes in the Section G. The Technician enters the Place, and Signing Authority is 
  already pre-filled by the Purchase Template. 

  A signing authority is a person who can approve a Purchase Order.  


Viewing Purchase Order Details
==============================

You can view the PO details from the :ref:`Details View <Open Purchase Order Details View>` under the Purchase Order tab.

.. _pur-40:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-40.png
    :align: center
    :alt: figure 40