**********
Automation
**********

Workflow 
========

Workflow automation enables Administrators to channel tickets (Request,
Problem and Change) through a funnel with predefined rules.
Administrators set the rules that interact with the ticket details
(Department, Type, Support Level, etc.) and even change them if
required.

We give our power users a complete, customized experience without the
need to write a single piece of code. Administrators can quickly design
a control flow using our predefined events, parameters, and actions.

Workflow automation is need because managing ITSM processes can be
hectic, and with rule based actions, users can increase their scale of
operation effortlessly.

.. note:: Setting Workflow Automation requires Administrative rights.

Understanding Workflow:
-----------------------

Log in to your dashboard and go to **Admin** >> **Workflow**
(Automation). The Workflow page lists all the Workflows; it is empty
if you do not have any Workflow.

Click **Create a Workflow** situated in the top right corner of the
page.

You see the below page to open:

.. _adf-26:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-26.png
    :align: center
    :alt: figure 26

Section A tells the product on what to apply the **Workflow** logic. A
workflow can either be for Requests, Problems or Changes.

Setting the rule based actions requires you to go through four stages:

Workflow Type
^^^^^^^^^^^^^

Section E (:numref:`adf-36`) gives you the option to decide whether you want a
Workflow that is event-driven, or a Workflow that runs periodically and
checks for the conditions.

-  Events Workflows are triggered by any one of the three types of an
   event: Request, Problem\ **,** and Change.

-  Periodic Workflows are triggered by a set time (periodic intervals),
   and they check their conditions against any one of the three types of
   tickets.

Select an Event
^^^^^^^^^^^^^^^

Section B (:numref:`adf-36`) tells the product on what event within a module
(either Request, Problem, or Change) triggers an automatic process. We
have predefined events each for Requests, Problems, and Changes.

For example, You can have a Request event that triggers a workflow when
Status is changed from Open to Pending on Technician.

.. _adf-37.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-37.1.png
    :align: center
    :alt: figure 37.1

.. _adf-37.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-37.2.png
    :align: center
    :alt: figure 37.2

Set Conditions
^^^^^^^^^^^^^^

Section-C (Figure 36) tells you to apply the conditions with which you
implement the rules. You can add multiple condition groups with the
**Add Condition Group** (section F of :numref:`adf-36`) option. Within
each group, you can add multiple condition statements.

.. _adf-38:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-38.png
    :align: center
    :alt: figure 38

.. _adf-39:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-39.png
    :align: center
    :alt: figure 39

Each condition statement talks about a parameter being equal/not equal
to/contains/less or more than something. You can form a condition
statement by clicking on the three components marked by red boxes in
:numref:`adf-38`. Condition statements exist within a group, and you can add
multiple conditions by clicking on the plus sign.

There’s a hierarchy that is followed in checking conditions: first
conditions are checked within a group, and then within groups. The
outcome of a condition statement or a group of statements, or groups of
statements is either true or false. The word AND & OR helps in deriving
an outcome when there are multiple statements or groups, or both.

Multiple condition statements can be evaluated using two basic
operators: AND & OR. These two operators describe the relationship
between two statements, and the outcome is always either true or false.
The below table demonstrates the outcomes of conditions formed by AND &
OR (All permutations are shown):

+-------------+-----+-------------+---------+
| Condition 1 |     | Condition 2 | Outcome |
+=============+=====+=============+=========+
| True        | AND | True        | True    |
+-------------+-----+-------------+---------+
| True        | AND | False       | False   |
+-------------+-----+-------------+---------+
| False       | AND | True        | False   |
+-------------+-----+-------------+---------+
| False       | AND | False       | False   |
+-------------+-----+-------------+---------+

+-------------+----+-------------+---------+
| Condition 1 |    | Condition 2 | Outcome |
+=============+====+=============+=========+
| True        | OR | True        | True    |
+-------------+----+-------------+---------+
| True        | OR | False       | True    |
+-------------+----+-------------+---------+
| False       | OR | True        | True    |
+-------------+----+-------------+---------+
| False       | OR | False       | False   |
+-------------+----+-------------+---------+

You can form complex logic flows using AND & OR statements. You can mix
them within a group and groups.

You can delete any condition parameter using the red trash icon next to
it.

Set Actions
^^^^^^^^^^^

Section D (:numref:`adf-36`) talks about the action that is taken if the
condition in section C (:numref:`adf-36`) is true. We have predefined actions
based on module type. You can add multiple actions using the blue plus
icon, and delete an action using the red trash icon.

For example, you can have an action that changes the Technician Group of
a Request to Database if set conditions are triggered.

.. _adf-40:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-40.png
    :align: center
    :alt: figure 40

Create a Workflow
-----------------
Follow the below steps to create a Workflow:

-  Go to **Admin** >> **Workflow** and click **Create a Workflow**.

-  We are going to create a Workflow called Un-Spam Request.

-  We select the module type as Request.

-  We set the following values for all the four :ref:`stages <workflow type>`:

+-----------------------------------+--------------------------------------------+
| Values                            | Stage Name                                 |
+===================================+============================================+
| Event                             | :ref:`Workflow Type <workflow type>`       |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Marked as Spam                    | :ref:`Selecting an Event <select an event>`|                        
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Description contains Antivirus OR | :ref:`Setting Conditions <set conditions>` |                    
| Subject contains Antivirus.       |                                            |
+-----------------------------------+--------------------------------------------+
| Set Spam to False                 | :ref:`Setting Actions <set actions>`       |                      
|                                   |                                            |
+-----------------------------------+--------------------------------------------+

.. _adf-41:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-41.png
    :align: center
    :alt: figure 41

-  We save the Workflow by clicking on **Create**.

**Edit a Workflow**

-  Go to **Admin** >> **Workflow**.

-  Click on the Workflow that you want to edit.

-  Make changes and hit **Update** to save your changes.

You can turn your Workflow on/off using the toggle button adjacent to
the Workflow name. You can delete a Workflow by going to the edit page
and then click **Delete**.

Managing SLA
============

Service Level Agreements define the commitment between Requestors and
the IT service provider in an organization. **SLA**\ s determine the
level of urgency, response time, and the time required for **Requests**
to get resolved, and they also govern the escalation rules when Requests
are not resolved or responded within a stipulated time frame. **SLA**\ s
can be set for a department and a sub-department.

By default we have four **SLA**\ s defined out of the box with each
having their own rules for resolution and escalation time:

+-----------------------+-------------------------+
| Low Priority **SLA**  | Medium Priority **SLA** |
+-----------------------+-------------------------+
| High Priority **SLA** | Urgent Priority **SLA** |
+-----------------------+-------------------------+

.. note:: Managing SLAs requires Administrative rights.

Create a SLA:
-------------

1. Log in to your dashboard.

2. Go to **Admin** >> **SLA** (Automation). The new page lists all
   existing SLAs in the system.

3. Click **Create SLA** situated in the top right corner of the page.

You get the following page:

.. _adf-42:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-42.png
    :align: center
    :alt: figure 42

You have to give the SLA a name before doing anything else.

Section A tells us that **SLA** is only applicable to Requests which is
the default selection.

Section C lets you define the **SLA** for a particular department. You
can select the department from a drop-down list.

**Creating an SLA rule in a four-stage process:**

Setting Operational Hour Type
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Section B gives you the option to either select clock time (Calendar
Hours) or business time (Business Hours). Under business time, working
hours of your organization would be considered when defining a day.

Setting SLA Conditions
^^^^^^^^^^^^^^^^^^^^^^

Section D (:numref:`adf-42`) lets you define the conditions for the **SLA** to
be applicable. To learn how to use control flow using condition
statements, please refer :ref:`setting Workflow conditions <set conditions>`.

Setting Response Time and Escalation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Section E (:numref:`adf-42`) lets you decide the response time. If no action is
taken on a Request within the Response time then SLA is triggered. You
can set escalation rules that determine the actions after an SLA
violation. Please refer below figure to set escalation.

.. _adf-43:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-43.png
    :align: center
    :alt: figure 43

.. note:: Please refer :numref:`adf-43`.

-  You can set multiple actions before and after a response violation.
   In section A (:numref:`adf-43`), you enter when the action happens, before
   or after violation, and the time period.

-  You decide the action, in case of violation, from a drop-down list in
   section B (:numref:`adf-42`).

-  You can add multiple actions by clicking the **Select-An-Action**
   option (section-C). You delete an action by clicking the delete icon.

Setting Resolution Time and Escalation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Section F (:numref:`adf-42`) lets you decide the maximum time that should take
to resolve a **Request**. Just like resolution, you can add actions that
are performed before or after a violation of resolution Time.

Here you can have multiple escalations each with its own before and
after time.

Add a Service Level Agreement (SLA)
-----------------------------------

-  Go to **Admin** (A Navigation Tab) >> **SLA** (Automation).

-  Click **Create SLA**.

-  We are going to create an SLA called VIP SLA.

-  We add a name and department.

-  We set the following values for the
   :ref:`Stages <setting operational hour type>`:

    +-----------------------------------+----------------------------------------------------------------------------------------+
    | Values                            | Stage Name                                                                             | 
    +===================================+========================================================================================+
    | Calendar Hours                    | :ref:`Setting Operational Hour Type <setting operational hour type>`                   |                         |
    +-----------------------------------+----------------------------------------------------------------------------------------+
    | VIP Request equals to True        | :ref:`Setting SLA Conditions <setting sla conditions>`                                 |
    +-----------------------------------+----------------------------------------------------------------------------------------+
    | Set assignee to a technician      | :ref:`Setting Response Time and Escalation <setting response time and escalation>`     |    
    | after 10 mins of violation.       |                                                                                        |
    +-----------------------------------+----------------------------------------------------------------------------------------+
    | Set priority to urgent a day      | :ref:`Setting Resolution Time and Escalation <setting resolution time and escalation>` |     
    | before violation.                 |                                                                                        |
    +-----------------------------------+----------------------------------------------------------------------------------------+

.. _adf-44:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-44.png
    :align: center
    :alt: figure 44

-  Save your changes by clicking on **Create**.

Edit Service Level Agreement (SLA)
----------------------------------

-  Go to **SLA** in Automation.

-  Click on the SLA that you want to edit or click the **Edit** button.

-  Make the changes.

-  You can update your changes or delete the SLA.

In the **SLA** page, you can turn on/off an **SLA** using the toggle
under the name.

Setting Review Period
---------------------

Flotomate allows you to set review period for each SLA, where you can
reward or penalize technicians falling within a specific compliance
range.

Rewarding Technicians for staying within compliance gives them incentive
to stay within SLA guidelines

-  Go to the create/edit SLA page.

-  Scroll down to the Review Period.

.. _adf-45:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-45.png
    :align: center
    :alt: figure 45

-  Turn on Review Period using the toggle button.

-  Enter a start and an end date. The compliance range is in percentage.

-  Set the reward and penalty points and update your changes.

Manage SLA with Status
----------------------

In the :ref:`Custom Status <ad-add-custom-status>` page, you can turn on/off
SLA in a Request Status using the adjacent toggle button. Learn more
about :ref:`SLA <managing sla>`.

Except for Open, Resolved and Closed, you can deactivate/activate SLA in
all other Statuses, including custom ones.

.. _adf-46:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-46.png
    :align: center
    :alt: figure 46

.. _use-case-1:

User Story
==========

Ravi, the IT manager, is using Flotomate to manage his company’s service
desk. He knows how hectic managing the service desk can be; he has been
using Flotomate’s **Workflow** automation to manage all his Requests.

The Antivirus subscriptions of the marketing department are about to
expire. Ravi knows a significant flow of Requests is about to come. He
logs into the dashboard and creates a **Workflow** called Antivirus Key
Renew.

.. _adf-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-47.png
    :align: center
    :alt: figure 47

Ravi’s Workflow is for a **Request**. When there’s an incoming Request,
his conditions are checked against the **Request**. If a **Request**\ ’s
subject contains the word *antivirus* or description contains the word
*antivirus*, and the Department Id is Marketing then the **Request**\ ’s
Technician group is set to Network, Urgency is set to High, the
Antivirus tag is added, and due date is set to some date & time.

He then sets a custom **SLA** for the Antivirus event and names it
virus@event.

.. _adf-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-48.png
    :align: center
    :alt: figure 48

The **SLA** virus@event sets the minimum response time to 8 hours and
resolution time to 1 day (business time) when a **Request** has a
Category, Service Request and Department ID, Marketing.

Ravi sets the escalation in such a way that if the **Request** is not
responded within 10 hours then the **Request** is auto-assigned to John,
and if the resolution does not happen within a day then the priority is
automatically set to high.

.. _ad-approval-workflow:

Approval Workflow
=================

Approval Workflow helps Administrators to automate the Approval process
in the product. Flotomate allows you to create an Approval Workflow
that, when initiated, creates an Approval and adds approvers to it.

You can create an Approval workflow for:

-  Request

-  Problem

-  Change

-  Patches

-  Packages

-  Knowledge Management

Understanding Approval Workflow
----------------------------

Go to **Admin** (A Navigation Tab) >> **Approval Workflow**
(Automation).

The Approval Workflow page opens. Click on **Create an Approval
Workflow** in the top right corner of the page.

You see the below page.

.. _adf-49:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-49.png
    :align: center
    :alt: figure 49

Section-A in :numref:`adf-49` is where you give a name to the Workflow and
select the module for which you are creating the Workflow.

Creating an Approval Workflow is a two-stage process:

Setting Approval Conditions
^^^^^^^^^^^^^^^^^^^^^^^^^^^

Section-B is where you set conditions for the Workflow. When set
conditions are triggered, the system creates an Approval and assigns
approver/approvers to it. Learn more about :ref:`setting conditions <set conditions>`.

Settings Approvers
^^^^^^^^^^^^^^^^^^

Section-C is where you can set who are the approvers and the Approval
type:

-  You can set a Requestor Group as approvers. In that case, all members
   of the select group become approvers.

-  You can set individuals to be approvers.

-  You can set a type for the Approval:

   a. **Unanimous**: All of the Approvers have to approve else the
      Approval is rejected.

   c. **Majority**: If the majority of Approvers agree then Approval is
      successful.

Creating an Approval Workflow
-----------------------------

-  Go to **Admin** >> Approval **Workflow** and click **Create an
   Approval Workflow**.

-  We are going to create an Approval Workflow called Approvers for
   Problem.

-  We select Problem as our chosen module.

-  We set the following values for the
   :ref:`stages <setting approval conditions>`:

    +-----------------------------------+---------------------------------------------------------------+
    | Values                            | Stage Name                                                    |
    +===================================+===============================================================+
    | Category equals to Software       | :ref:`Setting Approval Workflow <setting approval conditions>`|                 
    +-----------------------------------+---------------------------------------------------------------+
    | Set Approvers to two Technicians. | :ref:`Setting Approvers <settings approvers>`                 |         
    | Decision Type as **Unanimous**    |                                                               |
    +-----------------------------------+---------------------------------------------------------------+

.. _adf-50:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-50.png
    :align: center
    :alt: figure 50

-  Click on **Create** to create the Approval Workflow.

**Edit an Approval Workflow**

-  Go to **Admin** >> **Approval** **Workflow**.

-  Click on the Workflow that you want to edit.

-  Make changes and hit **Update** to save your changes.

You can turn your Workflow on/off using the toggle button adjacent to
the Workflow name. You can delete a Workflow by going to the edit page
and then click **Delete**.

Setting Email Notifications
===========================

Flotomate has 67 predefined email notifications that are sent on
particular events. Emails notifications are useful in keeping
stakeholders up to date on certain aspects of the product. You have
complete control over the content of the notifications, and you can even
turn them off if required.

:ref:`Request Feedback <request feedback settings>` has a dependence on
Email Notifications. Certain notifications need to be on for feedback to
work.

.. note:: Setting Email Notification requires Administrative rights.

View Email Notifications
------------------------

- Go to **Admin** (A Navigation tab) >> **Email Notification**
   (Automation)

- In the new page, you can view all the Notifications across the
  following types:

    a. Request (13 Notifications)

    b. Problem (12 Notifications)

    c. Change (17 Notifications)

    d. Asset (13 Notifications)

    e. Knowledge (4 Notifications)

    f. Patch (4 Notifications)

    g. Package (4 Notifications)

.. _adf-51:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-51.png
    :align: center
    :alt: figure 51

.. _modify-content-of-a-notification:

Modify Content of a Notification
--------------------------------

-  Go to the Email Notifications page.

-  Click on a Notification or the Edit Icon adjacent to a Notification.

-  Notification editor opens.

-  You can give your notification a subject with placeholders.
   Placeholders are words that are replaced with specific data by the
   system before sending the notification.

    .. _adf-52:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-52.png
        :align: center
        :alt: figure 52

   In section-A & B (:numref:`adf-52`), you get a plethora of placeholders to
   choose.

    .. _adf-53:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-53.png
        :align: center
        :alt: figure 53

-  You can create impressive content with placeholders from section-B.
   Place your cursor where you want to insert and choose a placeholder
   from the Placeholders dialog box.

-  The editor provides you toolbars to format your content the way you
   want.

-  Hit **Update** to save your content.

Turn a Notification On/Off
--------------------------

-  In the Email Notifications page, you can turn a Notification On/Off
   using the adjacent toggle.

-  You can also turn a Notification on/off from its editor.

.. _adf-54:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-54.png
    :align: center
    :alt: figure 54

Integration with Third Party Services
=====================================

Flotomate supports Jira integration out of the box and any other third
party client supporting rest API.

.. note:: Integration requires Administrative rights

Jira Integration
----------------

-  Go to **Admin** >> **Integrations** (Automation)

-  You see an empty list if you are integrating an app for the first
   time, else you can see all the existing third-party integrations.

-  Click **Create an Integration** situated in the top right corner of
   the page.

-  Give a Name to the service and a suitable description.

-  Select Jira API Integration from the below option.

-  Type in the username, password, and the domain name.

-  Save your settings before exiting.

.. _adf-55:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-55.png
    :align: center
    :alt: figure 55

Rest API Client
---------------

A REST API defines a set of functions which developers can perform
requests and receive responses via HTTP protocol such as GET and POST.
Flotomate allows third party clients to create Requests using REST API.

Before using REST API, you have to create an API Client.

**Creating an API Client:**

-  Go to **Admin** >> **Integrations** (Automation).

.. _adf-55.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-55.1.png
    :align: center
    :alt: figure 55.1

-  Click on **Create an Integration** situated in the top right corner of the page.

-  Give the settings a name and description.

-  Select the **Rest API Client** option from below, and you have two options with respect to user selection.

   a. **Allow any User**: You can use the credentials of any user (registered with the product) to make API calls.

   b. **Allow specific User**: You can only use the credentials of the mentioned user for making API calls.

.. _adf-55.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-55.2.png
    :align: center
    :alt: figure 55.2  

-  Click on **Create** to save your API Client.

.. note:: The user acts as an identifier for all interactions made using
          the API. It is preferable to create a dummy user specifically for the
          Client.

- Open the API client again from the Integrations page to view the Client **ID** and **Secrete**.

.. _adf-56:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-56.png
    :align: center
    :alt: figure 56

Learn how to make an :doc:`API Call <how-to-create-request-using-rest>`.

Edit Integration
----------------

-  Go to **Admin** >> **Integrations** (Automation).

-  Click the edit icon adjacent to the API name that you want to edit.

-  Make your changes and hit **Update**.

You can delete any API integration by clicking the Delete icon, or go to
edit page and click **Delete**.

Disable a API Integration
-------------------------

-  Go to **Admin** >> **Integrations**.

-  You can disable any API with the adjacent toggle.

.. _adf-57:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-57.png
    :align: center
    :alt: figure 57

Auto-Assignment
===============

The administrators of the product have a choice whether allow users to
manually assign Technicians to a Request or use auto-assignment.
Auto-Assignment automates the assignment of a Technician to a Request.

The Auto-Assignment feature has a direct impact on the workflow of
managing Requests. It streamlines the process of assigning Requests and
eliminates the possibility of having a bottleneck.

We have three strategies for assigning a Request.

.. note:: Setting Auto-Assignment requires administrative rights.

Activate Auto-Assignment
------------------------

1. Go to **Admin** (A Navigation Tab) >> **Auto-Assignment**
   (Automation).

2. The Auto-Assignment dialog box opens. Select a strategy and save
   your selections by hitting **Update**. There are three strategies to
   select from:

    a. Manual

    b. Round Robin

    c. Smart Balance

Learn more about the Auto-Assignment Strategies.

.. _adf-58:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-58.png
    :align: center
    :alt: figure 58

Auto-Assignment Strategies
--------------------------

1. **Smart Balance**: It is a process that is designed to give the most
   optimized Request allotment strategy to the users.


    .. _adf-59:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-59.png
        :align: center
        :alt: figure 59

   To understand how Smart Balance works, we need to understand when
   Smart Balance is initiated. Three events can trigger a Smart Balance
   allotment:

    a. Creation of a Request;

    b. Change in Support Level (this trigger is by default turned off ).

    c. Change in Technician Group (this trigger is by default turned off).

   The events can occur independently or simultaneously.

    a. **Creation of a Request**: When a Request reaches the system, a
       Technician is assigned automatically using our proprietary algorithm.
       The algorithm takes into consideration the following things:

        i.   Workload/availability of every Technician at that time.

        ii.  Associated tier of the Request.

        iii. Associated Technician group of the Request.

    b. **Change in Support Level**: After a Request is added to the Request
       List and the initial assignment, a change in the Support Level
       without effecting assignment, either done manually, by SLA or
       Workflow, acts as a trigger event for Smart Balance. Once Smart
       Balance is initiated two sub-conditions are checked: (Section-C of
       :numref:`adf-59`)

        i. **Auto-Assignment Based on Support Level Only**: If this
           condition is turned on, Smart Balance assigns the Request to a
           technician belonging to the new support level.

        ii. **Auto-Assignment Based on Support Level and Technician Group**:
            If this condition is turned on, the assignment goes to a
            Technician who is at the intersection between the new Support
            Level and the present Technician Group.


       If both conditions are turned on, the system checks the second
       condition first; if it is not meet, the product moves to the first
       condition.

       If neither of the conditions is met, then the assignment goes to the
       Default Assignee (section A of :numref:`adf-59`).

    c. **Change in Technician Group**: After getting added to the Request
       List and the initial assignment, subsequent changes in the Request
       resulting in a change of Technician Group acts as a trigger for Smart
       Balance to act. Once Smart Balance is initiated two sub-conditions
       are checked: (Section D of :numref:`adf-59`)

        i.  **Auto-Assignment Based on Technician Group Only**: If this
            condition is turned on, Smart Balance assigns the Request to a
            technician belonging to the new Technician Group.

        ii. **Auto-Assignment Based on Technician Group and Support Level**:
            If this condition is turned on, the assignment goes to a
            Technician who is at the intersection between the new Technician
            Group and the Support Level.

       If both conditions are turned on, the system checks the second
       condition first; if it is not meet, the product moves to the first
       condition.

       If neither of the conditions is met, then the assignment goes to the
       Default Assignee (section A of :numref:`adf-59`).

   The administrator has the option to exclude people from the Smart
   Balance process by providing their names in section B of :numref:`adf-59`.

2. **Round Robin**: Under this strategy, the assignment is done
   indiscriminately across all available technicians. The assignment
   starts with the first technician and moves to the next, and when it
   reaches the last, it again reverts to the first technician. The
   process is perpetual till the strategy is deselected.

   When a Request reaches the system, Round Robin is initiated after SLA
   and Workflow conditions (if any) are checked. In case no automatic
   assignment happens, Round Robin proceeds to assign a Technician to
   the Request based on its logic.

   The administrator has the option to include a list of
   technician/technicians, who is/are not authorized to process
   requests, in the Excluded Technicians field in :numref:`adf-58`.

3. **Manual Assignment**: In Flotomate creation of a Request is treated
   as an event, and when this event occurs, it can trigger specific
   automatic actions. If no assignment happens, even after the
   automatic actions, then the Request awaits for manual assignment.
   Subsequently, someone has to assign a Technician to the Requestor
   create/wait-for any other event that triggers an automatic action
   that leads to an assignment.

    .. _adf-60:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-60.png
        :align: center
        :alt: figure 60

   Manual is the default strategy if no automation is selected.