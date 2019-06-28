***************
Auto-Assignment
***************

The administrators of the product have a choice whether allow users to
manually assign Technicians to a Request or use auto-assignment.
Auto-Assignment automates the assignment of a Technician to a Request.

The Auto-Assignment feature has a direct impact on the workflow of
managing Requests. It streamlines the process of assigning Requests and
eliminates the possibility of having a bottleneck.

We have three strategies for assigning a Request.

.. note:: Setting Auto-Assignment requires administrative rights.

Activate Auto-Assignment
========================

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
==========================

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

3. **Manual Assignment**: In Motadata creation of a Request is treated
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