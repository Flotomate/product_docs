************
Managing SLA
************

Service Level Agreements define the commitment between Requestors and
the IT service provider in an organization. **SLA**\ s determine the
level of urgency, response time, and the time required for Tickets
to get resolved, and they also govern the escalation rules when Tickets
are not resolved or responded within a stipulated time frame. **SLA**\ s
can be set for a department and a sub-department.

By default we have four **SLA**\ s defined out of the box with each
having their own rules for resolution and escalation time. The default SLAs are defined for the Request module and, they are
triggered based on the Priority.

+-----------------------+-------------------------+
| Low Priority **SLA**  | Medium Priority **SLA** |
+-----------------------+-------------------------+
| High Priority **SLA** | Urgent Priority **SLA** |
+-----------------------+-------------------------+

We have extended support of SLA for Problem and Change modules from build-2.7.0. Only difference being, new modules don't 
support setting of Response time and Escalation; you can only set Resolution time and escalation. 

.. note:: Managing SLAs requires Administrative rights.

Create a SLA
============

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

Section A gives you the option to choose for which module the SLA is for.

Section C lets you classify the **SLA** for a particular department. You
can select the department from a drop-down list.

**Creating an SLA rule in a four-stage process:**

Setting Operational Hour Type
-----------------------------

Section B gives you the option to either select clock time (Calendar
Hours) or business time (Business Hours). Under business time, working
hours of your organization would be considered when defining a day.

Setting SLA Conditions
----------------------

Section D (:numref:`adf-42`) lets you define the conditions for the **SLA** to
be applicable. To learn how to use control flow using condition
statements, please refer :ref:`setting Workflow conditions <set conditions>`.

Setting Response Time and Escalation
------------------------------------

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
   section B (:numref:`adf-43`).

-  You can add multiple actions by clicking the **Select-An-Action**
   option (section-C). You delete an action by clicking the delete icon.

Setting Resolution Time and Escalation
--------------------------------------

Section F (:numref:`adf-42`) lets you decide the maximum time that should take
to resolve a **Request**. Just like resolution, you can add actions that
are performed before or after a violation of resolution Time.

Here you can have multiple escalations (maximum up to five) each with its own before and
after time.

Add a Service Level Agreement (SLA)
===================================

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

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/sla-monitor/AD-SLAM-1.png
    :align: center
    :alt: figure 44

-  Save your changes by clicking on **Create**.

Edit Service Level Agreement (SLA)
==================================

-  Go to **SLA** in Automation.

-  Click on the SLA that you want to edit or click the **Edit** button.

-  Make the changes.

-  You can update your changes or delete the SLA.

In the **SLA** page, you can turn on/off an **SLA** using the toggle
under the name.

.. _Setting Review Period:

SLA Monitor
===========

An admin can monitor the performance of an SLA. The admin can define a compliance level, based on which, he can reward
or penalize a SLA.

Monitoring has to be set individually for each SLA; this allows the admin to determine the health of a SLA based on the 
accumulated points. 

Currently, monitoring is available for all types of SLA and all modules (Request, Problem and Change): both default and custom SLA. 

Few of the uses cases for using SLA Monitoring:

- SLA stands for Service Level Agreement. An SLA is a commitment between a service provider and a client. Using the SLA monitoring
  feature, a client can penalize the service provider for non-compliance. 

- SLA monitoring can be used for internal control. 

- SLA monitoring can be used for identifying bottlenecks in the Helpdesk.

Enabling SLA Monitoring
-----------------------

- Go to **Admin** >>  **SLA** (Under Automation). 

- You can add a monitor to an existing SLA not when creating a SLA. Open a SLA (it could be from any module) in edit mode.

.. _ad-slam-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/sla-monitor/AD-SLAM-1.png
    :align: center
    :alt: figure 1

- Open the **Monitor** tab and click on **Add Monitor**. 

.. _ad-slam-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/sla-monitor/AD-SLAM-2.png
    :align: center
    :alt: figure 2

- Set a time period for the monitor. You can define Start and End date. 

.. _ad-slam-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/sla-monitor/AD-SLAM-3.png
    :align: center
    :alt: figure 3

- Set a penalty compliance and penalty point. Here you have the following options:

  .. _ad-slam-4:

  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/sla-monitor/AD-SLAM-4.png
        :align: center
        :alt: figure 4

  a. **Penalty Compliance Level**: This tells the system that the compliance level of the SLA shouldn't go below the
     given number (in percentage). 

     The compliance level of a SLA is calculated using the following formula: 

     Compliance Level = 100 - SLA-Performance

     SLA-Performance = (Violated Ticket by SLA  * 100 )/ (Qualified SLA Compliant Tickets + Violated Tickets by SLA)

     When compliance level of a ticket is below the penalty level then it becomes non-compliant.

  b. **Penalty Points and Penalty Compliance Level for**: The penalty points tell how many points to subtract when SLA
     stays below the compliance level for n number of days mention in *Penalty Compliance Level for*. For penalty to happen, SLA 
     has to stay below compliance for the mentioned number of days, else the counter will get reset.  

  c. **Penalty Recurring Points and Penalty Recurring for**: The *Penalty Recurring Points* tell how many points to subtract when SLA
     continues to stay below the compliance after n number of days in * Penalty Compliance Level for* . The deduction is recurring after every n number of
     days mentioned in *Penalty Recurring for*. For the recurring deduction to happen, the SLA has to stay below compliance throughout the n number
     of days in *Penalty Recurring for*.
     
  For example: Based on :numref:'ad-slam-4', if compliance of the said SLA goes below 90% and stays there for 3 days then 10 points 
  will be deducted first, and thereafter 10 points every day after the 3rd day. If compliance goes up anytime between, then the next deduction
  will happen after staying non compliant for another straight 3 days. 

- Set a reward compliance and reward point. Here you have the following options:

  .. _ad-slam-5:

  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/sla-monitor/AD-SLAM-5.png
        :align: center
        :alt: figure 5

  
  a. **Reward Compliance Level**: This tells the system to reward certain points to the SLA if SLA compliance goes above the set
     level and stays there for a certain period of time. 

  b. **Reward Points and Reward Compliance Level for**: The Reward points tell how many points to add when SLA
     stays above the compliance level for n number of days mention in *Reward Compliance Level for*. For reward to happen, SLA 
     has to stay above compliance for the mentioned number of days, else the counter will get reset.  

  c. **Reward Recurring Points and Reward Recurring for**: The *Reward Recurring Points* tell how many points to add when SLA
     continues to stay above the compliance after n number of days in *Reward Compliance Level for* . The addition is recurring after every n number of
     days mentioned in *Reward Recurring for*. For the recurring addition to happen, the SLA has to stay above compliance throughout the n number
     of days in *Reward Recurring for*.

  For example: Based on :numref:'ad-slam-5', if compliance of the said SLA goes above 90% and stays there for 3 days then 10 points 
  will be added first, and thereafter 10 points every day after the 3rd day. If compliance goes down anytime between, then the next addition
  will happen after staying compliant for another straight 3 days.
     
- When done, click on **Update**.

View SLA Compliance Data
------------------------

- Go to **Admin** >> **SLA**. 

- Select a SLA with a Monitor. You can view the data on the right side glance view. 

.. _ad-slam-6:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/sla-monitor/AD-SLAM-6.png
    :align: center
    :alt: figure 6

Manage SLA with Status
======================

In the :ref:`Custom Status <ad-add-custom-status>` page, you can turn on/off
SLA in a Request Status using the adjacent toggle button. Learn more
about :ref:`SLA <managing sla>`.

Except for Open, Resolved and Closed, you can deactivate/activate SLA in
all other Statuses, including custom ones.

.. _adf-46:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-46.png
    :align: center
    :alt: figure 46