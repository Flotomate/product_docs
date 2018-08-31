*******************
Workflow Automation
*******************

.. _ad-workflow:

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

Understanding Workflow
-----------------------

Log in to your dashboard and go to **Admin** >> **Workflow**
(Automation). The Workflow page lists all the Workflows; it is empty
if you do not have any Workflow.

Click **Create a Workflow** situated in the top right corner of the
page.

You see the below page to open:

.. _adf-36:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-36.png
    :align: center
    :alt: figure 36

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