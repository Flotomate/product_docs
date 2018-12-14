.. _ad-custom-rule:

************
Custom Rules
************

Using Custom Rules, you can set pre-requisites that need to be done
before performing certain actions. You can have Custom Rules for
Request, Problem, Change, Knowledge, Asset, Project, Remote Deployment and Purchase.

To Open Custom Rules:

-  Go to **Admin** >> **(Request, Problem, Change, Knowledge, Asset, Purchase, Project or Patch)
   Custom Rules**.

.. _adf-108.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-108.1.png
    :align: center
    :alt: figure 108.1

.. _adf-108.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-108.2.png
    :align: center
    :alt: figure 108.2

Current Custom Rules are as follows:

Request(CR)
===========

-  **Before resolving a Request**:

   a. User Interaction:

      i.   Should have at least one message in Ask Requestor tab.

      ii.  A Request should have at least one note.

      iii. Should have at least one solution.

   b. Mandatory fields:

      i. Should have an assigned Technician.

      ii.   Should have a Location.

      iii.    Should have an Estimated Time.

      iv.   Should have a Diagnosis.

      v.  Should have a Source.

      vi. Should have Approval status as either Approved or Pre-Approved.

   c. Should have all Tasks as closed.

-  **Before closing a Request**:

   a. Same as before resolving a Request.

   b. Should not skip Resolve status.

-  **Required to add a Note before**:

   a. Should add a Note to a Request before performing the following
      actions:

      i.   Changing assigned Technician of a Request.

      ii.    Changing Support Level of a Request.

      iii.   Changing Due Date of a Request.

      iv.  Changing Category of a Request.

      v. Changing Department of a Request.

      vi.   Changing Priority of a Request.

Problem(CR)
===========

-  **Before resolving a Request**:

   a. User Interaction:

      i.  A Request should have at least one note.

      ii. Should have at least one solution.

   b. Mandatory fields:

      i.  Should have an assigned Technician.

      ii. Should have a Location.

      iii.  Should have a Root Cause.

      iv.   Should have a Symptom.

      v.  Should have an Impact.

      vi. Should have Approval status as either Approved or Pre-Approved.

   c. Should have all Tasks as closed.

-  **Before closing a Request**:

   a. Same as before resolving a Request.

   b. Should not skip Resolve status.

-  **Required to add a Note before**:

   a. Should add a Note before performing the following actions:

      i. Changing assigned Technician.

      ii.   Changing Due Date.

      iii.    Changing Category.

      iv.   Changing Department.

Change(CR)
==========

You can set rules for each stage of a change process.

-  **Submit**:

   a. Should have a Change Manager.

   b. Should have an assigned Technician.

   c. Should have a Location.

-  **Planning**:

   a. Should have schedule and rollout dates.

   b. Should have a rollout plan.

   c. Should have an assigned Technician.

   d. Should have set impact.

   e. Should have a Backout plan.

-  **Implementation**:

   a. Should have a change implementer.

   b. All task must be closed before moving to the next stage.

   c. Should have an assigned Technician.

-  **In Review:**

   a. Should have a change reviewer.

   b. Should have an assigned Technician.

-  **Require Note befor**\ e:

   a. Changing category.

   b. Changing assigned Technician.

   c. Changing Department.

   d. Changing Location.

Asset(CR)
=========

-  Manual Update:

   .. note:: Asset rules are applicable for both discovered and manually created Assets.

   a. Whether to allow Technicians to update Hardware Components of an
      Asset.

   b. Whether to allow Technicians to update Software Components of an
      Asset.

   c. Whether to allow Technicians to update Users details of an Asset.

Knowledge(CR)
=============

Whether Knowledge should be approved by approvers before publishing.

Remote Deployment(CR)
=====================

Whether a deployment of Patches and Packages needs to go through an
Approval process.

.. _purchase-custom-rules:

Purchase(CR)
============

You can set rules for each stage of a Purchase Order process. A Purchase Order cannot move to a different stage as long as it's violating
a rule of its present stage. 

Learn what are the :doc:`Purchase Rules <po-purchase-rules>`.

Project(CR)
===========

- **Project Complete Rules**

  a. Mandatory fields before marking a project complete.

     i. Category

     ii. Location

     iii. Owner

  b. Prerequisites before marking a project as complete.

     i. All milestones must be marked as complete. 
     
     ii. All tasks must be closed

- **Milestone Complete Rules**

  a. Decide whether **Owner** should be mandatory field or not.

  b. Decide whether all tasks associated with the milestone needs to be closed before marking the milestone as complete.

- **Task Closure Rules**

  a. Decide whether **Owner** should be mandatory field or not.