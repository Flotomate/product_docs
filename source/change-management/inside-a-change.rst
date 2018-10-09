***************
Inside a Change
***************

Once a Technician decides to work on a Change, he heads to the Details
View. Every Change has a Details View that houses all related
information and tools to make the Change move through all the defined
stages.

Change Details View
===================

The Details View is the central hub for all process related activities.
It organizes and manages all information and the workflow related to a
Change. Every Change has its own Details View.

1. Go to the :doc:`Change List View <change-list-view>`.

2. Scroll down to the list area and click on the name of a Change. The
   Details View opens.

.. _cmf-17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-17.png
    :align: center
    :alt: figure 17

.. _cmf-18:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-18.png
    :align: center
    :alt: figure 18

-  Section-A, B & C are the :ref:`classifiers <classify-an-change>`.

-  Section-C also houses the feature to :ref:`link Knowledge Base with
   Change <adding-people-to-change>`.

-  Section-D provides tools to manage the :doc:`Change implementation
   workflow <cm-use-cases>`.

-  Section-E houses tools to :ref:`schedule Change
   period <cm-collaborate-schedule-and-planning>`.

-  Section-F houses the following functions:

   a. :ref:`Collaborate <cm-collaborate-schedule-and-planning>`

   b. :ref:`Relations <cm-adding-relations>`

   c. :ref:`Task <cm-managing-tasks.>`

   d. :ref:`Custom Fields <ad-custom-fields>`

   e. :ref:`Time Log <cm-time-log>`

   f. :ref:`Approvals <approval-in-change>`

-  Section-G shows you information about the Requester and the time of
   creation of the Change.

-  Section-H houses the following functions:

   a. :doc:`Claim and Assign <assigning-a-change>`

   b. :doc:`View Audit Trail <viewing-audit-trail-of-a-change>`

-  Section-I is where all the related Assets (Configuration Items) are
   shown.

-  Section-J is where :ref:`Planning <cm-collaborate-schedule-and-planning>`
   details are stored.

Modifying a Change’s Subject and Description
============================================

Below the header section of the Details View is the Change ID and
subject line. Next to the subject line is an edit icon that you can use
to modify the Subject and Description.

.. _cmf-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-19.png
    :align: center
    :alt: figure 19

**To edit Subject and Description:**

-  Click on the edit icon. A new dialog box opens.

-  Modify the Subject and Description fields and hit **Update**.

.. _cmf-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-20.png
    :align: center
    :alt: figure 20

Classify an Change
==================

Flotomate provides a lot of avenues to classify the information of a
Change. Go to the :ref:`Details View <change-details-view>` of a Change
where you get the following ways to classify:

.. _cmf-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-21.png
    :align: center
    :alt: figure 21

.. _cmf-22:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-22.png
    :align: center
    :alt: figure 22

-  **Status**: The stage of the Change is shown as Status. There are
   five broad stages that a Change has to go through in order to become
   a Change. This label is automatically updated by the system as the
   Change moves through the stages.

-  **Custom Tags**: These are additional tags that the Requester and
   Technicians can provide. It is a way to categorize the Change when
   default options are not enough.

-  **Due**-**Status**: This label classifies the Change based on the
   number of hours/days before expiry of the scheduled change. This
   classification happens after Change Schedule is set in the Planning
   stage.

-  **Importance**: The Change can be categorized based on its level of
   criticality in the following ways:

   a. **Priority**: Setting this label classifies the Change based on
      its criticality to the business. The Priority labels are
      system-defined and immutable.

   b. **Urgency**: Setting this label classifies the Change based on
      time bound urgency. The label has predefined values that are
      immutable, and they are Low, Medium, High, and Urgent.

   c. **Impact**: Setting this label shows the aspect of a business on
      which a Change has its effect which is either on a User,
      Department or Business.

   d. **Risk**: Setting this label classifies the Change based on the
      risk that it possesses to the IT infrastructure.

-  **Change Type**: Setting this field classifies the Change based on
   its magnitude.

-  **Technician Group**: The product allows grouping of Technicians into
   groups. Setting this field shows which group the Change belongs.

-  **Place**: An Change can be classified based on the associated
   physical locations which are:

   .. note:: Below both fields have predefined values (as a drop-down list)
             set by the Administrator.

   a. **Department**: If the Change is related to a particular
      department, then this field can be set to that department.

   b. **Location**: If the Change is related to a particular location,
      then this field can be set to that location.

-  **Category**: It is the primary method to categorize the Change. You
   get six predefined categories out of the box to choose from.

-  **Change Reason Type**: You can classify the Change based a reason
   predefined in the system. You get the following reasons to choose
   from:

   a. New Rollout

   b. Technology Upgrade

   c. Configuration Update

   d. Maintenance Update

-  **Target Environment**: You can set the environment where the change
   is going to happen as either:

   a. Production

   b. Development

   c. Test

Adding People to Change
=======================

Apart from the assigned Technician, a Change requires three more people.
All of them are added from the **More Details** section in a Change’s
:ref:`Details View <change-details-view>`.

.. _cmf-23:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-23.png
    :align: center
    :alt: figure 23

Change Implementer
------------------

He is the Technician who is responsible for the implementation of the
Change. He supervises actions that are derived from the Planning stage.
Anyone with the necessary rights can add this person as long as the
Change has an assigned Technician.

Change Manager
--------------

He is the Technician who is responsible for the entire Change cycle.
Anyone with the necessary rights can add this person as long as the
Change has an assigned Technician.

Change Reviewer
---------------

He is the Technician who audits the implementation of the Change. His
job is to see whether the Implementation is successful or not. Anyone
with the necessary rights can add this person as long as the Change has
an assigned Technician.

Linking Knowledge with Change 
=============================

You can link a Knowledge Article/FAQ with a Change by following the
below steps:

1. Go to the :ref:`Details View <change-details-view>` of a Change.

.. _cmf-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-24.png
    :align: center
    :alt: figure 24

2. Click on **Search Knowledge** on the Details View. A dialog box
   opens.

.. _cmf-25:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-25.png
    :align: center
    :alt: figure 25

3. In the dialog box, you see a search bar and a list area. Use the
   search bar to search for Knowledge Articles/FAQs. The list area
   shows the available Knowledge content. You can preview an
   Article/FAQ by clicking on it.

4. Select an Article/FAQ that you want to link. Click on the **Link**
   button below. The Knowledge content gets linked to the Change. You
   can view the relationship in the **Relations** tab of the Change. In
   the same way, you can link multiple Articles/FAQs.

.. _cm-collaborate-schedule-and-planning:

Collaborate, Schedule and Planning
==================================

The :ref:`Details View <change-details-view>` of a Change gives the tools
for a Technician to collaborate with other Technicians; schedule a
timeline for the change process; and record planning details regarding
the change.

-  **Collaborate**: There are multiple stakeholders in a Change, and
   anyone with the Change update permission can start a conversation,
   keeping all of them in a loop.

    .. _cmf-26:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-26.png
        :align: center
        :alt: figure 26

   Under the **Collaborate** tab (:ref:`Details View <change-details-view>`),
   you get the options to add a **Collaborate** or **Note**. In either
   case, you get an editor where you put the message. Using @, you can
   direct the message to a specific person.

    .. _cmf-27:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-27.png
        :align: center
        :alt: figure 27

    .. _cmf-28:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-28.png
        :align: center
        :alt: figure 28

   Once a conversation is added, you cannot edit or delete it.

-  **Schedule**: Once a Change goes to the planning stage, the assigned
   Technician can schedule the entire change process. As an assigned
   Technician, you can enter a Start Time and End Time for the following
   sub-schedules:

    .. _cmf-29:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-29.png
        :align: center
        :alt: figure 29

    a. **Change Schedule**: It is the period of the entire Change process.

    b. **Down Time**: If the Change can cause an interruption in business
       processes, then you can mention the period of the same (requires you
       to first set the **Roll Out Schedule**).

    c. **Roll Out Plan**: It is the period for the actual implementation of
       the Change (requires you first set the **Change Schedule**).

-  **Planning**: As an assigned Technician, you can record the details
   of the Planning under three heads:

    .. _cmf-30:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-30.png
        :align: center
        :alt: figure 30

    a. **Impact**: Textual information about the effects of the Change in
       the Business.

    b. **Rollout Plan**: The detailed plan on how the Change is implemented.

    c. **Backout Plan**: A backup plan in case something goes wrong while
       commencing the Change.

.. _cm-adding-relations:

Adding Relations
================

Flotomate helps Technicians to build contextual information by building
relationships between various events in the system. The Relations tab in
the :ref:`Details View <change-details-view>` of a Change serves this
purpose.

The Relations tab gives you an option to create relationships between a
Change and other Changes, Requests, Problems, Knowledge Articles/FAQs,
and Assets.

.. _cmf-31:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-31.png
    :align: center
    :alt: figure 31

You can view the present relationships of the Change in **Relation
For**.

.. _cmf-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-32.png
    :align: center
    :alt: figure 32

You can create a new Request, Problem, Change or Asset and link it to an
existing Change using the **Create and Relate** button.

The **Add Relation** option lets you add one or more relationships.
Clicking **Add Relation** opens a pop-menu where you select what you
want to link (Request, Problem, Change (Change) or Asset). A dialog box
opens with a list of items and a search dialog box; the search bar
supports Advanced Search features where you can search for items with
predefined search options and keywords. You can perform a link by
selecting the items and clicking on **Link**.

.. _cmf-33:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-33.png
    :align: center
    :alt: figure 33

Approval in Change
==================

At the Approval stage, you might need an Approval from approver/approvers (multiple approvers can span across multiple Approvals) 
to move the Change to the next stage.

.. _cmf-34:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-34.png
    :align: center
    :alt: figure 34

.. _cm-different-states-in-an-approval-process:

Different States in an Approval Process
---------------------------------------

-  Approval:Pending

-  Approval:Rejected

-  Approval:Pre-Approved

-  Approval:Approved

.. _cm-manually-adding-approval:

Manually Adding Approval
------------------------

Clicking on **Add** (:numref:`cmf-34`) opens the Create an Approver dialog box.

.. _cmf-35:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-35.png
    :align: center
    :alt: figure 35

Using the dialog box, you can create an Approval with multiple
approvers. The assigned approvers get notified immediately. You can have
two types of Approval:

-  **Unanimous**: All of the approvers have to approve else the Approval
   is rejected.

-  **Majority**: If the majority of approvers agree then Approval is
   successful.

.. _cm-asking-for-approval:

Asking for Approval
-------------------

You can check whether an Approval Workflow is set or not by clicking on
**Ask For Approval**. An Approval Workflow has conditions based on that
approvers are automatically set. If conditions of a workflow are not
triggered or there’s no workflow (and manual Approvals) then the Change is Pre-Approved and the
Approval moves to next stage.

.. note:: Refer to Administration Manual to know more about Approval Workflows.
.. note:: A Change can have both manual and automatic Approvers.

.. _cm-approval-process:

Approval Process
----------------

-  Whether you create Approval manually or ask for Approval, once
   created it follows the same Approval process.

-  Technicians can view all the approvers, their statuses and comments
   under the Approvals tab.

    .. _cmf-36:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-36.png
        :align: center
        :alt: figure 36

   Once an Approval is set, the Approval status of the Change changes to
   **Pending** and it stays there as long as the approver/approvers don’t
   express a decision.

-  An approver can see his Approvals in the **My Approvals** section of
   his account.

    .. _cmf-37:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-37.png
        :align: center
        :alt: figure 37

   Clicking on **My Approvals** (:numref:`cmf-37`) opens the My Approval page
   where the approver can view his Approvals.

    .. _cmf-38:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-38.png
        :align: center
        :alt: figure 38

   Clicking on a Change Approval in **My Approval** opens a page with the
   title of the Approval as the header title and other details like:

    a. Change Details.
    b. Related Asset information.
    c. Planning details.
    d. Comment thread.
   
   Here the approver can perform the following actions:

    .. _cmf-39:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-39.png
        :align: center
        :alt: figure 39

    a. Review the details, schedule, related Assets, planning and comments
       of the Change.

    b. Start a comment thread which is visible to anyone having access to
       the comment section.

    c. Reject or Approve the Approval

-  The outcome of an Approval process is decided in two ways:

   a. **Unanimous**: All of the Approvers have to approve else the
      Approval is rejected.

   b. **Majority**: If the majority of Approvers agree then Approval is
      successful.

-  On success, the Approval moves to the Approved status and the Change
   goes to the next stage. On failure, the Approval moves to the
   Rejected status and the Change doesn’t move forward; you can put it
   back to the Planning stage, close it or re-initiate (Re-Approve) the Approval
   process.

.. _cmf-40:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-40.png
    :align: center
    :alt: figure 40

-  If a Technician has the :ref:`right <Technician Roles>` to ignore approvers (refer
   Administration Manual), then he can ignore non-responsive approvers
   and push the Approval towards Approved stage. An ignored approver can
   only see his status as Ignored in the Details View of the Change,
   because an approver cannot see the Approvals where he/she was ignored
   in his/her **MY Approvals** section.

   Ignoring all the approvers in an Approval changes the Approval status
   to Approved. The assigned Technician, only if he has the rights, can
   ignore an entire Approval using the **Re-Approve** option where a
   duplicate Approval is created and the original Approval is ignored.
   The Technician can also use the Re-Approve option to create duplicate
   Approvals in case he gets stuck in the Change Approval stage due to a
   rejection.

-  During an Approval process, the following things cannot be modified:

   a. Risk of the Change.

   b. Change Type.

.. _cm-managing-approvals-for-technician:

Managing Approvals for Technician.
----------------------------------

An assigned Technician can create multiple Approvals (manually) with the same
approvers or different ones; automatic Approval workflow can also create multiple Approvals. 
Between multiple Approvals, whether to go with unanimous or majority can be set from **Admin** (A Navigation Tab)
>> **Approval Workflow** (Automation) >> **Approval Settings**, but the
rights to do it lies with the Super Admin.

A Technician can send an email notification using the **Remind** button (refer: :numref:`cmf-41`) adjacent to an approver.

.. _cmf-41:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-41.png
    :align: center
    :alt: figure 41

Clicking on the Comment Icon in :numref:`cmf-41` opens the comment dialog box.
Anyone can comment as long as the dialog box is visible to them.

Related Topics:

-  :ref:`Understanding Approval Workflow`
-  :ref:`Creating an Approval Workflow`
-  :ref:`Allow Manual Approval`   

.. _cm-time-log:

Time Log
========

Once a Change moves to the Implementation stage, Technicians (including
the assigned Technician) working to implement the Change can log their
time spent working in the **Time Log** section.

.. _cm-adding-a-time-log:

Adding a Time Log:
------------------

1. Go to **Change** >> :doc:`List View <change-list-view>`.

2. Select a Change and go to its :ref:`Details
   View <change-details-view>`.

3. Scroll down to the **Time Log** tab and click on it.

.. _cmf-42:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-42.png
    :align: center
    :alt: figure 42

4. In Time Log tab, you can view all the logs, if any. Click on **Add**
   to add a new log. A dialog box opens.

.. _cmf-43:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-43.png
    :align: center
    :alt: figure 43

5. In the dialog box, enter a Start Date Time (e.g., Mon, Dec 11, 2017,
   5:12 PM) and an End Date Time (e.g., Mon, Dec 11, 2017, 10:10 PM),
   and hit **Add** to save your log.

Edit/Delete a Time Log:
-----------------------

1. Go to the :ref:`Details View <change-details-view>` of the Change.

2. Scroll down to **Time Log** tab and click on it. You can view all
   your logs under the tab.

.. _cmf-44:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-44.png
    :align: center
    :alt: figure 44

3. Perform edits using the Edit Icon adjacent to a log. Alternatively,
   you can delete them using the Delete Icon.

.. _cm-managing-tasks:

Managing Tasks
==============

Sometimes implementing a Change becomes a collaboration between multiple
Technicians; which is why the tool allows delegation of tasks from the
Details View of a Change.

Once a Change reaches the Implementation stage, you can create Tasks
related to the Change and assign them to Technicians. Assignees get
notified immediately.

.. note:: In order to work with Tasks in a Change. The Change has to have an assigned Technician.

.. _cmf-45:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-45.png
    :align: center
    :alt: figure 45

Adding a Task
-------------

Clicking on **Add Task** (:numref:`cmf-45`) in **Tasks** (in Details View)
opens the Add Task dialog box (:numref:`cmf-46`) where you can create and
assign n number of Tasks.

.. _cmf-46:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-46.png
    :align: center
    :alt: figure 46

A Task assignee sees his Task/Tasks on his Dashboard under **My Tasks**.

.. _cmf-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-47.png
    :align: center
    :alt: figure 47

**Edit/Delete a Task**

In the :ref:`Details View <change-details-view>`, the Tasks appear as a
list. There you can perform modifications to a Task and add notes (notes
are additional information).

.. _cmf-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-48.png
    :align: center
    :alt: figure 48

Anyone with the manage task rights can edit Tasks in a Change using the
edit icon. Same is true for deleting a Task using the delete icon
(:numref:`cmf-48`).

Adding a Note
-------------

Clicking on the note icon next to delete opens the Add Note dialog box.

.. _cmf-49:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-49.png
    :align: center
    :alt: figure 49

Here anyone with the manage task rights can add a note for all the
stakeholders to see. In the dialog box, click on **Add Notes** to add a
Note.

Closing a Task
--------------

Anyone with the manage task rights can go to the :ref:`Details
View <change-details-view>` and close a Task either by clicking on
**Done** or setting the Status of the Task to Closed.