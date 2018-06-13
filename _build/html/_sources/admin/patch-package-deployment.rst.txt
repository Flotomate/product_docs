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

Share Drive Configuration
=========================

A Shared Drive is a shared resource on a Computer network. It is a
device or piece of information on a Computer that can be remotely
accessed from another Computer, typically via a local area network or an
enterprise intranet, transparently as if it were a resource in the local
machine.

The Shared Drive is the default location where the Product Server stores
all the Patches before deployment. The product asks for a Shared Drive
when Patches don’t have a locally stored Package file.

**To Setup a Shared Drive:**

1. Log in to your Dashboard.

2. Go to **Admin** (accessed from **Product Launcher**) >> **Shared
   Drive Configurations** (Patch/Package Deployment).

.. _adf-117:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-117.png
    :align: center
    :alt: figure 117

3. The Shared Drive Configuration page opens. Here you get the
   following fields and options:

    .. _adf-118:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-118.png
        :align: center
        :alt: figure 118

    a. In section-A (:numref:`adf-118`), you type in a URL that tells the Product
       Server the location of the Shared Drive.

    d. If you want the Patches to be automatically downloaded when there’s a
       request, then turn on the toggle button in section-B.

   Click the **Edit** button to make the fields editable. Once you enter
   the URL, you can test the connection; the product tells you whether a
   successful connection was established with the Share Drive. Once you
   are done with everything, click on **Update** to save your changes.

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

System Health Settings
----------------------

Go to **Admin** (Accessed from **Product Launcher**) >> **System Health
Settings** (Patch/Package Management).

.. _adf-119:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-119.png
    :align: center
    :alt: figure 119

These settings help Flotomate to flag Computers as either Highly
Vulnerable or Vulnerable. You can filter the flagged Computers on the
:ref:`Computer List View <computer-management/computer-list-view>`. Clicking on **System Health
Settings** opens a page. Here you can set the conditions separately to
define Highly Vulnerable and Vulnerable.

.. _adf-120:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-120.png
    :align: center
    :alt: figure 120

Click on **Edit** to make the fields editable. You are expected to enter
the minimum number of missing Patches for each severity label.

Each vulnerability status has a set of four severity labels and their
counts. No two same labels can have the same numbers (Numbers in Highly
Vulnerable have to be higher than Vulnerable).

.. _adf-121:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-121.png
    :align: center
    :alt: figure 121


The number zero in a field signifies that there’s no condition for the
corresponding severity label.

If a Computer has a missing Patch number that is equal to or exceeds a
minimum value for a label, then the Computer is flagged with the
corresponding health status. In case a Computer satisfies multiple
labels then the label top in the hierarchy is considered (Critical
Patches having the highest priority and Low severity having the lowest).

.. _adf-122:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-122.png
    :align: center
    :alt: figure 122

Endpoint Scope
==============

Depending on the License agreement you have with us, the number of
Computers you can manage with the product (for remote deployment) is
limited. All discovered Computers (with our Agent application) stay out
of the scope of the product by default; you have to bring them within
the scope before you can use our product features.

The Endpoint Scope lets you view all available Computers (not in the
Scope) and add them to the Scope. You can set certain conditions that
allow the product to add any new Computers automatically. You can also
add Computers manually.

There is a counter that shows how many Computers are within the scope
and how many you can still add. In no situation, you can exceed the
total number of Computers you are allowed to add to the Scope.

.. note:: Only Computers configured with our Agent Application is visible
          on Endpoint Scope.

Add Computers to a Scope
------------------------

-  Go to **Admin** (accessed from **Product Launcher**) >> **Endpoint
   Scope** (Patch/Package Management).

.. _adf-123:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-123.png
    :align: center
    :alt: figure 123

-  The Endpoint Scope page opens.

.. _adf-124:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-124.png
    :align: center
    :alt: figure 124


-  You can view the total number of Computers that you can add from the
   Total Endpoint Scope number. The Total Available shows you the number
   of Computers you can still add to reach the Total Endpoint Scope
   number.

.. _adf-125:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-125.png
    :align: center
    :alt: figure 125


**Adding a Network (Automatic Addition of Computers)**

-  You can associate a Network with a Scope; this allows the Scope to
   automatically add Computers (with the Agent application) in the
   Network based on include and exclude conditions. You can use both
   manual and automatic addition of Computers together; they are not
   mutually exclusive.

.. _adf-126:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-126.png
    :align: center
    :alt: figure 126


-  Once you select a Network, you now have to add conditions. The
   conditions are of two types: include and exclude. Both the types
   create a set of Computers from which to either include or exclude.
   When there’s an intersection or conflict between the two types then
   exclude conditions/condition override the include set. For example,
   to add Computers within an IP range with a hostname containing “Digi”
   and excluding those with Linux OS, yields the following conditions:

.. _adf-127.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-127.1.png
    :align: center
    :alt: figure 127.1

.. _adf-127.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-127.2.png
    :align: center
    :alt: figure 127.2


**Manual Adding Computers**

-  You can manually search and add Computers to a scope. The search bar
   supports the Advanced Search feature where you get search options by
   clicking on the search bar.

    .. _adf-128.1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-128.1.png
        :align: center
        :alt: figure 128.1

    .. _adf-128.2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-128.2.png
        :align: center
        :alt: figure 128.2


   You can also enter keywords to search for a Computer. When entering a
   keyword, the product explores all the Computers with the keyword in
   their Name, Hostname, Domain name, OS name and Service Pack. A Computer
   has to have at least one field matched (partial or full) with the
   keyword; in case there are multiple keywords, a Computer has to have at
   least one field matched for each keyword.

   You can combine search options with keywords. Between two different
   conditions of the same type OR logic is followed. Between different
   types AND logic is observed. An example of same type contradiction is OS
   Name contains Windows vs. OS Name contains Linux.

.. _adf-129:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-129.png
    :align: center
    :alt: figure 129

-  Once you have found your Computers, add by selecting them, and they
   move to the Selected Computers list. Manually selected Computers
   override the exclude criteria/conditions set under the Network.

.. _adf-130:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-130.png
    :align: center
    :alt: figure 130

-  Once you are done setting conditions and adding Computers, click on
   **Update**.

-  You can create more than one Scope to accommodate multiple Networks
   (a Scope can have only one Network). The actual Computer list is
   cumulative of all available Scopes (added manually and
   automatically).

.. _adf-131:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-131.png
    :align: center
    :alt: figure 131

Preview Computer List
---------------------

Once you are done with adding Computers and setting conditions, you can
view the final list of all the Computers (added manually and
automatically) in all Scopes using the Preview function.

Open Endpoint Scope from **Admin**. Click on **Preview** to generate the
Computer list.

.. _adf-132:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-132.png
    :align: center
    :alt: figure 132

You can search for a Computer. The search bar supports the Advanced
Search feature. It is similar to the search bar in a Scope.

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