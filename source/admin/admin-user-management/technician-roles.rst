****************
Technician Roles 
****************

Every Technician is different, so we have roles to give them different
rights and permissions. Each role is unique, and out of the box we have
seven roles in the system; you cannot modify the permissions and rights
of these roles. However, you can add custom roles where you can set the
permissions and rights; there’s no limit to the number of custom roles
that you can create.

Using Roles you can control the CRUD operations a Technician can perform
across the following modules:

-  Request

-  Problem

-  Change

-  Project

-  Patch

-  Knowledge

-  Asset

-  Admin

- Contract

- Purchase

- Report

- Dashboard

Default Roles
=============

Motadata offers eight default roles with predefined permissions
covering major ITSM processes.

+-------------------------------+-------------------------------+------------------------------+
| Contract Manager              | Purchase Manager              | Patch Specialist Technician  |
+-------------------------------+-------------------------------+------------------------------+
| Junior Technician             | Asset Specialist Technician   | Change Specialist Technician |
+-------------------------------+-------------------------------+------------------------------+
| Problem Specialist Technician | Request Specialist Technician | Service Desk Technician      |
+-------------------------------+-------------------------------+------------------------------+
| Admin                         |                               |                              |
+-------------------------------+-------------------------------+------------------------------+

Add/View Roles
==============

-  In the **Admin** section, you can view all the roles in Roles
   (under Users) page. Click any one role to view its permissions and rights.

.. _adf-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-27.png
    :align: center
    :alt: figure 27

-  You add a custom role by going back to the **Roles** page and
   clicking **Create a Role** situated in the top right corner of the page.
   We have the permissions and rights grouped module wise. Click any one
   module to see its rights and permissions.

-  Add a name to the role and a description. You can set the permissions
   and rights for every module.

   We have the following rights and permissions:

    +-----------+--------------------------------------------------+
    | Project   | -  Only view details of Projects                 |
    |           |                                                  |
    |           | -  Create & Update Projects                      |
    |           |                                                  |
    |           | -  Delete Projects                               |
    |           |                                                  |
    |           | -  Manage Project milestones                     |
    |           |                                                  |
    |           | -  Closing a Project                             |
    |           |                                                  |
    |           | -  Manage Project Attachments                    |
    |           |                                                  |
    |           | -  Create Tasks in Project.                      |
    |           |                                                  |
    |           | -  Cancel a Project                              |
    +-----------+--------------------------------------------------+
    | Knowledge | -  Create, update, manage folders,               |
    |           |    and archive folder.                           |
    +-----------+--------------------------------------------------+
    | Request   | -  View, create, update and delete a Request.    |
    |           |                                                  |
    |           | -  Communicate with Requestors.                  |
    |           |                                                  |
    |           | -  Mark a Request as spam.                       |
    |           |                                                  |
    |           | -  Assign a Technician to a Request.             |
    |           |                                                  |
    |           | -  Update status of a Request.                   |
    |           |                                                  |
    |           | -  Close a Request                               |
    |           |                                                  |
    |           | -  Manage relationship in a Request.             |
    |           |                                                  |
    |           | -  Add solution and tasks in a Request.          |
    |           |                                                  |
    |           | -  Merge multiple Requests.                      |
    |           |                                                  |
    |           | -  Resolve a Request.                            |
    |           |                                                  |
    |           | -  Re-open a closed Request.                     |
    |           |                                                  |
    |           | -  Update priority of a Request.                 |
    +-----------+--------------------------------------------------+
    | Problem   | -  View, create, update and delete a Problem.    |
    |           |                                                  |
    |           | -  Add solution to a Problem.                    |
    |           |                                                  |
    |           | -  Assign Technician to a Problem.               |
    |           |                                                  |
    |           | -  Resolving a Problem.                          |
    |           |                                                  |
    |           | -  Re-opening a closed Problem.                  |
    |           |                                                  |
    |           | -  Create tasks in a Problem.                    |
    |           |                                                  |
    |           | -  Update status and priority in a Problem.      |
    |           |                                                  |
    |           | -  Managing relationships in a Problem.          |
    +-----------+--------------------------------------------------+
    | Change    | -  View, create, update and delete a Change.     |
    |           |                                                  |
    |           | -  Creating tasks in a Change.                   |
    |           |                                                  |
    |           | -  Assign a Technician to a Change.              |
    |           |                                                  |
    |           | -  Updating status and priority of a Change.     |
    |           |                                                  |
    |           | -  Managing relationships in a Change.           |
    |           |                                                  |
    |           | -  Closing and Re-opening a Change               |
    +-----------+--------------------------------------------------+
    | Patch     | -  Manage Patches & Packages                     |
    |           |                                                  |
    |           | -  View Patches & Package.                       |
    |           |                                                  |
    |           | -  View Remote Deployment.                       |
    |           |                                                  |
    |           | -  View/Manage Computer Group                    |       
    |           |                                                  |
    |           | -  Manage Remote Deployment Policy.              |
    |           |                                                  |
    |           | -  View Auto Patch Deployment Task.              |
    |           |                                                  |
    |           | -  Manage Auto Patch Deployment Task.            |
    |           |                                                  |
    |           | -  View Auto Patch Test Task.                    |
    |           |                                                  |
    |           | -  Manage Auto Patch Test Task.                  |
    |           |                                                  |
    |           | -  View Decline Patch Configuration.             |
    |           |                                                  |
    |           | -  Manage Decline Patch Configuration.           |
    |           |                                                  |
    |           | -  Manage Remote Deployment.                     |
    |           |                                                  |
    |           | -  Permission to ignore Patches.                 |
    |           |                                                  |
    |           | -  Permission to configure Packages for Patches. |
    +-----------+--------------------------------------------------+
    | Asset     | -  Managing Asset discovery and Administration.  |
    |           |                                                  |
    |           | -  View, create, update and delete an Asset.     |
    |           |                                                  |
    |           | -  Update status of Assets.                      |
    |           |                                                  |
    |           | -  Manage relationships of Assets.               |
    +-----------+--------------------------------------------------+
    | Admin     | -  Manage organization.                          |
    |           |                                                  |
    |           | -  Manage automation in the product.             |
    |           |                                                  |
    |           | -  Ignore approvers in an Approval process.      |
    +-----------+--------------------------------------------------+ 
    | Contract  | - View Contracts                                 |
    |           |                                                  |
    |           | - Update and Create Contracts                    |
    |           |                                                  |
    |           | - Delete Contracts                               |
    |           |                                                  |
    |           | - Manage attachments of Contracts                |
    |           |                                                  |
    |           | - Contract Renewal                               |
    |           |                                                  |
    |           | - Manage relationships of Contracts              |
    +-----------+--------------------------------------------------+
    | Purchase  | - View Purchase Order                            |
    |           |                                                  |
    |           | - Create and update Purchase Order               |
    |           |                                                  |
    |           | - Delete Purchase Orders                         |
    |           |                                                  |
    |           | - Manage invoice and payments                    |
    |           |                                                  |
    |           | - Manage relationships of PO                     |
    |           |                                                  |
    |           | - Closing POs                                    |
    |           |                                                  |
    |           | - Cancel Purchase Order                          |
    +-----------+--------------------------------------------------+
    | Report    | - View and manage Reports                        |
    +-----------+--------------------------------------------------+
    | Dashboard | - Manage Dashboard gives the permission to       |
    |           |   Create/Update/Delete/Duplicate Dashboards      |
    |           |                                                  |
    |           | - Manage KPI and Widgets gives the permission to |
    |           |   Create / Update / Delete / Duplicate Dashlets  |
    +-----------+--------------------------------------------------+

-  Once you are done with the permissions and rights, hit **Create** to
   create your new role.

**Modify Roles**

You can go to the **Roles** page anytime and change the permissions and
rights of the roles that you have created using the Edit Icon. Default
roles cannot be modified.