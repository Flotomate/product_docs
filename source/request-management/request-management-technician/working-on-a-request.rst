********************
Working on a Request
********************

Once a Technician decides to work on a Request, he heads to the Details
View of the Request. There he/she uses the product features and tools to
resolve the Request.

Request Details View
====================

The Request Details view organizes and manages all information related
to a Request. Each Request has its own Details View having features that
Technicians use to resolve a Request.

To open the Details View

1. Go to :doc:`Request List View <request-list-view>`.

2. Scroll down to a Request that you want to open. Click on the name of
   the Request, which is adjacent to its ID. The Request Details View
   opens. Each Request has its own Details View.

The List View is a dynamic interface with the following features:

.. _rmf-16:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-16.png
    :align: center
    :alt: figure 16

-  Section-A houses the :ref:`Subject and Description <modifying-request-subject-and-description>`.

-  Section-B & C houses the :ref:`Classifiers <classify-requests>`.

-  Section-C also houses the :ref:`Search Knowledge
   Base <linking-knowledge-with-a-request>` feature.

-  Section-D houses five functions:

   a. :ref:`Work <communication-collaboration-and-resolution>`

   b. :ref:`Relations <add-relations>`

   c. :ref:`Approvals <rm-asking-for-approval>`

   d. :ref:`Custom Fields <ad-custom-fields>`

   e. :ref:`Time Log <rm-time-log>`

   f. :ref:`Notification <rm-notifications>`

-  Section-E is :ref:`Task <rm-managing-task>` column which is a sub-function
   of Work.

-  Section-F shows you the requester details.

-  Section-G houses the following options:

   a. :ref:`Close this Request <closing-from-details-view>`

   b. :doc:`Assignment options <assigning-a-request>`

   c. Action Menu:

      i.   :doc:`Mark as Spam <mark-a-request-as-a-spam>`

      ii.    :doc:`View Audit Trail <rm-viewing-audit-trail>`

      iii.   :ref:`Add Watcher <rm-watchers>`

      iv.  :ref:`Send Notification <rm-notifications>`

      v. Watch/Unwatch

      vi. :doc:`Send Feedback <asking-for-feedback>`

Modifying Request Subject and Description
=========================================

You can modify the Subject and Description of a Request. Below the
header title (section-A in :numref:`rmf-16`) shows the ID of the Request. Next
to the ID is the subject line of the Request. It is supposed to give you
a short description of the Request, and next to it is the Edit Icon for
editing the Subject and Description.

-  Go to the :ref:`Details View <request-details-view>` of the Request.

-  Click on the Edit Icon.

-  A dialog box opens. There you modify the Subject and Description and
   hit **Update**.

.. _rmf-17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-17.png
    :align: center
    :alt: figure 17

.. _rmf-18:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-18.png
    :align: center
    :alt: figure 18

Viewing Other Requests Created by the Requestor
===============================================

The product has the provision to view all other Requests created by the Requestor from the Details View
of a Request.

- Go to the :ref:`Details View <request-details-view>` of a Request
- Hover your mouse over the Requestor info section of the page.
- A pop-up menu opens where you can access other Requests.

.. _rmf-18.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-18.1.png
    :align: center
    :alt: figure 18.1

Classify Requests
=================

Flotomate provides many avenues to classify a Request. Go to the
:ref:`Details View <request-details-view>` of a Request, and there you get
the following ways:

.. _rmf-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-19.png
    :align: center
    :alt: figure 19

-  **Status**: Every Request has a life-cycle in the system. Setting the
   Status tag shows the stage at which the Request is in its life-cycle.
   There are seven Predefined statuses in the system: Open, In-Progress,
   Pending on Requester, Pending in Approval, Pending on Technician,
   Resolved and Closed. Other than In Progress, you cannot modify any of
   the predefined statuses.

   The status **Pending in Approval** is set automatically by the system
   whenever a Request goes through the Approval process. This status
   cannot be set manually.

   You can add custom statuses for which you need Admin rights. For
   example: you have a custom status called hold.

-  **Custom Tags**: These are additional tags that a Requester and
   Technicians can provide. This is a way to categorize a Request when
   default options are not enough. For example: you can add a tag
   Antivirus to all Requests related to antivirus renewal.

-  **Identified as Problem**: This label classifies the Request as
   having a related Problem. The Problems can be viewed in the
   **Relations** tab.

-  **Importance**: A Request can be categorized based on importance in
   the following ways:

   a. **Priority**: Setting this label shows the magnitude of the
      Request in the system. The Priority labels are system-defined. You
      can choose whether to set Priority manually or automatically using
      the Priority Matrix feature in Admin (refer Administration
      Manual).

   b. **Urgency**: Setting this label helps Technicians to ascertain the
      response time for the Request. These are predefined labels that
      are immutable, and they are Low, Medium, High, and Urgent.

   c. **Impact**: Setting this label shows where the Request has its
      effect which is either on User, Department or Business.

-  **Service Level Agreement**: SLA determines the Response Time and
   Resolution Time after considering Priority (others conditions in case
   of custom SLA). It also determines the escalated action when a time
   condition is violated. This generates the following data points about
   a Request.

   a. **SLA Status**: Tells whether any of the SLA conditions are
      violated or not.

   b. **Due-Date**: It reminds Technicians about the due date.

   c. **Estimated Time**: It tells the estimated time of resolution of
      the Request in minutes. A Technician can modify this, but it
      doesn’t changes the SLA conditions.

   d. **Support Level**: All Technicians are grouped into four Tiers
      based on their expertise and experience. Setting this tag shows
      which Tier the Request belongs.

   e. **Escalation Level**: This is the number of times escalated
      actions were taken based on SLA.

-  **Place**: A request can be classified based on the associated
   physical locations which are:

   .. note:: Below both fields have predefined values (as a drop-down list)
             set by the Administrator.

   a. **Department**: If the Request is related to a particular
      department, then this field is set to that department. A
      Technician can manually set the department field if needed.

   b. **Location**: If the Request is related to a particular location,
      then this field is set to that location.

-  **Source**: It shows the medium used to create the Request. The field is 
    automatically set by the server based on how it was created. 
    For example: all Requests created via email have the source set to
    Email.

-  **Category**: It is the primary method to categorize the Request.
   :doc:`Learn More <introduction-request-management>`.

-  **Technician Group**: The product allows grouping of Technicians into
   groups. Setting this field shows which group the Request belongs.

-  **Approval Status**: This classifies the Request based on the
   Approval stage. Learn more about
   :ref:`Approval <rm-different-states-in-an-approval-process>`.

-  **Reopen Count**: This label shows how many times the Request has
   been opened after getting close. The tag appears when a Request gets
   reopened for the first time.

Linking Knowledge with a Request
================================

It is crucial for a Technician to resolve a Request as fast as possible,
which is why information is made available through Knowledge in the
:ref:`Details View <request-details-view>`.

You can use the Search Knowledge to perform a search of the Knowledge.
You could find related information which you can link it with the
Request.

.. _rmf-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-20.png
    :align: center
    :alt: figure 20

Follow the detailed steps below to use the option:

-  Click on **Search Knowledge** opens a dialog box with a giant search
   bar.

-  Type your keyword in the search bar and press enter.

-  Matched Articles/FAQs populate below the search bar.

-  You can preview an Article/FAQ by clicking on it.

.. _rmf-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-21.png
    :align: center
    :alt: figure 21

-  Select an Article/FAQ and click on **Link**. To link multiple
   Articles/FAQs, you have to repeat the above process for each one.

You can view the related Articles/FAQs of a Request under the Relations
tab.

.. _rmf-22:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-22.png
    :align: center
    :alt: figure 22

Communication, Collaboration, and Resolution
============================================

Flotomate has functions that allow Technicians to gather information
through collaboration and communication and use it to resolve a Request.
The **Work** tab in the :ref:`Details View <request-details-view>` of a
Request has those functions.

.. _rmf-23:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-23.png
    :align: center
    :alt: figure 23

Work tab shows all the work and communication done for a Request. The
section is also referred to as Resolution section. In here you can
perform the following actions:

.. note:: Apart from Diagnosis, everything else is shown as part of a
          unified thread.

-  **Ask Requester**: You can directly communicate with the Requestor
   from the Details View using this option. Whatever you communicate
   gets added to a unified thread. The comments of the Requester also
   get added to the thread.

   The Requester gets an email notification on every message you post and vice-versa (Requestor and assigned Technician are the
   default recipients for email notification). The Requestor can reply to the emails and the replies are added to
   the comment thread.

   A Requestor can also comment in the Details View of a Request
   from the Customer Portal. Where he/she can specify a Technician’s
   name (other than the assigned Technician) as @tachnician_name in the 
   message body, and the mentioned Technician/Technicians get notified via email.

    .. _rmf-24:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-24.png
        :align: center
        :alt: figure 24
   
   Yon can use a template to insert a canned response in the text field. Click on **Insert from Template**
   , which opens a dialog box from where you can search and add a template. 

   .. _rmf-24.1:
   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-24.1.png
        :align: center
        :alt: figure 24.1

   Learn how to add a :ref:`Response Template<ad-response-template>`. 

-  **Collaborate**: You can collaborate with other Technicians. You can
   start a message thread which is visible to people who has access to
   the Technician Portal. You can notify a Technician my mentioning
   his/her name as @technician in the message body. This is an immutable
   action.

-  **Add Note**: This option allows you to add additional information
   about the Request so that others can view the same. You can attach
   files along with the textual information. This is an immutable
   action.

   Custom rules set by an administrator might ask you to add a Note
   while doing the following operations:

   a. Assigning a Request.

   b. Changing Department of a Request.

   c. Changing Category of a Request.

   d. Setting a new Due Date of a Request.

      Please refer the Administrator Manual to know more about Custom
      Rules for Requests.

Add Diagnosis
-------------

You can add a diagnosis statement in the :ref:`Details
View <request-details-view>` under **Work** tag.

.. _rmf-25:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-25.png
    :align: center
    :alt: figure 25

The Add Diagnosis option allows you to add an inspection of the related
problem. The Diagnosis statement sits on top of the pane with a
different color scheme. You can add only one Diagnosis statement per
Request. You can modify the diagnosis statement after adding one.

Add Solution
------------

You can add a Solution statement in the :ref:`Details
View <request-details-view>` under **Work** tag. You write your
solution in the **Add Solution** section. Along with textual
information, you can attach files and can even add links to Knowledge
posts.

.. _rmf-26:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-26.png
    :align: center
    :alt: figure 26

When you add a solution, you get a prompt asking you to resolve the
Request.

Yon can use a template to insert a canned response in the text field. Click on **Insert from Template**
, which opens a dialog box from where you can search and add a template.

.. _rmf-26.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-26.1.png
    :align: center
    :alt: figure 26.1

Learn how to add a :ref:`Response Template<ad-response-template>`.

Resolve Rules
-------------

Custom rules set by an administrator might prevent you from resolving a
Request unless you fulfill the set conditions. Rules are in regards to:

-  Minimum user interaction with the Request

-  Mandatory fields.

-  The state of the Request.

Please refer the Administrator Manual to know more about Custom Rules
for Requests.

Add Relations
=============

Flotomate helps Technicians to build contextual information by building
relationships between various items in the system. The **Relations** tab
in the ref`Details View <request-details-view>` of a Request serves this
purpose.

.. _rmf-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-27.png
    :align: center
    :alt: figure 27

The **Relations** tab gives you an option to create relationships
between a Request and other Requests, Problems, Changes, Knowledge
Articles/FAQs, and Assets.

.. _rmf-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-28.png
    :align: center
    :alt: figure 28

You can view the present connections of the Request by using the item
heads in **Relation For** section. You view the connections as a list.

You can create a new Request, Problem, Change or Asset and link it to
the Request using the **Create and Relate** option.

The **Add Relation** option lets you add one or more relationships with
existing Requests, Problems, Changes and Assets.

-  Clicking on **Add Relation** shows you a popup menu where you have to
   select either Request, Problem, Change or Asset.

-  A dialog box opens with a search box (it supports Advanced Search
   features)

-  Search for the right entry and click **Link** to add a relationship
   between your selection/selections and the Request.

.. _rm-time-log:
Time Log
========

Once a Technician gets assigned to a Request, he along with other
Technicians can log their time spent working on the Request in the Time
Log section of the Request.

Adding a Time Log
-----------------

1. Go to the :ref:`Details View <request-details-view>` of the Request.

2. Scroll down to the **Time Log** tab next to **Approvals** and click
   it.

    .. _rmf-29:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-29.png
        :align: center
        :alt: figure 29

3. Click on **Add** to add a new log.

    .. _rmf-30:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-30.png
        :align: center
        :alt: figure 30

4. Enter a Start Date Time (e.g., Mon, Dec 11, 2017, 5:12 PM), an End
   Date Time (e.g., Mon, Dec 11, 2017, 10:10 PM) and a description, and hit **Add** to
   save your log.

How to Edit/Delete Time Log:
----------------------------

1. Go to the :ref:`Details View <request-details-view>` of the Request.

2. Scroll down to the **Time Log** tab. Click on the tab, and you see
   the time logs as a list.

    .. _rmf-31:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-31.png
        :align: center
        :alt: figure 31

3. Perform edits using the Edit Icon adjacent to a log. Alternatively,
   you can delete them using the Delete Icon.

Custom Fields
=============

Custom fields are additional fields that appear on the Create a
Request form (both Technician and Customer Portal) and the
Details View of Requests. You can create such fields from the Admin
section.

A field can be made compulsory in a particular status. For example, we
created a field called employee ID and made it compulsory for the status
**Open**; so anyone changing Status from **Open** to any other has to
make sure the Employee ID is not empty.

Inputted values in the Custom field is shown in the :ref:`Details
View <request-details-view>` of a Request under Custom Fields tab.

.. _rmf-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-32.png
    :align: center
    :alt: figure 32

.. _rm-asking-for-approval:

Asking for Approval
===================

This is an option a Technician assigned to a Request can utilize to seek
approvals from others before resolving or closing a Request. The
Approval process is a mechanism for control that ensures Technicians
don’t commit unauthorized actions.

Custom rules, set by someone with Admin rights, decide whether taking
Approval is necessary or not before resolving or closing a Request.

Initiating an Approval
----------------------

.. note:: You need to be the assigned Technician in order to start the
          Approval process.

1. Go to the :ref:`Details View <request-details-view>` of a Request.

2. Scroll down to the **Approval** tab and click it.

.. _rmf-33:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-33.png
    :align: center
    :alt: figure 33

3. Click on **Ask for Approval** to initiate the Approval process.

.. _rm-different-states-in-an-approval-process:
Different States in an Approval Process
---------------------------------------

-  Approval Pending:

-  Approval Rejected:

-  Approval Pre-Approved:

-  Approval Approved:

Managing Approval
-----------------

An assigned Technician can view all his Approvals under the Approvals
tab. The Approvals tab shows two columns: the Approvals column which
lists all the Approvals along with their approvers, and the Comments
column that shows the message thread between Technicians and approvers.
Any Technician with the necessary rights can access the Approvals tab of
a Request.

.. _rmf-34:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-34.png
    :align: center
    :alt: figure 34

An assigned Technician can create multiple Approvals with the same
approvers or different ones. Between multiple Approvals, whether to go
with unanimous or majority can be set from **Admin** (A Navigation Tab)
>> **Approval Workflow** (Automation) >> **Approval Settings**, but the
rights to do it lies with the Super Admin.

.. _rmf-35:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-35.png
    :align: center
    :alt: figure 35

Approval Process
----------------

-  When an Approval process is initiated, first the system changes the
   Request status to **Pending in Approval** and then checks for
   available Approval Workflows. If there are no workflows, then the
   Request is pre-approved, and the Approval status is changed to
   **Pre-Approved** and Request status is changed to Pending on
   Technician. If there is a workflow, then based on its set conditions
   approver/approvers are auto-assigned for approval.

   .. note:: Refer to Administration Manual to know more about Approval
             Workflows.

-  You can view all the approvers, their statuses and comments in the
   Approvals tab.

    .. _rmf-36:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-36.png
        :align: center
        :alt: figure 36

   Once an Approval is set, the Approval status of the Request changes to
   **Pending,** and it stays there as long as the approver/approvers don’t
   express a decision.

-  An approver can see his Approvals in the **My Approvals** section of
   his account.

    .. _rmf-37:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-37.png
        :align: center
        :alt: figure 37

   Clicking on **My Approvals** (:numref:`rmf-37`) opens the My Approval page
   where he can view his Approvals.

    .. _rmf-38:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-38.png
        :align: center
        :alt: figure 38

   Clicking on a Request Approval in **My Approval** opens a page with the
   title of the Approval as the header title. There he can perform the
   following actions:

    .. _rmf-39:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-39.png
        :align: center
        :alt: figure 39

    a. Review the details and comments on the Request.

    b. Start a comment thread which is visible to anyone having access to
       the comment section.

    c. Reject or Approve the Approval.

-  The outcome of an Approval process is decided in two ways:

    a. **Unanimous**: All of the Approvers have to approve else the
       Approval is rejected.

    b. **Majority**: If the majority of Approvers agree then Approval is
       successful.

-  On success, the Approval moves to the Approved status and the Request
   status changes to Pending on Technician. On failure, the Approval
   moves to the Rejected status and Request status changes to Pending on
   Technician; the assigned Technician has to reinitiate the Approval
   process.

.. _rmf-40:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-40.png
    :align: center
    :alt: figure 40

-  If a Technician has the right to ignore approvers (refer
   Administration Manual), then he can ignore non-responsive approvers
   and push the Approval towards the Approved stage. An ignored approver
   can see his status as Ignored in the Details View of the Request. An
   approver cannot see the Approvals where he/she was ignored in his/her
   **MY Approvals** section.

   Ignoring all the approvers in an Approval changes the Approval status
   to Approved. A Technician can ignore or reinitiate an Approval using
   the **Re-Approve** option where a duplicate Approval is created, and
   the original Approval is ignored. You can Re-Approve an already
   Approved Approval; in that case, you can manually set the Request
   status to Pending in Approval.

.. _rmf-41:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-41.png
    :align: center
    :alt: figure 41

-  During an Approval process, the following things cannot happen:

   a. SLA cannot run during an Approval process. It stays paused still
      Approval is approved.

   b. Location, Category, and Department cannot be modified.

.. _rm-managing-task:
Managing Task
=============

Sometimes resolving a Request becomes a collaboration between multiple
Technicians; which is why the product allows delegation of tasks from
the Details View of a Request.

Any Technician can assign Tasks to other Technicians related to any
Request if he has manage Task rights. An assignee can see his Task/Tasks
on his Dashboard.

.. _rmf-42:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-42.png
    :align: center
    :alt: figure 42

Adding a Task
-------------

-  Go to the :ref:`Details View <request-details-view>` of a Request.

-  Click **Add Task** in the Task column under **Work** tab. The Add
   Task dialog box opens.

.. _rmf-43:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-43.png
    :align: center
    :alt: figure 43

-  Give a suitable title that describes the Task. Select an assignee
   from the drop-down list in the **Assignee User** field.

-  Set a time-frame (Start Date Time and End Date Time), Priority, and
   Description for the task and hit **Create**.

Editing/Deleting Tasks
----------------------

-  Go to the Request’s Task Column.

.. _rmf-44:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-44.png
    :align: center
    :alt: figure 44

-  You can see all created Tasks. You can edit a Task using the Edit
   Icon and delete a Task using the Delete Icon. Perform the action you
   want.

Adding Note to a Task
---------------------

.. _rmf-45:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-45.png
    :align: center
    :alt: figure 45

-  Go to the Request’s Task Column.

-  Click on the Note Icon of a Task.

.. _rmf-46:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-46.png
    :align: center
    :alt: figure 46

-  Add your note in the text editor. You can upload files along with the
   text.

Closing a Task
--------------

-  Go to the Details View of the Request. The assignee of the Task can
   directly go to the Details View by clicking on the Task title on his
   Dashboard.

-  Scroll down to the Task Column. You can close a Task by clicking on
   **Done** or changing the Status to Closed. Anyone with the necessary
   rights can perform this operation.

.. _rmf-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-47.png
    :align: center
    :alt: figure 47

.. _rm-notifications:
Notifications
=============

The scope of a Request is broad in terms of stakeholders involved;
communication plays a crucial role to make sure everyone is aware of the
progress happening with the resolution process. Here bulk Notification
features come handy to communicate with all stakeholders effectively and
efficiently.

 Sending a Notification:
------------------------

1. Since Notifications are Request specific, you have to go to the
   :ref:`Details View <request-details-view>` of a Request.

2. In the Details View, click on the Action Menu and select **Send
   Notification** from the pop meu.

.. _rmf-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-48.png
    :align: center
    :alt: figure 48

3. Clicking on **Send Notification** opens a dialog box.

    .. _rmf-49:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-49.png
        :align: center
        :alt: figure 49

    a. Now choose the audience who receives your notification. You can
       select individuals or groups, be it Requesters or Technicians, or
       both. You can add multiple emails using the **Add Email** (section-A
       in :numref:`rmf-49`) button.

    b. Request specific details are there in the Subject and Body. You can
       edit the Subject and Body if you want. Make all the changes and hit
       **Send**. Now you have successfully sent a Notification.

Viewing Notification
--------------------

A Technician can view all his Notifications that he created under
**Notifications** tab in the :ref:`Details View <request-details-view>`.
Click on a Notification to get more details.

.. _rmf-50:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-50.png
    :align: center
    :alt: figure 50

System Defined Request Notifications
------------------------------------

Flotomate has 13 Notifications that are predefined and generated
automatically. They can be turned on by an Admin. The Notifications are
as follows:

-  Notify ticket agent when Approver rejects an Approval.

-  Notify ticket agent when Approver approves an Approval.

-  Notify Approver when Approval is created.

-  Notify Approvers and ticket agent when a new comment is added to the
   Approval.

-  Acknowledge Requester when Request is reported.

-  Notify Technician when a Task is assigned.

-  Notify Requester when a Request is closed.

-  Notify Requester when Request is resolved.

-  Notify Technicians when they are mentioned in the conversation for a
   Request.

-  Notify Requester when Technician attaches solution for a Request.

-  Notify Requester when Technician reply to Requester for a Request.

-  Notify Technicians in a Group when Request is assigned to that Group.

-  Notify Technicians when a Request is assigned.

.. note:: Only an Admin can modify the content of the above-predefined
          Notifications.

.. _rm-watchers:
Watchers
========

In a Request, it is likely that multiple stakeholders want to keep a
watch so that necessary actions are taken promptly. With the Watch
feature, one can subscribe to a specific Request and receive
notifications that go to the Requestor.

Watchers of a Request are the default contact people for Notifications.
Their names are added by default whenever a technician creates a
Notification.

Adding/Editing People as Watchers
---------------------------------

1. Go to the :ref:`Details View <request-details-view>` of a Request.

2. In the Details View, click on the Action Menu and select **Add
   Watcher** from the popup menu.

.. _rmf-51:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-51.png
    :align: center
    :alt: figure 51

3. **Add Watcher** dialog box opens. You can add people individually
   using their email addresses, or you can add groups available under
   Technician and Requestor, or you can use both emails and groups.

.. _rmf-52:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-52.png
    :align: center
    :alt: figure 52

4. Add your watchers and save your changes before exiting.

5. Later you can use the **Add Watcher** dialog box to add/remove
   Watchers.

How a Technician can add Himself as a Watcher:
----------------------------------------------

A Technician can be a Watcher too with a single click.

1. Head to the :ref:`Details View <request-details-view>` of a Request.

2. Click on **Watch** in the Action Menu next to Assignment options,
   and you become a Watcher.

.. _rmf-53:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-53.png
    :align: center
    :alt: figure 53

3. Click **Unwatch** in the Action Menu to unwatch the Request.

Jira Integration
================

If you have Jira integrated with Flotomate, then you can directly add a
Request to Jira from the product.

To add a Request:

-  Go to the :ref:`Details View <request-details-view>` of a Request that
   you want to add.

-  The Integrations tab appears in all Requests when you have Jira
   integrated. Go to the Integrations tab.

.. _rmf-54:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-54.png
    :align: center
    :alt: figure 54

-  Click on **Add to Jira**. A new dialog box opens.

.. _rmf-55:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-55.png
    :align: center
    :alt: figure 55

-  Set Project, Issue Type, and Priority. Subject and Description are
   fetched from the Request. Click **Add** to begin the import.

Closing a Request
=================

Flotomate gives you multitude of ways to close a Request which are as
follows:

Closing from List View:
-----------------------

1. Go to **Request** >> :doc:`Request List View <request-list-view>`.

2. Click on the Status of a Request and change it to Closed. The
   Request is now marked as closed.

.. _rmf-56:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-56.png
    :align: center
    :alt: figure 56

Closing from Details View:
--------------------------

1. Go to the :ref:`Details View <request-details-view>` of a Request.

2. There you can change the Status to close. If the Request is assigned
   to someone, then you can use the **Close this Request** option for
   closure.

.. _rmf-57:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-57.png
    :align: center
    :alt: figure 57

Closure Rules
-------------

An Admin might set rules that prevent you from closing a Request unless
you fulfill certain set conditions. Such conditions can be grouped under
three heads:

-  User interaction

-  Mandatory Fields

-  Required State

To know more about Closure Rules refer to the Administration Manual.