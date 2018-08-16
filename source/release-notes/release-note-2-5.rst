===========================================
Flotomate ITSM – Eagle 2.5.0 – Release Note
===========================================

.. _rei-2.5-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/REl-2.5-1.png
    :align: center
    :alt: figure 1

**Introduction of new components**
==================================

1. **Service Catalog :**

   IT departments can design a pre-defined list of services items as a
   catalog which is available in requester portal as shopping service
   experience. Users can rely on the Service Catalog to avail services
   from the IT department. Flotomate provides service catalog solution
   that helps in streamlining service management to increase
   opportunities for self-service.

   **Benefits :**

   -  Improves customer satisfaction

   -  Improves the reputation of IT service department

   -  Provides efficient engagement channel for standard services with
      or without authorizations

   -  Showcases availability of services for business user consumption

   -  Improves IT opportunities for service automation resulting in
      higher service delivery performance

2. **Purchase Management :**

   Purchase department can streamline Purchase process of buying goods
   and services from a vendor and take complete control of every aspect
   of the purchase. It automates complete cycle from purchase
   requisition, approval, purchase order, invoice, payment, receive,
   inventory and reconciliation of a variety of assets. Moreover,
   Product Catalogue, Vendor Catalogue along with pre-defined price and
   tax template, Flotomate Purchase Management module makes Purchase
   Order creation process simple, easy and consistent.

   **Benefits :**

   -  Maintenance of proper and updated records of all transactions.
   
   -  Avoid stock out situations.
   
   -  To follow financial prudence.
   
   -  Reduction in inventory cost.
   
   -  Development of good relationships with existing vendors.
   
   -  Managing the departmental expenses of an Organization.

3. **Contract Management :**

   Contract Management automates the practice of managing the life-cycle
   of contracts. Contract creation, execution, and analysis come in the
   ambit of Contract Management.

   **Benefits :**

   -  Maximize the operational and financial performance of an organization
   
   -  Notifications for renewals of the contract
   
   -  Centralize Contract and its related asset information.

4. **Native Mobile App (Android & iOS)**

   Flotomate native mobile app offers a variety of features which is
   most useful for both technician and requester when they are working
   out of their desk. It especially helpful for the field technician.

   Our Mobile app has mobile-friendly features for

   -  Incident Management
   
   -  Knowledgebase
   
   -  Asset Management
   
   -  Approvals


   It is a native application built for both platform

   -  Android (Tentative on 17\ :sup:`th` August in the Google Play Store)
   
   -  iOS (Submission to App Store tentative on 31\ :sup:`st` August)

5. **Dynamic Form Builder for Customization**

   Understanding every organization has variation in implementing IT
   processes, Flotomate extensive built-in dynamic form builder allows
   to support various type of custom field with drag’n drop experience.
   It supports Text, Multi-Line Text, Number, Date, Radio, Checkbox,
   Drop-Down field with its own special property like mandatory and
   other validation. Our FlotoUX makes sure that custom field nicely
   intervenes with existing core field for simplified experience.

   Custom Field Everywhere, offers :

   -  Ability to Search on Custom Field
   
   -  Tabular & Matrix Report on Custom Field
   
   -  CSV Import into Custom Field
   
   -  Workflow & Approvals with Custom Field
   
   -  Custom Rules on Custom Field

**Service Desk & Asset Management – New Features**
==================================================

1. **Request – Canned Response :** For Repetitive/Frequent request,
   Service Desk can design pre-defined response and now Technician can
   just respond/resolve the request in few seconds to improve
   productivity.

2. **Link from My Assets on Request :** Requester can browse through
   his/her own assets in customer portal and attach in incident/request,
   so request content has more context and overall it will have a faster
   resolution time.

3. **Customizable Feedback Form :** Service Desk can design a set of a
   questionnaire for Customer Service Satisfaction survey using a
   dynamic form builder and it will be sent upon resolution of
   service-request.

4. **Guest User Request – Sign Up Link :** When guest user reports a
   service request, ITSM will send self-signup link in acknowledgment
   email, so the guest user can browse through its own tickets in
   customer portal as the logged-in user. This can be driven by
   configurable organization policy.

5. **Explicit Approval Selection :** Apart from workflow-driven,
   Technician can explicitly select for whom to ask Approval for. This
   can be driven by configurable organization policy.

6. **Configurable Notification Days :** Service Desk admin can now
   configure before how many days certain expiry and warning
   notification (i.e. License expiry, contract expiry, payment due alert
   etc.)

7. **BIOS Component Discovery :** Flotomate discovery engine and an
   agent will discover BIOS component of a computer for both Windows and
   Linux Machines.

8. **Improved Asset Relation Topology design :** Underhood technology
   change makes easy to design and visualize the direct and inverse
   relations between assets.

**Desktop Automation – New Features**
=====================================

1. **Remotely Push Windows Registry Updates :** You can create a single
   value or multi-value typed windows registry template and then select
   computers or networks as a target to push those updates with a simple
   flow. It also supports dynamic windows variables to support different
   directory location in target computers.

2. **Relay / Distribution Server :** Customer who have geographically
   distant multiple branches with thousands of desktop, Relay Server act
   as distribution point per single branch for Patches or Package
   deployment to save inter-location bandwidth which usually has higher
   latency.

3. **Batch Deployment :** Our deployment command issuer design makes
   sure your internal network bandwidth does not chock up due to patch
   or package deployment such your user can have a lower impact due to
   this activity. Our algorithm consider all asynchronous scenarios and
   allow to deploy patches in batches; same time make sure it complete
   the overall task as soon as possible.

4. **Retry Configuration for Deployment Request :** There’s always a
   chance of failure of remote deployment due to the availability of
   agent or network issue. Retry configuration allows
   remote-deploy-admin to retry count and other parameters for the
   request.

5. **Remotely Uninstallation of Patches & Software :** Similar to
   installation, Supported patches or software can be un-installed via
   remote deployment request.

6. **Software Installation with default non-silent Installer :** Not all
   software are supported to be installed silently as it required
   explicit inputs. Flotomate support feature to provide explicit inputs
   upfront and allow to install software silently.

**Administration & Support – New Features**
===========================================

1. **Periodic DB Backups :** Administrator can configure to schedule
   ITSM database backup.

2. **Workflow Action – Add me as Watcher :** New action type added “Add
   me as watcher” in workflow action to allow subscription of
   notification certain events.

3. **Ability to Change Super Admin** : Ability to transfer to ownership
   of Super Admin role to another technician.

4. **Actuator Services via Support Console :** Apart from downloading
   logs, License apply and download DB backup, System now supports a
   special kind of Production grade services called “Actuator Service”
   which will help us to diagnose system configuration, JVM memory
   utilization via single Web-UI interface, So Customer Support can be
   faster and smoother.

5. **Agent Watchdog Service :** Standalone Agent watchdog service allows
   to upgrade agent remotely for the environments where there’s no
   domain controller setup.