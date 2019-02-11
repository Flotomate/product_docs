Change Workflow without Rejection:
==================================

-  The workflow starts with the submission of a Change (Request for
   Change) by a Requester.

-  A Technician is :doc:`assigned <assigning-a-change>` to the Change, and then he
   assigns a Change Manager.

-  Either the Assignee, Change Manager or anyone with the update Change
   right can approve the Change, and it then moves to the Planning
   Stage.

-  In the Planning stage, anyone who has the update Change right can
   complete the Planning stage and move the Change to the Approval
   stage.

-  In the Approval stage, the assigned Technician appoints approvers for
   :ref:`Approval <Approval in Change>`. He can appoint n number of
   approvers. Alternatively, the RFC can go to approvers automatically if there are pre-defined workflows already. 

   An approver gets to see his Approvals in the **My Approvals** section
   of his account.

    .. _cmf-50:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-50.png
        :align: center
        :alt: figure 50

  Clicking on **My Approvals** (:numref:`cmf-50`) opens the My Approvals page
  where the approver can view his Approvals.

    .. _cmf-51:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-51.png
        :align: center
        :alt: figure 51

  Clicking on an Approval opens a page with the subject line as the page
  header title. It resembles the :ref:`Details View <change-details-view>`
  of a Change but has no editing capabilities.

  Here the approver can start conversation threads and finally decide
  whether to approve or reject the Approval. Anyone can be part of these
  conversation threads as long as he/she has access to the comment
  section.

    .. _cmf-52:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-52.png
        :align: center
        :alt: figure 52

-  On approval, either unanimous or majority, the Change moves to the
   Implementation stage. A Technician with update Change right assigns a
   Change Implementer and Change Reviewer.

   At this stage, the Change is implemented. On success, the Change is
   marked as Completed.

-  The Change moves to the final stage where the Change Reviewer audits
   the Change implementation. On successful audit, the Change is marked
   as Completed. This ends the journey of the Change in the system.

Change Workflow with Rejection:
===============================

At any given stage a Change can be either rejected or put on hold.

-  In Submitted and Planning stage, any Technician with update Change
   rights can reject the Change using the **Rejected/Cancelled** button
   after the Change has an assigned Technician.

   The **Req.Info** (button name can be modified and additional buttons
   can be added) button (:numref:`cmf-53`) puts the Change on a custom status.
   It is a way to tell the requester to provide further information for
   the Change to move forward.

.. _cmf-53:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-53.png
    :align: center
    :alt: figure 53

-  In Approval and Implementation stage, the **Rejection** button
   rejects a stage. A Technician can put the Implementation on a custom
   status (Backout and other custom buttons) or send the Change back to
   Planning stage by clicking on **Back to Planning** (Only after
   rejecting the stage).

.. _cmf-54:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-54.png
    :align: center
    :alt: figure 54

-  The In-Review stage has the **Req.info** (you can add other custom
   buttons) for putting the Change on a custom status and **Failed** to
   reject.

On rejection, a stage turns red, and the Technician can close the Change
by clicking on **Close this Change** situated in the top right corner of
the page.

.. _cmf-55:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-55.png
    :align: center
    :alt: figure 55

.. _cmf-56:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-56.png
    :align: center
    :alt: figure 56

The Change reaches the last stage and closes with the status Closed. A
Technician can reopen the Change by clicking on **Reopen** (:numref:`cmf-56`).