************************
Patch/Package Deployment
************************

Patch Custom Rules
==================

Custom rules allow you make certain things prerequisite before
performing certain activities. You can access custom rules from
**Admin** (accessed from **Product Launcher**) >> **Patch Custom Rules**
(Patch/Packages Deployment). Currently, the product offers the following
rules:

.. note:: The edit button makes the fields editable.

-  Set requirement for an Approval before publishing a Deployment
   Request.

.. _adf-116:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-116.png
    :align: center
    :alt: figure 116

System Health Configuration
===========================

Patch Management ensures that all administered IT Assets are updated
with the latest Patch from the Software Vendor; this enhances security
and helps in thwarting external and internal cyber-attacks.

Computers fetch and deploy Patches. So it becomes imperative to monitor
all Computers to keep yourself aligned with the idea of Patch
Management.

Our product has a feature called System Health that flags Computers that
are missing critical, essential Patches. This helps you to manage your
vulnerability and prevent any attacks.

Learn how configure :ref:`system-health-settings`. 

.. _add-endpoint-scope:

Endpoint Scope
==============

Depending on the License agreement you have with us, the number of
Computers you can manage for Patch/Packages/Registry is
limited. All discovered Computers (with our Agent application) stay out
of the scope (target) of Remote Deployment by default; you have to bring them within
the scope (target).

The Endpoint Scope lets you view all available Computers (both in and out of Endpoint Scope) and add them to the scope of Remote Deployment. 
You can set certain conditions that will allow the main server to add any new Computers automatically to the scope. You can also
add Computers manually.

There is a counter on the Endpoint Scope page that shows how many Computers are allowed within the scope. 
In no situation, you can exceed the mentioned number.

.. note:: Only Computers configured with our Agent Application are visible in the Endpoint Scope page.

.. _add-computer-scope:

Add Computers to a Scope
------------------------

-  Go to **Admin** (a Navigation Tab) >> **Endpoint Scope**
   (Patch/Package Management).

.. _P-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-1.png
   :align: center
   :alt: figure 1

-  The Endpoint Scope page opens.

.. _P-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-2.png
   :align: center
   :alt: figure 2

-  You can view the total number of Computers that you can add as
   *Total Endpoints in Scope* number. 

.. _P-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-3.png
   :align: center
   :alt: figure 3

.. _add-remote-office:   

Adding a Remote Office (Automatic Addition of Computers)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

-  You can associate a :doc:`Remote Office <remote-office>` with a Scope (target); this allows the Scope (target) to
   automatically add Computers (with the Agent application) in the
   Remote Office based on include and exclude conditions. You can use both
   manual and automatic addition of Computers together; they are not
   mutually exclusive.

   .. note:: Related Topic: :doc:`Remote Office <remote-office>`

.. _P-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-4.png
   :align: center
   :alt: figure 4

-  Once you select a Remote Office, you can add conditions. The
   conditions are of two types: include and exclude. Both the types
   create a set of Computers from which to either include or exclude.
   When there’s an intersection or conflict between the two types then
   exclude conditions/condition override the include set. For example,
   to add Computers within an IP range and with a hostname containing “Digit”
   , and excluding those with "Vector" in their Hostname, yields the following conditions (refer: :numref:`P-5.2`):

   .. note:: Without include and exclude conditions, all Computers in a Remote office will be added.

.. _P-5.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-5.1.png
   :align: center
   :alt: figure 5.1

.. _P-5.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-5.2.png
   :align: center
   :alt: figure 5.2

Adding of Computers from List
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

-  You can manually search and add Computers to a scope (target). The search bar
   supports the Advanced Search feature where you get search options by
   clicking on the search bar.

.. _P-6.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-6.1.png
   :align: center
   :alt: figure 6.1

.. _P-6.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-6.2.png
   :align: center
   :alt: figure 6.2

::
    You can also enter keywords to search for a Computer. When entering a
    keyword, the product explores all the Computers with the keyword in
    their Name, Hostname, Domain name, OS name and Service Pack. A Computer
    has to have at least one field matched (partial or full) with the
    keyword; in case there are multiple keywords, a Computer has to have at
    least one field matched for each keyword.

    You can combine search options with keywords. Between two different
    conditions of the same type OR logic is followed. Between different
    types AND logic is observed. An example of same type contradiction is Network
    equals Windows vs. OS Network equals Dell-Servers. Between keywords and conditions AND logic is followed.

.. _P-7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-7.png
   :align: center
   :alt: figure 7

-  Once you have found your Computers, add by selecting them, and they
   move to the Selected Computers list. Manually selected Computers
   override the exclude criteria/conditions set for the Remote Office.

.. _P-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-8.png
   :align: center
   :alt: figure 8

-  Once you are done setting conditions and adding Computers, click on
   **Update**.

.. _endpoint-scope:

Adding Multiple Scopes
^^^^^^^^^^^^^^^^^^^^^^

-  You can create more than one Scope (target) to accommodate multiple Remote Offices
   (a Scope can have only one Remote Office). The actual Endpoint Computer list is
   cumulative of all available Scopes (added manually and
   automatically).

.. _P-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-9.png
   :align: center
   :alt: figure 9

.. _P-9.1.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-9.1.1.png
   :align: center
   :alt: figure 9.1.1   

.. _preview-scope-list:

Preview Computer List
---------------------

Once you are done with adding Computers and setting conditions, you can
view the final list of all the Computers in all the Scopes (targets) and also individual scopes using the Preview function.

Open Endpoint Scope from **Admin**. Click on **Preview** to generate the
Computer list. The preview button is also there for each scope.

.. _P-9.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-9.1.png
   :align: center
   :alt: figure 9.1

.. _P-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-10.png
   :align: center
   :alt: figure 10

You can search for a Computer. The search bar supports the Advanced
Search feature. It is similar to the search bar in a
:ref:`Scope <endpoint-scope>`.          

.. _patch-approval-settings:

Approval Settings
=================

The idea of Patch Management revolves around security, enhancement, and
compliance. Sometimes it may happen that specific Patches don’t comply
with the idea of Patch Management. It becomes necessary to keep these
Patches out from the IT infrastructure which might cause more trouble
than any good.

The tool has the provision to seek Approval for each and every Patch
before they can be deployed. There are two methods for Approval: Manual
Approval and Automatic Approval (Automatic Patch Test). Which method to
choose is decided from the Patch Approval Setting in Admin.

Patch Approval Setting (Selecting an Approval Method)
-----------------------------------------------------

.. note:: Configuring Patch Approval Settings requires Admin rights.

-  Go to **Admin** (accessed from **Product Launcher**) >> **Patch
   Approval Setting** (Patch/Package Deployment).

-  The Patch Approval Setting page opens. There you get three options
   (Approval Types). Click on **Edit** to make the page editable.

    .. _adf-133:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-133.png
        :align: center
        :alt: figure 133

    a. **All Patches Pre-Approved**: As the name suggests, all incoming
       Patches (both new and missing Patches) are Pre-Approved by default. A
       user can manually change the Approval status of Patch to Reject or
       Approved. The Automatic Patch Test doesn’t work with this selection.

       This selection comes into effect for incoming future Patches, and it
       doesn’t affect Patches that are already in the product.

    b. **All Patches will be Manually Approved**: All new incoming Patches
       have the Approval status **Not Approved** by default. A user has to
       change the status manually to either Approved or Reject.

    c. **Qualified Patches will be Approved by Test Task**: All new incoming
       Patches have the status **Not Approved** by default. A user can
       manually set the status. He also has the option to create a Test
       Task.

       A Test Task, also known as Automatic Patch Test, deploys a selected
       set of Patches to a specific set of Computers; if deployment is
       successful in all of the Computers, then the Patches are
       auto-approved after a set number of days. Test Task only works in
       this setting.

-  Select an Approval Type and hit **Update**.

Remote Office
=============

Modern organizations are geographically dispersed. They have offices at different locations all controlled from a main office. Offices that are
away from the main office are termed as Remote Offices. It may happen that all the offices of an organization form part of a single 
network. Individual offices may have a relay server: A relay server is used to allow communications from outside a company's firewall 
to the internal Servers.  

In order to accommodate such situations, we have the following Remote Automation features:

- A user can create a group of computers for a location and save it as a Remote Office. 

- A user can add a Remote Office in a scope (Endpoint Scope) instead of individual computers for Patch/Package/Registry Management.

- Users can point a Remote Office to a relay Server. This is useful when there are multiple offices, and the admin doesn't want them
  to hog the central :ref:`File Server <File Server Installation Guide>` for Patch/Package download. This is why we have the feature that allows a Remote Office to download Patches/Packages from a 
  Relay Server rather than the central File Server. 

Learn More about :ref:`Remote Office`.

.. _ad-batch-deployment:

Batch Deployment
================

When deploying Patches/Packages over a large number of computers, it may cause unwanted consumption of network bandwidth. We have created Batch Deployment
to overcome this problem. 

Batch Deployment allows you to deploy Patches/Packages in a specific number of PCs at a time. Batch Deployment is by default turned off. 

Some of the Benefits of Batch Deployment are:

- Effective usage of an organization's internal bandwidth.

- Drives down the need for high-cost hardware updates to increase local network bandwidth.


**To Configure Batch Deployment:**

- Go to **Admin** (A Navigation Tab) >> **Batch Deploy Configuration** (Patch/Package Deployment).

- The Batch Deploy Configuration page opens. Here you get the following options:

    .. _P-batch-1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-BATCH-1.png
        :align: center
        :alt: figure 1
  
  a. During a Patch/Package Deployment cycle, the deployment process is broken down into smaller units. For example; deployment in 100 computers
     can be divided into 25 computers at a time; at a time, only 25 computers will receive the deployment command. The **Batch Size**
     decides the size of each unit.

  b. Batch Interval is the time between two Batches (units). For example; you can deploy Batches every 2 hours. 

  c. The Max Time Out decides how long the system would wait before considering a computer as failed in deployment. Failed computers are
     removed from a batch and replaced with computers next in line. 

     During a deployment each computer receive a limited number of commands. If a computer fails to deploy within the given number of 
     commands or exceeds the max time out time then it is deemed as failed.

- When done, click on **Update** to save your changes. 


