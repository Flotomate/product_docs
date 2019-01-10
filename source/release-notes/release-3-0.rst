*****************************
Release Notes - Ostrich 3.0.0
*****************************

**Introduction of New Features**
================================

1. Location Scoping
-------------------

We have implemented location based data segregation for organizations with diverse geographical presence; 
it is achieved using location scoping. Data in the ITSM tool is segregated for technicians and requesters based on location; 
for example, London office technicians will support that office’s requesters and authorized to see that location’s data.

**Few Use Cases for Location Scope**

- A ticket filed in a particular office will be visible to the technicians assigned to that office. 
  A ticket must carry location information for location scope to work. Such segregation speeds up the service delivery process.

- Achieve security through obscurity. You can define access authorization using location. 
  A technician assigned to a particular location will see data of that location only.

- Manage large amount of tickets through segregation based on location. 
  A technician assigned to a location will able to see tickets of his/her location.

- Achieve separate automated workflows for different locations using location scoping. Scope of Location Segregation

Following objects comes within the scope of location based segregation (i.e. Data accessed by location):

- Incident

- Problem

- Change

- Asset

- Report

- Project

- Technician***

- Requester***

**Implementing Location Scope**

.. _re-3.0-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-3.0-3.png
    :align: center
    :alt: figure 3

**Related Guides:**

- :ref:`Data Segregation with Location Scope`

2. Plugin Server
----------------

Flotomate has introduced the concept of plugins, which is piece of code that integrates with our main server to perform 
a specific function. In the context of our product, a plugin is nothing but a .fp bundle (i.e. Kind of app, zip).

A Plugin server is a server which hosts/runs plugins. It is like our main server with a specialized purpose of running plugins. 
The main server will call a plugin server to execute specific plugin and get the desired output.

.. _re-3.0-0:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-3.0-0.png
    :align: center
    :alt: figure 0

**Why use a Plugin Architecture?**

Different users have different needs as customization is the reality of our market. It not possible to accommodate all different needs in the form of a product feature, which is why we have introduced the concept of plugin architecture.

**Benefits of a Plugin Architecture:**

- Gives the ability to add business specific functions to the ITSM tool; for example, a user might want to send a notification to his CRM when a ticket is created.

- Provides a great deal of flexibility when it comes to customization without burdening the tool.

- New functions can be added with changing the code base of the main product.

Related Guides:

- :ref:`Plugin Server Setup Guide`
- :ref:`Register a Plugin`  

3. ITSM Plugin - Active Directory Integration 
---------------------------------------------

This is a standard plugin offered by Flotomate to all our users.

**Purpose**: The plugin provides integration with an Active Directory. When the plugin is executed it can create new users, update existing users, read user data and delete a user using the LDAP protocol.

**Perquisite**: Plugin server needs to be setup with the main server.

Learn how to :ref:`Setup Plugin <ITSM Plugin - Active Directory Integration>`.

4. Scenario Automation
----------------------

Scenario automation allows a user to apply specific changes to a Request, Problem or Change ticket based on a defined scenario (conditions).
An admin can create multiple scenarios each for Request, Problem and Change. He can define access level for each scenario
that restricts access to  particular technician/technicians or group/groups. 

.. _re-3.0-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-3.0-1.png
    :align: center
    :alt: figure 1

.. _re-3.0-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-3.0-2.png
    :align: center
    :alt: figure 2

**Some of the Benefits of Scenario Automation**

- Make multiple changes to a ticket on a single click. 
- Create a template for a specific kind of tickets.
- Automate the handling of recurring scenarios.

You can also create a specific scenario for a :ref:`Service Catalog <Service Catalog Workflow>` item. 
:ref:`Learn more <Create a Scenario>`. 

Related Guides:

- :ref:`Scenario Automation`

5. Project & Task Management
----------------------------

Flotomate now has the Project Management module. To support the Project Management module, we have centralized the task
management as a separate module that shows all tasks (throughout the system) of a technician. 

.. _re-3.0-5:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-3.0-5.png
    :align: center
    :alt: figure 5

.. _re-3.0-6:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-3.0-6.png
    :align: center
    :alt: figure 6

**Some of the Benefits:**

- Collaboration on Projects.

- Monitoring of milestones.

- Track resource utilization.

- Share documents.

- Perform delegation in the form of tasks

**Key Highlights:**

- Intuitive UI to track project milestones and tasks. 

- Create and assign tasks from a project.

- Track total man hour worked on a project through time-log.

- Relate a task with other modules.

- Location scope in project management. 

- Assign technician to a project as a member. 

**Feature Improvements**
========================

1. **Auto Update of Asset Location and User:** 

   Flotomate now has a feature that allows the system to automatically assign an asset to a requester based on the Logon Name provided in the
   system. The Logon Name is the workstation username which is provided when registering a requester. When an asset is discovered, it is matched
   with a requester using the Logon Name. You can find the username in Windows 10 from Control Panel >> User Accounts.
   
   .. _re-3.0-4:
   
   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-3.0-4.png
       :align: center
       :alt: figure 4
   
   Related Topics: :ref:`Adding a Requester <Add Requestors Individually>`.
   
   Now Flotomate automatically assigns a location to an asset based on the Network.The assignment happens during a discovery of an asset by both agent-based and agent-less method. The location
   is assigned from the :ref:`Network List <Add a Network>`; if a discovered asset has an IP that falls in a Network with an assigned location,
   then the location is inherited by the asset as well.
   
   Relate Guide: :ref:`helpdesk security`

2. **Report:**

   - Package Report

   - Deployment Request Report

   - Report of Asset Audit Trail (Change Log, and Scan Log).

   - Agent report based on active and inactive status.

3. **Request**:

   - Requests created from a Service Catalog item automatically has the source field set to *Service Catalog*. 

4. **Patch and Packages:**

   - Check whether downloaded patches are corrupt or not using Checksum.

5. **Service Catalog:**
  
   - Service template workflow now runs for all event triggers. 

   - Hide a form field of a Service Catalog item from Requesters.

6. **New Technician Access Control**
   
   - **Group Access**: This puts an additional restriction on top of :ref:`location scope <Data Segregation with Location Scope>`. A technician with Group Access permission
     will be able to see only Requests tickets with unassigned Technician Group, and if assigned, then he/she has to be
     part of the group in order to see the tickets.

   - **Restricted Access**: This puts an additional restriction on top of :ref:`location scope <Data Segregation with Location Scope>`. Technicians with this permission 
     won't be able to view and create Request tickets.
 
7. **SLA (Service Level Agreement):**
   
   - **SLA Monitoring**: An admin can monitor the performance of an SLA. The admin can define a compliance level, based on which, he can reward
     or penalize a SLA (:ref:`Learn more <SLA Monitor>`).
   
8. **Knowledge:** 
  
   - New privacy model and sharing features (:ref:`Learn More <Knowledge Permissions>`).

9. **Others:**

   - Create workflows on approval statuses for Service Desk and Catalog. 

   - Custom Fields in a workflow Event, (both main workflow and Service Catalog workflow)

   - Create custom hidden fields to show system generated data. 

   - Shared Drive Cleanup and Disk Space notification feature.

   - A global group has been added called **All Technician Group**. 
