*************************
Creating a Purchase Order
*************************

A Purchase Order is an official acknowledgement of intent of purchase of Assets from a third party. A PO is a legally binding document between a buyer and seller. 
It has the following key information:

- Vendor Details.

- Product Info.

- Purchase quantity.

- Agree price

- Billing and Shipping addresses.

A Technician (with create :ref:`PO rights <Technician Roles>`) can easily generate a PO right from a Request or separately. After creating a PO, the Technician
has to fill in the PO details and save it.

Based on our :ref:`Use Case <pur-use-case>`. A Request was marked as a Purchase Request by a Technician. A Technician moves forward and
creates a PO from the Purchase Request. 

Creating a PO from a Request
=============================

One benefit of creating a PO for a Purchase Request is that it's automatically linked with the Request.

- A Technician opens the :ref:`Request Details View` of the Purchase Request. 

- He clicks the **Relations** tab and then the **Create and Relate** button. 

.. _pur-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-4.png
    :align: center
    :alt: figure 4

- A dialog box opens with the following fields:

    .. _pur-5:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-5.png
        :align: center
        :alt: figure 5

    a. Name of the PO.

    b. Deadline for the Purchase process.

    c. A Template to fill the PO details (:doc:`Learn More <create-po-template>`).

    d. Description of the PO

- A PO is created which is visible in the **Purchase** section (:numref:`pur-4`).    

Creating a PO from Purchase List View
======================================

.. note:: Creating a PO directly from the Purchase List View will not create a Relationship with the Purchase Request. 

- A Technician clicks on the Launcher icon from the Technician Dashboard. 

- Then he selects **Purchase**.

.. _pur-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-6.png
    :align: center
    :alt: figure 6

- Purchase List View opens. Here all existing Purchase Orders are visible. He clicks on **Create a Purchase Order** situated in the
  top right corner of the page to create a PO. 

- A dialog box opens which is similar to :numref:`pur-5`. Clicking on **Create** directs the Technician to another page where he has
  to fill in te details of the PO (:doc:`Learn More <edit-po-details>`). 

- After filling the PO details, the Technician has the option to link the PO with a Purchase Request (:doc:`Learn More <po-relationships>`).
