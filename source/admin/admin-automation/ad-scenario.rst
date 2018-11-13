*******************
Scenario Automation
*******************

Scenario automation allows a user to apply specific changes to a Request, Problem or Change ticket based on a defined scenario (conditions).
An admin can create multiple scenarios each for Request, Problem and Change. He can define access level for each scenario
that restricts access to  particular technician/technicians or group/groups. 

**Some of the Benefits of Scenario Automation**

- Make multiple changes to a ticket on a single click. 
- Create a template for a specific kind of tickets.
- Automate the handling of recurring scenarios.

Create a Scenario
=================

.. note:: The operations requires admin rights. 

We are going to create a scenario that assigns a Problem ticket to a particular technician having the tag **Server** and Priority: **High**.

-  We go to **Admin** >> **Scenario** (Automation).

.. _sce-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/scenario/AD-SCE-1.png
    :align: center
    :alt: figure 1

- In the scenario page, we can view existing scenarios. We can filter scenarios by module and search them using a keyword.

- Click on **Create a Scenario** situated in the top tight corner of the page. 

- In the create page, you can input the following:

  .. _sce-1.1:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/scenario/AD-SCE-1.1.png
       :align: center
       :alt: figure 1.1

  a. Name of the scenario.

  b. Module of the scenario.

  c. Define an access level:

     i. **Technicians Access Level**: Grant access to specific technicians to use the scenario.
     ii. **Technicians Group Access Level**: Grant access to group.groups.

  d. Description of the scenario.

  e. **Scenario Condition**: Learn :ref:`how to set conditions <Set Conditions>`.

  f. **Scenario Actions**: Define what operations to perform when scenario conditions are meet. 
     Learn :ref:`how to set actions <Set Actions>`.

- We create the following scenario:

  a. We grant access to the **Hardware Group**. Only technicians in the mentioned group can execute the scenario.

  b. We define conditions and an action.

    .. _sce-2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/scenario/AD-SCE-2.png
        :align: center
        :alt: figure 2

- We click **Create** to save the scenario.

An admin can enable & disable a scenario from the Scenario page. He can also edit a scenario. 

Enforcing a Scenario 
====================

A technician can enforce a scenario on a ticket from its details view. When a scenario is enforced, the system checks whether 
the ticket fulfills the scenario conditions; if it fulfills then the scenario implements its actions.

.. note:: :ref:`Request Details View`, :ref:`Problem Details View` and :ref:`Change Details View`.

**Follow the steps to enforce a scenario:**

- Go to the Details View of a ticket and click on **Scenario**. 

.. _sce-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/scenario/AD-SCE-3.png
    :align: center
    :alt: figure 3

- A dialog box opens showing available scenarios for the module. Here you will view scenarios created by you and scenarios
  shared with you by others. 

  .. note:: Creating a scenario requires admin rights.

.. _sce-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/scenario/AD-SCE-4.png
    :align: center
    :alt: figure 4

- Enforce a scenario by clicking on the adjacent **Execute** button and confirming the operation. 