************************************
Different Stages in a Purchase Order
************************************

A Purchase Order goes through six stages before a Technician can close it. They are as follows:

.. _pur-41:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-41.png
    :align: center
    :alt: figure 41

- Open

- Approval 

- Order

- Receive 

- Payment

- Review

- Close

Each stage is unique can have its own set of rules. There is a limited scope for Technicians to jump stages in a PO.

Some of the benefits of having a multi-stage Purchase Management are:

- It makes a purchase visible and controllable. 

- Ensures accuracy of pricing, quantity, and materials or services ordered is exactly what is billed. 

- Greater financial control over purchases.

- Allow only authorized employees to initiate purchase orders.

- Complete purchases on time. 


Based on our :ref:`Use Case <pur-use-case>`. A Request was marked as a Purchase Request by a Technician. A Technician has created a PO from
the Purchase Request and has updated the PO details. Now the assigned Technician (only assigned Technician can initiate Approval) takes the PO through all the stages and closes the PO before the Required By time.

The Transition through the stages happen over a course of time and is controlled using pre-defined and :ref:`custom rules <ad-custom-rule>`.

Open Stage
==========

The assigned Technician submits the PO for Approval. The status changes to **Approval: Pending**.

.. note:: Only an assigned Technician can initiate an Approval process. 

.. _pur-42:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-42.png
    :align: center
    :alt: figure 42

Certain fields can be made compulsory at this stage. Learn about :ref:`Purchase Custom fields <purchase-custom-rules>`.

Approval Stage
==============

First, the system checks all available Approval Workflows when an
Approval is asked. If there are no workflows or the workflow
conditions are not meet, then the PO is Approved, and the Technician can proceed to the next stage. If there is a
workflow/are workflows, and their conditions are met, then
approver/approvers across multiple Approvals are assigned to the PO. 

Here an Approval is created and it goes to a another person (Finance department). Approval details can be viewed under the **Approvals** tab.

.. _pur-43:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-43.png
    :align: center
    :alt: figure 43

The Approver approves the Approval from **My Approval**.

.. _pur-44:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-44.png
    :align: center
    :alt: figure 44

The stage of the PO automatically changes to **Order: Pending**.

.. note:: Related Topic: :ref:`Understanding Approval Workflow`.

If the Approval had failed, then the Technician could have used the **Re-Approve** option. 
It creates a duplicate Approval and ignores the previous one. He also had the option to ignore individual approvers.

.. note:: Only Technicians with certain rights can ignore Approvals and Approvers.

.. _pur-45:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-45.png
    :align: center
    :alt: figure 45

Order Stage
===========

At this stage, the Technician confirms the PO by clicking on **Order**. The system then asks for permission to change stage. 
On confirmation, a dialog box opens which the Technician uses to send an email. The status changes to **Receive: Pending**.

.. _pur-46:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-46.png
    :align: center
    :alt: figure 46

Certain fields can be made compulsory at this stage. Learn about :ref:`Purchase Custom fields <purchase-custom-rules>`.

Receive Stage
=============

At this stage, the Technician waits for the delivery of the goods. The Technician can accept the goods any time after the Approval 
stage. 

The Technician accepts the delivery by clicking on **Receive Item**. In a new dialog box, he updates the quantity received.

.. _pur-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-47.png
    :align: center
    :alt: figure 47

The moment he receives the items, the status changes to **Partially Receive**; this status signifies waiting for order completion.
The Technician manually changes the status to **Received** (after Receiving all the items) which pushes the PO to the next stage after a confirmation. 

Certain fields can be made compulsory at this stage. Learn about :ref:`Purchase Custom fields <purchase-custom-rules>`.

Payment Stage
=============

The Technician receives an Invoice from the Vendor. He updates the status to **Invoice Received**. He uploads the Invoice by 
going to the **Invoice and Payments** tab and clicking on **Add Invoice**. 

.. _pur-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-48.png
    :align: center
    :alt: figure 48

He adds periodic payments to the Invoice while keeping the PO status as **Payment: Partially Received**. He saves the payments in the
**Invoice and Payments** tab by clicking on **Make Payment** adjacent to the invoice. The technician can see what amount is still due here.

.. _pur-49:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-49.png
    :align: center
    :alt: figure 49

The Technician changes the status to **Payment Done** when full amount is paid. On confirmation, the PO moves to the next stage.

Certain fields can be made compulsory at this stage. Learn about :ref:`Purchase Custom fields <purchase-custom-rules>`.

Review
======

The Technician reviews the PO and closes it. The PO moves to the Closed stage.

Certain fields can be made compulsory at this stage. Learn about :ref:`Purchase Custom fields <purchase-custom-rules>`.

