***********************************
Creating a Service Catalog Template
***********************************

A Service Catalog Template allows you to define a service. You define a Template in a particular Service Category (:ref:`Learn more<adding service catalog categories>`).
A Template is defined with respect to the following:

- Form fields that will capture custom data.

- Specific workflow to automate the handling of the life-cycle of the Requests created using the Template.

- Specific SLA to control the response and resolution time, and escalation.

- Specific Approval workflow to add supervision.

- Create associated task for Requests created using the Template.

We are going to create a Template called On-Boarding that will be used to create a Service Item which will be used by the HR dept
to create Request for on-boarding of new employees in the Marketing department. Learn about the :ref:`Use Case <sc-use-case>`.  

New Service Catalog Template
============================

- We go to **Admin** (A Navigation tab) >> **Templates** (under Service Catalog).

- Templates page opens. Here we can see all existing categories and their templates. We select the category Human Resource
  (Learn how we created the :ref:`Category<adding service catalog categories>`) and then we click on **Create Template**.

.. _scf-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-9.png
    :align: center
    :alt: figure 9

- A dialog box opens, asking for a name, and we give the name **On-Boarding**. 

.. _scf-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-10.png
    :align: center
    :alt: figure 10

- A new page opens, here we have to create a form, define a workflow, create a SLA and create an Approval workflow, and add tasks. 

Create Form
-----------

.. note:: Related Topic: :ref:`Working with Form Fields <Working with Custom Fields>`

- Using drag and drop we create the following form:

.. _scf-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-11.png
    :align: center
    :alt: figure 11

- All of the fields are Text Fields. Learn about the :ref:`different types of fields <ad-types-of-fields>`. You can access the
  properties of a field by clicking on it. We have set the fields to be compulsory and visible to the requesters.

.. _scf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-12.png
    :align: center
    :alt: figure 12

You can select what default fields to show on the Service Item Request form.

.. _scf-12.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-12.1.png
    :align: center
    :alt: figure 12.1    

Create Workflow
---------------

Workflow automation enables Administrators to channel tickets through a funnel with predefined rules.
Administrators set the rules that interact with the ticket details
(Department, Type, Support Level, etc.) and even change them if
required.

**Implementation Behavior:**

- Workflow created here will work specifically for Requests created using a :doc:`Service Item<create-service-item>` having the On-Boarding Template.

- The Workflow created here works parallel with the generic :ref:`WorKflow <ad-workflow>` in Admin. Both the Workflows might get initiated
  together and perform their own actions after checking their conditions.

- The Template Workflow is initiated based on the **When Condition** of a workflow.

.. note:: Related Topic: Learn how to create a :ref:`Custom Workflow <understanding workflow>`.


We click on the **Workflow** tab. Here we see all Workflows specific for that Template, if any. We click on **Create a Workflow**
button to add a new workflow. 

In the new page, we define a name, add parameters and select actions.

    .. _scf-13:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-13.png
        :align: center
        :alt: figure 13

The workflow wil work on Requests satisfying the parameters, which are Department equals to Marketing and Location
equals Ahmedabad. 

    .. _scf-14:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-14.png
        :align: center
        :alt: figure 14

Following actions are taken when a Request satisfies the parameters:

- Request is assigned to a Technician.

- Priority is set to High.

- An Email is sent to the Requestor.

    .. _scf-15:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-15.png
        :align: center
        :alt: figure 15

Fields created in the :ref:`Form section <Create Form>` can be used to make conditions as part of a template workflow. 
Custom fields are automatically added to the event list, Add if list, and Add Action list. For example, We can create
an event condition with the field Employee ID:

.. _scf-15.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-15.1.png
    :align: center
    :alt: figure 15.1

Define SLA
----------

Service Level Agreements define the commitment between Requestors and
the IT service provider in an organization. **SLA**\ s determine the
level of urgency, response time, and the time required for **Requests**
to get resolved, and they also govern the escalation rules when Requests
are not resolved or responded within a stipulated time frame. **SLA**\ s
can be set for a department and a sub-department.

**Implementation Behavior:**

- An SLA created here will work specifically for Requests created using a :doc:`Service Item<create-service-item>` having the On-Boarding Template.

- Template SLA will decide Response and Resolution time of Requests created using a Service Item (with the On-Boarding Template).

- The system SLA will not work along side Template SLA.

.. note:: Related Topic: Learn more about :ref:`Create a SLA`. 

We click on the **SLA** tab. Here we can see all existing SLA's specific to the Template, if any. We click on **Create an SLA**.

In the new page, we set the following things:

We give a name, set Operational Hour Type and Department.

     .. _scf-16:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-16.png
         :align: center
         :alt: figure 16

We set the following parameters. The SLA will be valid for Requests satisfying the below mentioned parameters. 

     .. _scf-17:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-17.png
         :align: center
         :alt: figure 17

Then we set the minimum response and resolution time, and escalation in case of violation.

     .. _scf-18:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-18.png
         :align: center
         :alt: figure 18   
       
We set the response time as 3 hours and on violation the assigned Technician and Priority is changed.
We set the Resolution time as 1 day and on violation the assigned Technician is changed.

Approval Workflow
-----------------

Approval Workflow helps Administrators to automate the Approval process for a Request. 
An Approval Workflow, when initiated, creates an Approval and adds approvers to it.

**Implementation Behavior:**

- An Approval Workflow created here will work specifically for Requests created using a :doc:`Service Item<create-service-item>` having the On-Boarding Template.
 
- The generic Approval Workflow in Admin doesn't work in Requests created using a Service Item.

.. note:: Related Topic: Learn more about :ref:`Approval Workflow<ad-approval-workflow>`

We click on the **Approvals** tab. Here we can see all existing Approval Workflows specific to the Template, if any. 
We click on **Create an Approval**.

In the new page, we give a name, parameters and actions:

  .. _scf-18.1:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-18.1.png
       :align: center
       :alt: figure 18.1

Any Request (made using the template) having the Department Marketing will have the following output:

- A two stage Approval will be created. 

- Each stage of the Approval will have a single Approver.

- Stages will have an order (:ref:`Learn More <Multiple Approvals>`)


Adding Tasks
------------

.. note:: Related Topic: Learn about :ref:`rm-managing-task` 

- We can pre-define tasks that will be added to the Request. We can break the tasks stage wise; meaning tasks at one stage has to be 
  completed to move to another stage. We click on the Task tab. 

  .. _scf-19:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-19.png
        :align: center
        :alt: figure 19

- We create three stages (we define a stage by adding a task to it) with each having one task.

Things to Remember:

- The Task thread created here will not be disturbed by a Task created manually in the Request.

- Tasks of one stage is visible at a time.


Create a Scenario
-----------------

We can create scenarios specifically for Requests created using the Template. A scenario is a set of actions ,when applied, that can
modify a ticket. We can create n number of scenarios in a template each with its own set of conditions. 

- Under the Scenario tab, click on **Create a Scenario**.

- Create a scenario in the new page. Learn :ref:`how to create a scenario <Create a Scenario>`. 

After creating the scenario, we can enforce the scenario on Request tickets created using the template. :ref:`Learn more <Enforcing a Scenario>`.

Now we are done with everything. We have two options now: either publish the Template or leave it as Draft. We publish the Template
using the **Publish** button. The Template gets activated.

.. _scf-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-20.png
    :align: center
    :alt: figure 20


You can edit/delete the Template (along with its conditions) anytime later. 

.. _scf-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-21.png
    :align: center
    :alt: figure 21