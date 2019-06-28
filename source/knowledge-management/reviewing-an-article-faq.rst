************************
Reviewing an Article/FAQ
************************

You can review the entire content of an Article/FAQ. It is possible for
both drafted and published Articles/FAQs with plus & minus few features.

In order to review an Article/FAQ, you have to open the Article/FAQ in
full view. You can search and open any Article/FAQ from the
:doc:`Homepage <modifying-a-knowledge-article-faq>`.

.. _kbf-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-19.png
    :align: center
    :alt: figure 19

.. _kb-comment:

Comment
=======

Motadata allows you to add comments in an Article/FAQ. Commenting lets,
you communicate with an audience. By commenting, you can highlight
issues or ask questions. You can comment on both drafted and published
Articles/FAQs.

Adding a Comment
----------------

-  Open an Article/FAQ.

-  You can see all current comments on the right side pane if any. You
   can search for a comment using the search box and even sort them
   based on time. Click on **Add Comment** to add a new comment.

.. _kbf-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-20.png
    :align: center
    :alt: figure 20

-  The pane expands to show a paragraph text field where you can enter
   your comment.

-  The **Reply** button inside a comment allows you to start a
   conversation thread.

Resolving a Comment
-------------------

Resolving a comment marks it as closed, and it is no longer visible. It
is available for Articles only, and anyone with update Knowledge rights
can resolve a comment.

.. note:: Remember that a drafted Article with unresolved comments cannot be published.

-  Open an Article.

-  Click on **Mark as Resolved** against the comment you want to
   resolve. The comment disappears when it is resolved.

.. _kb-approval:

Approval
========

In case there is a :ref:`custom rule <Custom Publish Rule>`, then you have
to make every drafted Article go through an Approval process before
publishing it. In an Approval process, you seek approval from an
approver/approvers.

Initiating Approval Process:
----------------------------

.. note:: only a creator of an Article can initiate an Approval for the same.

-  Open a drafted Article.

-  Click on **More** and then **Approval**.

.. _kbf-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-21.png
    :align: center
    :alt: figure 21

-  Approval details dialog box opens. Clicking on **Ask for Approval** initiates the Approval process

Different States in an Approval Process
---------------------------------------

-  Approval Pending:

-  Approval Rejected:

-  Approval Pre-Approved:

-  Approval Approved:

Approval Process:
-----------------

.. note:: An assigned Technician can initiate an Approval process for n number of times. At the start of each process, the 
          Article will start from the Pending status. 

-  An Approval can be initiated manually or automatically by an Approval Workflow. When the :ref:`manual approval option <Allow Manual Approval>` 
   is turned on, you get the following dialog box when you click on **Ask for Approval**.

    .. _kbf-21.1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-21.1.png
        :align: center
        :alt: figure 21.1  

   When you create a manual approval, the system also checks for Approval workflows. Incase a workflow is triggered,
   both the manual approval and an automatic Approval are created. You can skip manual approval altogether using the 
   **Skip** button. 

-  When an Approval process is initiated, first the system checks for
   available Approval Workflows. If there are no workflows and no manual approval, then the
   drafted Article is Pre-Approved, and you can proceed with publishing.
   If there is a workflow or a manual approval, then based on its set conditions
   approver/approvers are auto-assigned/assigned for approval.

-  You can view all the approvers and their comments in the Approval
   details dialog box.

    .. _kbf-21.2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-21.2.png
        :align: center
        :alt: figure 21.2

    .. _kbf-22:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-22.png
        :align: center
        :alt: figure 22

   The Approval status changes to Pending, and it stays there as long as
   the approver/approvers don’t express a decision.

-  An approver can see his Approvals in the My Approvals section of his
   account.

    .. _kbf-23:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-23.png
        :align: center
        :alt: figure 23

   Clicking on My Approvals (:numref:`kbf-23`) opens the My Approval page where he
   can view his Approvals.

    .. _kbf-24:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-24.png
        :align: center
        :alt: figure 24

   Clicking on an Approval in **My Approval** opens a dialog box. There he
   can perform the following actions:

    .. _kbf-25:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-25.png
        :align: center
        :alt: figure 25

    a. Open the Article.

    b. Start a comment thread which is visible to anyone having access to
       the comment section.

    c. Reject or Approve the Approval

-  The outcome of an Approval process is decided in two ways:

   a. **Unanimous**: All of the Approvers have to approve else the
      Approval is rejected.

   b. **Majority**: If the majority of Approvers agree then Approval is
      successful.

      In case there are multiple Approvals, the decision to go with
      unanimous or majority can be set from **Admin** (A Navigation Tab)
      >> **Approval Workflow** (Automation) >> **Approval Settings**,
      but the rights to do it lies with the Super Admin.

-  On success, the Approval moves to the Approved stage where the author
   can publish the draft. On failure, the Approval moves to the Reject
   stage where the author has to re-initiate the Approval process. The
   author re-initiates an Approval process using the Re-Approve option or by starting a fresh approval using the **Ask for Approval** option.

.. _kbf-26:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-26.png
    :align: center
    :alt: figure 26

.. _kbf-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-27.png
    :align: center
    :alt: figure 27

-  Any Technician with the **Can Ignore Approval** right can ignore
   approvers and push the Approval towards the Approved stage; where he
   can publish the draft. The ignored approvers can see their Approval
   status as Ignored in Approval details dialog box of the Article.

.. _kbf-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-28.png
    :align: center
    :alt: figure 28

-  Throughout the Approval stage, no one can modify the folder of the
   Article.

Related Topics:

-  :ref:`Understanding Approval Workflow`
-  :ref:`Creating an Approval Workflow`
-  :ref:`Allow Manual Approval`   

Linked Events
=============

Motadata helps Technicians to build contextual information by creating
relationships between various events in the system. The product allows
you to view all linked events of a published Article/FAQ. You can view
relationships with the following types of event:

-  Request

-  Problem

-  Change

-  Asset

**View/Unlink events:**

-  Open an Article/FAQ.

-  Click on **More** and then **Linked Events.**

.. _kbf-29:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-29.png
    :align: center
    :alt: figure 29

.. _kbf-30:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-30.png
    :align: center
    :alt: figure 30

-  In the new dialog box, you can view all the events by type and even
   unlink individual events.

View Audit Trail
================

The Audit Trail of an Article/FAQ shows all updates and changes along
with date and time. It works in both draft and publish mode.

To View Audit Trail:

-  Open an Article/FAQ.

-  Click on **More** in the top right corner. Select **Audit Trail**
   from the pop-up menu. The Audit Trail dialog box opens where you can
   view and search changelogs.

.. _kbf-31:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-31.png
    :align: center
    :alt: figure 31

.. _Change Visibility:

Change Visibility and Permissions
=================================

You can decide who can see an Article/FAQ by changing the Visibility
settings. You can change this setting for both drafted and publish
Articles/FAQs.

To change Visibility:

-  Open an Article/FAQ.

-  Click on Visibility situated at the top left.

.. _kbf-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-32.png
    :align: center
    :alt: figure 32

.. _kbf-32.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-32.1.png
    :align: center
    :alt: figure 32.1

-  Select any one option from the pop-up menu. Know more about the
   :doc:`options <authoring-an-article-faq>`.

- Based on the Visibility option selected, you also have to set the permission which will give editing and viewing rights to other
  users. 

.. _kbf-32.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/knowledge-management/KB-32.1.png
    :align: center
    :alt: figure 32.1