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
   section B (:numref:`adf-42`).

-  You can add multiple actions by clicking the **Select-An-Action**
   option (section-C). You delete an action by clicking the delete icon.

Setting Resolution Time and Escalation
--------------------------------------

Section F (:numref:`adf-42`) lets you decide the maximum time that should take
to resolve a **Request**. Just like resolution, you can add actions that
are performed before or after a violation of resolution Time.

Here you can have multiple escalations each with its own before and
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
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-44.png
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

Setting Review Period
=====================

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