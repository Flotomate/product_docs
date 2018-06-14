**********************************
Request Management for Technicians
**********************************

Creating a Request 
==================

Technicians can create Requests using the email to ticket feature and
the Create a Request dialog box.

The Create a Request dialog box is available on both the Requestor and
Technician Portal. However, the Create a Request form on the Technician
portal is different. It has additional fields that are specific to the
needs of the Technicians.

Only people with create Request rights can create Requests. Please refer
Roles (Users) in the Administration Manual.

1. Log in to the Technician Portal. Hover your mouse over the **Create**
   button in one of the Navigation Tabs. You see a popup menu; click on
   **Request**.

.. _rmf-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-1.png
    :align: center
    :alt: figure 1

2. The **Create-a-Request** dialog box opens.

.. _rmf-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-2.png
    :align: center
    :alt: figure 2

.. _rmf-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-3.png
    :align: center
    :alt: figure 3

3. You have to set a Request Category in section-A (:numref:`rmf-2`). It is a
   way to categorize Requests. The product has two predefined Categories
   (:ref:`Incident and Service Requests <what-is-a-request>`) to choose
   from, and you can add more categories. Each category can have
   Sub-Categories, up to three levels. Please refer Request Category
   (Helpdesk) in the Administration Manual to learn how to add
   Categories and Sub-Categories.

   The dialog box highlights the selected Category in the Category field
   in section-B (:numref:`rmf-2`).

4. You can fill the form using a template which is a quicker way to
   submit Requests that are recurring or part of a Service Request
   catalog. Section-B has the field that lets you populate the form from
   a custom template.

   You can manage custom templates from **Request Templates** (Helpdesk)
   in **Admin**. Please refer the Administration Manual on how to add
   templates.

   .. note:: The person who creates Templates must have administrative rights.

   Loading a custom Template (if any) performs the following changes:

   a. It populates the Subject of the Request.

   b. It configures the following classifiers of the Request:

      i.   Priority of the Request.

      ii.  Urgency level of the Request.

      iii. Impact of the Request on the organization.

   c. It can add Tags to the Request.

   d. It can add a Description.

5. In section-C, you need to add the Requestor email and name (Requestor
   Email ID and Requestor Name). You cannot create a Request with an
   unauthenticated email. You have to ask an Administrator to enable
   Request creation without login to do so.

   You can add other emails using **Add Cc Email**. That adds them to
   the Watcher list, which means they get notifications that the
   Requestor gets.

6. In section-D, you add the Subject line that gives a brief
   introduction to the Request. If you use a Template, the field
   auto-populates. Else, you have to fill it yourself because it is a
   mandatory field.

7. In section-E, you set the Status, Priority, Urgency, and Impact. This
   data is vital for tracking and managing Requests.

   If you are not using a template, then you have to set them manually
   according to your requirements.

   Tags are optional identifiers that you can add. You can add multiple
   tags if you want.

8. Section-F is the Description area where you write a detailed
   explanation of the Request. It should talk about the symptoms that
   lead to the Request. You can attach additional documents to support
   the resolution process in section-H.

9. In section-G&H, you can add Technician Group, Location, and
   Department. These fields have a drop-down list of values predefined
   by an Administrator; you just need to select the appropriate values.

   Please refer the Administration Manual to know more about the fields.

10. Hit **Create** when you are done filling the form. Now you have
    successfully created your Request. An email is sent to the Requester
    acknowledging the Request.

**Email to ticket**

Flotomate gives the option to set up an email as the Helpdesk email
address. Technicians can send an email to create a Request.

The question, who can create a Request, depends on the **Helpdesk**
settings in the **Admin** section. If settings allow creating Requests
without login, then anyone with the Helpdesk email can create a Request.
Else, the system accepts email Requests from registered emails only.

When a Technician creates a Request using an email, the email subject
becomes the Request Subject, email body becomes the Request Description,
and any attachments become the Request attachment.

Request List View
=================

The Request interface is divided into two parts: Request List View and
the Request Details View. The Request List View allows **Technicians**
to track and manage all Requests at one place.

In the Request List View, users get to see all the available Requests in
the system. It is the central hub for a Technician, where he/she finds a
Request and acts upon it.

To open Request List View:

1. Log in to Flotomate through the Technician Portal.

2. Click on **Request** (A Navigation Tab) to open the Request List
   View, or you can hover your mouse over **Request**; you get a popup
   menu. Click on **All Open Request** to view the list of all the
   available Requests in the List View.

.. _rmf-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-4.png
    :align: center
    :alt: figure 4

The List View is dynamic with the following features:

.. _rmf-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-5.png
    :align: center
    :alt: figure 5

-  Section-A, B, C, & D are the :ref:`search
   features <searching-requests>` of the UI.

-  Section E houses the bulk operations which are:

   a. :ref:`Bulk Update <request-bulk-update>`

   b. :ref:`Merge <merge-requests>`

   c. :ref:`Mark as Spam <mark-a-request-as-a-spam>`

   d. :ref:`Archive <deleting-a-request>`

   e. :ref:`Claim <assigning-a-request>`

   f. :ref:`Assign <assigning-a-request>`

-  Section-F is the actual list area listing all the Requests with the
   following information:

    .. _rmf-6:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-6.png
        :align: center
        :alt: figure 6

    a. :ref:`Classifiers <classify-requests>` (Status, Priority, Due Date)

    b. Assignee information or :ref:`Claim and Assign
       buttons <assigning-a-request>`. Next to them is the Action
       Menu having the following options:

        i.   Mark as Spam

        ii.  View Audit Trail

        iii. Open In New Window

    c. Requester info and Create time of the Request.

-  Section-G is the Details Pane section that shows you some
   :ref:`classifiers <classify-requests>`. You also have two tabs:

    a. **Details**: It shows the Requester info and Create Time of the
       Request

    b. **Activity**: It shows the :ref:`Audit Trail <rm-viewing-audit-trail>`
       of the Request.

-  Section-H gives you the option to set the number of Requests visible
   per page; the highest is 100 per page.

   You can toggle between Detailed View and Glance View.

    a. In Detailed View, the listings are more descriptive and explicit
       compared to List View. You can view additional information in the
       Details Pane of a Request.

        .. _rmf-7:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-7.png
            :align: center
            :alt: figure 7

    b. Glance View is minimalist which shows minimum information. The
       focus is to give you the most critical information.

.. _rmf-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-8.png
    :align: center
    :alt: figure 8

-  Section-I is the :ref:`Manage Announcements <announcements>` option.

Searching Requests
==================

Flotomate gives you two broad ways to search Requests in :ref:`Request List
View <request-list-view>`.

-  Using custom and predefined filters.

-  Using a search bar.

Using a Search Bar
------------------

The product allows you to perform Advanced Search using various
combinations of predefined search options and keywords. If you want to
see the list of available options, then click on the Search Box. You can
select an option or multiple options from a drop-down menu.

.. _rmf-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-9.png
    :align: center
    :alt: figure 9

You can search Requests with keywords. When you provide a keyword,
Flotomate examines all the Requests with the keyword in Subject,
Description, Solution, Tags, Requestor Email, and ID fields. All matched
Requests get displayed in the list area. In case of multiple keywords,
all keywords need to be matched.

You can make a filter using a chain of search options and keywords. You
can save your search queries, refer :numref:`rmf-10`. Saved search queries
appear in the section-A’s menu list (:numref:`rmf-5`).

For example, if you are looking for all Requests containing the word SLA
in the Subject line and have an Impact on a Department. You have the
search query in :numref:`rmf-10`.

.. _rmf-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-10.png
    :align: center
    :alt: figure 10

Between two different conditions of the same data type, the OR logic
prevails. Between different data, types, the AND logic prevails. An
example of same data type conditions is Status Open vs. Status Closed.
Between keywords and conditions AND logic is followed.

.. _rmf-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-11.png
    :align: center
    :alt: figure 11

Using Filters
-------------

The product has filters to sort Requests List using the following
criteria:

-  Status

-  Priority

-  Assignee

-  SLA

Go to the :ref:`Request List View <request-list-view>`. In the List View,
clicking on the header section (Section-A :numref:`rmf-5`) gives you a popup
menu containing seven predefined filters.

.. _rmf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-12.png
    :align: center
    :alt: figure 12

Selecting any one filter populates the list area with Requests
satisfying the filter’s conditions. All seven filters have different
conditions, which are:

+-----------------------------------+-----------------------------------+
| All Open Request                  | It shows all the Unclosed         |
|                                   | Requests available in the system. |
+-----------------------------------+-----------------------------------+
| My Unresolved Request             | It includes all the unclosed,     |
|                                   | unresolved Requests assigned to   |
|                                   | you.                              |
+-----------------------------------+-----------------------------------+
| My Urgent or High Priority        | It includes all the unclosed,     |
| Request                           | unresolved Requests assigned to   |
|                                   | you with either High or Urgent    |
|                                   | priority.                         |
+-----------------------------------+-----------------------------------+
| My Overdue Request                | Includes all the unclosed,        |
|                                   | unresolved Requests assigned to   |
|                                   | you that are past their due date. |
+-----------------------------------+-----------------------------------+
| Urgent or High Priority Request   | It includes all the unresolved,   |
| in My Group                       | unclosed Requests with either     |
|                                   | High or Urgent priority and with  |
|                                   | a Technician Group that you are   |
|                                   | part of.                          |
+-----------------------------------+-----------------------------------+
| Unassigned Request in My Group    | It includes all the open,         |
|                                   | unassigned Requests with a        |
|                                   | Technician Group that you are     |
|                                   | part of.                          |
+-----------------------------------+-----------------------------------+
| All Un-analysed Request            | It shows all the Requests without |
|                                   | a Diagnosis.                      |
+-----------------------------------+-----------------------------------+

There are status based filters in Section-B (:numref:`rmf-5`) of List View that
tell you about the distribution of Requests under various predefined and
custom statuses.

.. _rmf-13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-13.png
    :align: center
    :alt: figure 13

You can create and manage custom statuses, but you cannot change some
statuses, which are:

-  Open

-  Pending on Requester

-  Pending in Approval (This :ref:`status <classify-requests>` can only be set by
   the system when the Request is in the :ref:`Approval <request-asking-for-approval>` stage.)

-  Pending on Technician

-  Resolved

-  Closed

Please refer Request Custom Status (Customization and Configuration) in
the Administration manual to learn how to create Custom Statuses.

The product can also show you the distribution of all the unclosed
Requests across the priority levels and SLA statuses.

.. _rmf-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-14.png
    :align: center
    :alt: figure 14

Additional tags appear when one or more Requests are about to reach
their Due-dates. The maximum time-frame to show due is 24 hours.

Assigning a Request
===================

Assigning a Request to a Technician makes that person responsible for
the Request. He/she becomes the point of contact for all matters related
to the Request. An assigned Technician has the privilege to initiate an
Approval process when required.

A Technician, with the necessary Request rights, can assign a Request to
other Technicians or claim it for himself/herself.

Assigning from List View
------------------------

1. Go to **Request** >> :ref:`Request List View <request-list-view>`.

2. Hover your mouse over the Request that you want to claim or assign.
   The **Claim** and **Assign** buttons appear. Perform the operation
   that you want.

   Selecting **Claim** assigns the Request to you, and you can view your
   name against the Request Subject line.

   You can assign the Request to other Technicians. Selecting **Assign**
   pops up a list where you can see the names of other Technicians along
   with colored rings showing the workload of each Technician. Red
   represents maximum load and green, minimum load.

Alternatively, you use Claim and Assign as a bulk operation. You can
Claim or Assign multiple Requests at once.

.. _rmf-15:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-15.png
    :align: center
    :alt: figure 15

Assigning from Details View
---------------------------

1. Go to **Request** >> Request List View.

2. Click on a Request and go to its :ref:`Details View <request-details-view>`.

3. You can find the **Claim** and **Assign** button in the top right
   corner. Perform the action that you want.

Working on a Request
====================

Once a Technician decides to work on a Request, he heads to the Details
View of the Request. There he/she uses the product features and tools to
resolve the Request.

Request Details View
--------------------

The Request Details view organizes and manages all information related
to a Request. Each Request has its own Details View having features that
Technicians use to resolve a Request.

To open the Details View

1. Go to :ref:`Request List View <request-list-view>`.

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

   c. :ref:`Approvals <request-asking-for-approval>`

   d. :ref:`Time Log <request-time-log>`

   e. :ref:`Notification <rm-notifications>`

-  Section-E is :ref:`Task <rm-managing-task>` column which is a sub-function
   of Work.

-  Section-F shows you the requester details.

-  Section-G houses the following options:

   a. :ref:`Close this Request <closing-from-details-view>`

   b. :ref:`Assignment options <assigning-from-details-view>`

   c. Action Menu:

      i.   :ref:`Mark as Spam <mark-a-request-as-a-spam>`

      ii.    :ref:`View Audit Trail <rm-viewing-audit-trail>`

      iii.   :ref:`Add Watcher <rm-watchers>`

      iv.  :ref:`Send Notification <rm-notifications>`

      v. Unwatch

Modifying Request Subject and Description
-----------------------------------------

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

Classify Requests
-----------------

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

-  **Source**: It shows the medium used to create the Request. For
   example: all Requests created via email can have the source set to
   Email.

-  **Category**: It is the primary method to categorize the Request.
   :ref:`Learn More <what-is-request-management>`.

-  **Technician Group**: The product allows grouping of Technicians into
   groups. Setting this field shows which group the Request belongs.

-  **Approval Status**: This classifies the Request based on the
   Approval stage. Learn more about
   :ref:`Approval <rm-different-states-in-an-approval-process>`.

-  **Reopen Count**: This label shows how many times the Request has
   been opened after getting close. The tag appears when a Request gets
   reopened for the first time.

Linking Knowledge with a Request
--------------------------------

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
--------------------------------------------

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

   The Requester gets an email notification on every message you post.
   The Requestor can reply to the emails and the replies are added to
   the comment thread in the **Work** tab.

   A Requestor can directly comment in the Details View of a Request
   from the Customer Portal. Where he/she can specify a Technician’s
   name as @tachnician_name in the message body. The mentioned
   Technician gets notified via email.

.. _rmf-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-24.png
    :align: center
    :alt: figure 24

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

**Add Diagnosis**
^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^

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

Resolve Rules
^^^^^^^^^^^^^

Custom rules set by an administrator might prevent you from resolving a
Request unless you fulfill the set conditions. Rules are in regards to:

-  Minimum user interaction with the Request

-  Mandatory fields.

-  The state of the Request.

Please refer the Administrator Manual to know more about Custom Rules
for Requests.

Add Relations
-------------

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

.. _request-time-log:
Time Log
--------

Once a Technician gets assigned to a Request, he along with other
Technicians can log their time spent working on the Request in the Time
Log section of a Request.

Adding a Time Log
^^^^^^^^^^^^^^^^^

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

4. Enter a Start Date Time (e.g., Mon, Dec 11, 2017, 5:12 PM) and an End
   Date Time (e.g., Mon, Dec 11, 2017, 10:10 PM), and hit **Add** to
   save your log.

How to Edit/Delete Time Log:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
-------------

Custom fields are additional fields that can appear on the Create a
Request form (both Technician and Customer Portal) or solely on the
Details View of Requests. You can create such fields from the Admin
section.

A field can be made compulsory in a particular status. For example, we
created a field called employee ID and made it compulsory for the status
**Open**; so anyone changing Status from **Open** to any other has to
make sure the Employee ID is not empty.

Inputted values in the Custom field is shown in the :ref:`Details
View <request-details-view>` of a Request.

.. _rmf-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-32.png
    :align: center
    :alt: figure 32

.. _request-asking-for-approval:
Asking for Approval
-------------------

This is an option a Technician assigned to a Request can utilize to seek
approvals from others before resolving or closing a Request. The
Approval process is a mechanism for control that ensures Technicians
don’t commit unauthorized actions.

Custom rules, set by someone with Admin rights, decide whether taking
Approval is necessary or not before resolving or closing a Request.

Initiating an Approval
^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

-  Approval Pending:

-  Approval Rejected:

-  Approval Pre-Approved:

-  Approval Approved:

Managing Approval
^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^

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
-------------

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
^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^^^

-  Go to the Request’s Task Column.

.. _rmf-44:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-44.png
    :align: center
    :alt: figure 44

-  You can see all created Tasks. You can edit a Task using the Edit
   Icon and delete a Task using the Delete Icon. Perform the action you
   want.

Adding Note to a Task
^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^

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
-------------

The scope of a Request is broad in terms of stakeholders involved;
communication plays a crucial role to make sure everyone is aware of the
progress happening with the resolution process. Here bulk Notification
features come handy to communicate with all stakeholders effectively and
efficiently.

 Sending a Notification:
^^^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^

A Technician can view all his Notifications that he created under
**Notifications** tab in the :ref:`Details View <request-details-view>`.
Click on a Notification to get more details.

.. _rmf-50:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-50.png
    :align: center
    :alt: figure 50

System Defined Request Notifications
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
--------

In a Request, it is likely that multiple stakeholders want to keep a
watch so that necessary actions are taken promptly. With the Watch
feature, one can subscribe to a specific Request and receive
notifications that go to the Requestor.

Watchers of a Request are the default contact people for Notifications.
Their names are added by default whenever a technician creates a
Notification.

Adding/Editing People as Watchers
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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
----------------

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
-----------------

Flotomate gives you multitude of ways to close a Request which are as
follows:

Closing from List View:
^^^^^^^^^^^^^^^^^^^^^^^

1. Go to **Request** >> :ref:`Request List View <request-list-view>`.

2. Click on the Status of a Request and change it to Closed. The
   Request is now marked as closed.

.. _rmf-56:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-56.png
    :align: center
    :alt: figure 56

Closing from Details View:
^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Go to the :ref:`Details View <request-details-view>` of a Request.

2. There you can change the Status to close. If the Request is assigned
   to someone, then you can use the **Close this Request** option for
   closure.

.. _rmf-57:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-57.png
    :align: center
    :alt: figure 57

Closure Rules
^^^^^^^^^^^^^

An Admin might set rules that prevent you from closing a Request unless
you fulfill certain set conditions. Such conditions can be grouped under
three heads:

-  User interaction

-  Mandatory Fields

-  Required State

To know more about Closure Rules refer to the Administration Manual.

Mark a Request as a Spam
========================

It may happen that some Requests that you receive are irrelevant, and
you want them disappear. You can discard a Request as a Spam, and it
disappears from the product. You can mark multiple Requests as Spam at
once or mark them individually.

.. _rmf-58:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-58.png
    :align: center
    :alt: figure 58

1. Go to **Request** >> :ref:`Request List View <request-list-view>`.

2. Select a Request or Requests from the list area. The **Mark as
   Spam** option appears.

3. Clicking **Mark as Spam** sends the selected Requests to spam. Else
   you can mark then individually by selecting **Mark as Spam** from the
   Action Menu of a Request.

You can also send Requests to spam from the Request Details View:

1. Go to a Request’s Detail View.

2. Click on the Action Menu.

.. _rmf-59:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-59.png
    :align: center
    :alt: figure 59

3. Click **Mark as Spam** to send the Request to spam.

Viewing/Unspam a Spammed Requests
---------------------------------

1. Go to **Requests** >> :ref:`Request List View <request-list-view>`.

2. Click on the Search Box.

3. Select **Spam equals** >> **Yes**.

   You would see all the Spam Requests in the list area. You can Unspam
   them by selecting **Mark as Unspam** from the Action menu of a
   spammed Request. You can also Unspam multiple Requests in the same
   way you Spammed them.

    .. _rmf-60:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-60.png
        :align: center
        :alt: figure 60

   You can also find the **Mark as Unspam** option in the Details View of a
   Spammed Request. It is in the Action Menu of a Request.

.. _rm-viewing-audit-trail:
Viewing Audit Trail
===================

The Audit Trail dialog box lists most changes concerning assignment, and
:ref:`classifiers <classify-requests>` of a Request.

1. Go to **Request** >> :ref:`Request List View <request-list-view>`.

2. Select the Request whose **Audit Trail** you want to see.

3. Click on the Action Menu next to Assign/Name-of-Assignee, and click
   **View Audit Trail**. The Audit Trail dialog box opens, and you can
   search and sort the Audit Trail information.

.. _rmf-61:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-61.png
    :align: center
    :alt: figure 61

Alternatively, the Audit Trail is also visible under the Activity tab.

.. _rmf-62:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-62.png
    :align: center
    :alt: figure 62

Another way to view Audit Trail is from the Details View:

1. Go to the Details View of a Request.

2. Click on the Action Menu next to Assign/Name-of-Assignee and then
   click on **View Audit Trail**.

.. _rmf-63:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-63.png
    :align: center
    :alt: figure 63

Asking for Feedback
===================

A Technician can ask a Requestor for feedback about his/her experience
with a Request. In taking feedback, an email is sent with a link to the
feedback form or the link is embedded in the notification emails sent
when a Request is resolved and closed.

To activate feedback:

-  Go to **Admin** >> **Request Feedback Settings** (Helpdesk).

.. _rmf-64:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-64.png
    :align: center
    :alt: figure 64

-  You can automatically send a feedback link to a Requestor in the
   following ways:

   a. **Resolving a Request**: If you toggle the Resolved button on, a
      feedback link is sent with the email notification on Resolving a
      Request.

   b. **Closing a Request**: If you toggle the Closed button on, a
      feedback link is sent with the email notification on Closing a
      Request.

-  If you turn **Send feedback manually** button on, then you can send a
   feedback link to a Requester from the Details View of a Request.

.. _rmf-65.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-65.1.png
    :align: center
    :alt: figure 65.1

.. _rmf-65.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-65.2.png
    :align: center
    :alt: figure 65.2

When a Requestor clicks on the feedback link he/she gets the following
form:

.. _rmf-66:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-66.png
    :align: center
    :alt: figure 66

You can view the feedback of a Requestor in the Details View of a
Request.

.. _rmf-67:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-67.png
    :align: center
    :alt: figure 67

.. _request-bulk-update:
Bulk Update
===========

The product allows Technicians to change Request information of multiple
Requests at once.

To perform Bulk Update:

-  Go to the :ref:`Request List View <request-list-view>`.

-  Select more than one Request.

-  The **Bulk Update** button appears above the list area. Click on
   **Bulk Update,** and a dialog box opens.

    .. _rmf-68:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-68.png
        :align: center
        :alt: figure 68

   You can change the following things:

        a. Change the assignee of the Requests.

        d. Modify the Technician Group.

        e. Change four :ref:`classifiers <classify-requests>` (Status, Priority,
           Urgency, and Impact).

        f. Add new tags or append to the existing ones.

        g. Change Category, Source, Department, and Location.

-  When you are done hit **Update,** and your changes are saved.

Merge Requests
==============

Sometimes two or more Requests are similar, or they are duplicates The
Merge function in Flotomate helps in dealing with duplicates and similar
Requests.

In the Merge process, one is the Primary Request, and all others are
Secondary. The outcome of a merge is always the Secondary Requests
linked to the Primary Request. If the Merge process happens between
Requests created by the same Requestor, then all the Secondary Requests
are closed, but they stay linked with the Primary Request.

Doing a Merge:
--------------

1. Log in to the Technician Portal.

2. Go to **Request** >> :ref:`Request List View <request-list-view>`.

.. _rmf-69:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-69.png
    :align: center
    :alt: figure 69

3. Select two or more Requests, and the **Merge** option appears over
   the list area.

.. _rmf-70:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-70.png
    :align: center
    :alt: figure 70

4. Clicking on **Merge** takes you to a new dialog box. Here you can
   choose which one to keep as Primary and which one, Secondary.
   Referring to :numref:`rmf-70`, section-A shows the Primary Request (which
   can only be one) and section-B lists the Secondary. Clicking on the
   symbol adjacent to a Request (S & P) changes a Request from Primary
   to Secondary and vice-versa.

   Section-C is the search area. You can use the search area to find
   specific Requests by using custom keywords and predefined search
   options. The Search Box works similarly to the :ref:`Search Box <searching-requests>` in List View.

   Below the Search Box is a list of other Requests. If no search filter
   is applied, then the list contains all the other Requests not
   selected for merge. Section-D allows you to select multiple Requests.
   The total number of selected Requests appears on top of the Search
   Box along with the symbol S. Click on the S symbol to add them to the
   Secondary Request area.

5. Click **Merge** once you are done with the setup. The Merge process
   closes all those Secondary Requests with the same Requestor email,
   treating them as duplicate, as in the Primary Request. Requests with
   a different email stay open.

Viewing the Relation of a Primary Request:
------------------------------------------

You can see the effect of merge under **Relations** tab in the Primary
Request’s Details View.

.. _rmf-71:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-71.png
    :align: center
    :alt: figure 71

Deleting a Request
==================

Deleting is a bulk operation which means you can delete multiple
Requests at once.

1. Go to **Request** >> :ref:`Request List View <request-list-view>`.

2. Select a Request or Requests from the list area.

3. Click Archive, and you get a confirmation message; click **Yes** to
   delete the selected Request/Requests.

.. _rmf-72:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-72.png
    :align: center
    :alt: figure 72

Announcements
=============

An announcement is a statement made to the public (Customers and
Technicians) or on a particular portal which gives information about
something that has happened or that will happen. For example: an
announcement can be made stating that the Helpdesk will be down for a
certain period.

You can run an Announcement on both Customer and Technician Portals.

.. _rmf-73:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-73.png
    :align: center
    :alt: figure 73

.. _rmf-74:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-74.png
    :align: center
    :alt: figure 74

Creating an Announcement 
------------------------

1. Log in to the Technician Portal.

2. Go to **Request** >> :ref:`Request List View <request-list-view>`.

3. Click **Manage Announcements** situated in the top right corner of
   the page. You are now on the Announcements page.

.. _rmf-75:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-75.png
    :align: center
    :alt: figure 75

4. Click on **Create Announcement** situated in the top right corner of
   the page. Create Announcement dialog box opens.

.. _rmf-76:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-76.png
    :align: center
    :alt: figure 76

5. The subject of an Announcement (section-A in :numref:`rmf-76`) is the first
   line of the message. It is supposed to give a brief introduction of
   the message.

   .. note:: All Announcements are visible to the Technicians on the
             Dashboard (under Announcement tab) in the Technician Portal.

   Section B highlights the Display options available on the dialog box,
   which are:

    +-----------------------------------+-----------------------------------+
    | Display to Customer Portal Guest  | The Announcement is visible on    |
    |                                   | the Customer Portal even when     |
    |                                   | people are not logged in.         |
    +-----------------------------------+-----------------------------------+
    | Display to only logged in         | Requestors can view the           |
    | Requestors                        | Announcement on the Customer      |
    |                                   | Portal after logging-in.          |
    +-----------------------------------+-----------------------------------+
    | Display in Technician Portal only | The Announcement is visible to    |
    |                                   | the Technicians on the Technician |
    |                                   | Portal.                           |
    +-----------------------------------+-----------------------------------+


   In section C, you can send the Announcement as an email to a group or
   groups. Flotomate allows you to send to both Technician and Requestor
   Groups or any one of them.

   All Announcements in Flotomate are scheduled. They begin on a start
   date at a specific time and end on an end date at a specific time. In
   section D, you can enter the Start Date-Time and the End Date-Time of
   the Announcement.

   The body of the message goes into the text editor (section E).

6. When you are done with your setup, click **Send** to add your
   Announcement to the list. Once added, it is scheduled to begin on
   start date-time.

Editing an Announcement
-----------------------

1. Go to **Request** >> **Manage Announcements** >>Announcements.

2. Click on the Edit Icon next to the Announcement that you want to
   change.

3. Make the changes on the Announcement dialog box and click **Send**
   to save your changes.

Deleting an Announcement
------------------------

1. Go to **Request** >> **Manage Announcements** >>Announcements.

2. Click on the Delete Icon adjacent to the Announcement that you want
   to delete.

Turning off an Announcement
---------------------------

Go to **Request** >> **Manage Announcements** >>Announcements.

.. _rmf-77:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-77.png
    :align: center
    :alt: figure 77

There is a toggle button adjacent to every Announcement. Use that to
toggle on/off any Announcement. You can also turn off an
Announcement from its Create Announcements dialog box.