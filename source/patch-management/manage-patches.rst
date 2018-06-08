********************
Working with Patches
********************

.. _patch-list-view:
Patch List View
===============

The UI is divided across Patch and Computer. The Patch aspect lets you
view patches and perform related operations, and the Computer aspect
lets you view Computers and perform related operations.

The Patch aspect is made up of two types of views: the Patch List View and
Details View. The Patch List View gives a point & click interface to
manage all patches from a single place. The view is divided across
Windows and Linux platform. You can view Patches of any one platform at a
time.

**To open Patch List View**

-  Log in to your Dashboard.

-  Click on the Launcher icon and select **Patch**.

-  Now choose a platform: either Windows or Linux. Based on your
   selection Patches are shown.

.. _pf-15.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-15.1.png
   :align: center
   :alt: figure 15.1
.. _pf-15.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-15.2.png
   :align: center
   :alt: figure 15.2
.. _pf-15.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-15.3.png
   :align: center
   :alt: figure 15.3

.. _pf-16:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-16.png
   :align: center
   :alt: figure 16

::  
    .. note:: Please refer to :numref:`pf-16` for the below description.

-  Section A, B, C & D are the :ref:`Search Features <search-patches>`.

-  Section-E is the list area where you can view all the Patches in the
   system. You can see the following information about a Patch here:

   a. **Patch ID**: This is a system generated ID by Flotomate.

   b. **Name**: The name of the Patch.

   c. **KB ID**: This is a unique ID given by the Software Vendor.

   d. **Severity**: This signifies the importance of a Patch, and the
      Software Vendor provides it.

   e. **Application**: Refers to the application/OS for which a Patch is
      meant.

   f. **Category**: These are pre-defined categories done by the
      Software Vendor.

   g. **Installed System**: The total number of installation done in
      various Nodes.

   h. **Download Size**: The size of a Patch.

-  On this page, you can perform Deployment, Approval and Ignore of
   Patches as bulk operations. In the list area, selecting one or more
   Patches makes the options visible.

.. _pf-17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-17.png
   :align: center
   :alt: figure 17

::
    The Deploy button lets you create a Deployment Request for the chosen
    Patches.

    The Approve button approves the selected Patches. Only approved Patches
    can be deployed.

    The Ignore button marks the selected Patches as Ignored, which means it
    is excluded from all the processes in the system, and they appear only
    under the Ignored tab. Learn more about :doc:`Ignored Patches <ignore-patch>`.

.. _quick-glance-patch:
Quick Glance of Patch Details
=============================

The Patch List View allows you to quickly glance the details of a Patch
in the following way:

-  Open the :ref:`Patch List View <patch-list-view>`.

-  You can open the Patch Details dialog box of any Patch by clicking on
   the view icon adjacent to a Patch.

.. _pf-18:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-18.png
   :align: center
   :alt: figure 18

-  The Patch Details dialog box is a concise version of the :ref:`Details
   View <patch-details-view>`. You get all the information minus the
   features and description.

.. _pf-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-19.png
   :align: center
   :alt: figure 19

.. _search-patches:
Search for a Patch
==================

There are two broad ways to search Patches in the product’s :ref:`List
View <patch-list-view>`:

-  Using Search Bar

-  Using Filters

.. _search-bar-list-view:
Search Bar
----------

The way the search bar works is same across all the platforms (Windows
and Linux). The only difference being is the available search options in
each category.

You can use a search bar to search Patches in the :ref:`List
View <patch-list-view>`. The search bar supports the
Advanced Search feature where you get a set of predefined search options
to narrow down your searches. If you want to see all the available
options, then click on the search box. You can select a single option or
multiple options from the drop-down list.

.. _pf-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-20.png
   :align: center
   :alt: figure 20

You can also search Patches with keywords in the search field. When you
provide a keyword, Flotomate explores all the Patches with the keyword
in their Name, Description, Bulletin ID and KB ID. A Patch has to have
at least one field matched (partial or full) with the keyword; in case
there are multiple keywords, the Patch has to have at least one field
matched for each keyword.

A search query can be made up of pre-defined options and keywords. In
any case, the output yields Patches that satisfy all the parameters of
the search query.

Between two different conditions of the same option type OR logic is
followed. Between different types AND logic is observed. Between
keywords, and keywords and conditions AND logic is followed. An example
of same option type contradiction is Severity Equals Important vs.
Severity Equals Critical.

.. _pf-21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-21.png
   :align: center
   :alt: figure 21

.. _custom-filter-list-view:
Custom Filters
^^^^^^^^^^^^^^

You can make a filter using search options and keywords and save it by
clicking on the star icon to the far left of the search bar. Saved
search filters appear along with the platform filter in :numref:`pf-22.1`.
Custom filters are specific to a particular platform.

For example, a user saves a search query that filters Patches with
severity **Important** and the keyword Net Framework in the Name.

.. _pf-22.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-22.1.png
   :align: center
   :alt: figure 22.1
.. _pf-22.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-22.2.png
   :align: center
   :alt: figure 22.2

.. _filters-patch-list:
Filters
-------

You can search for a Patch in the :ref:`List
View <patch-list-view>` using Quick Filters. Flotomate
gives you three types of Quick Filters:

-  Platform-specific custom filters (either for Windows or Linux).

-  Status-based filter.

-  Severity type based filter.

You can filter the Patches by platform (Windows or Linux). All :ref:`custom
filters <custom-filter-list-view>` appear in their respective
platform-specific filter list.

.. _pf-23.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-23.1.png
   :align: center
   :alt: figure 23.1
.. _pf-23.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-23.2.png
   :align: center
   :alt: figure 23.2

You can pin a custom filter using the Pin Icon. The pinned filter is
applied by default whenever someone clicks on Patch and goes to the
:ref:`List View <patch-list-view>`.

Another way to filter Patches is by using status:

-  **All**: Refers to all available Patches in the system.

-  **New**: These are newly discovered Patches on which no action has
   been taken.

-  **Installed**: Refers to Patches that have already been deployed and
   installed.

-  **Missing**: Refers to Patches that Computers ought to have installed
   but still being demanded, then they are highlighted as Missing. Learn
   more about :ref:`Missing Patches <what-is-missing-patch>`.

-  **Ignored**: Refers to all Patches that have been tagged as Ignore.

.. _pf-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-24.png
   :align: center
   :alt: figure 24

You can also filter Patches based on their severity label:

-  Critical

-  Moderate

-  Important

-  Low

-  Unrated

.. _pf-25:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-25.png
   :align: center
   :alt: figure 25

The severity labels are assigned by the Software Vendor based on their
criteria

.. _patch-details-view:
Patch Details View
==================

The UI is divided across Patches and Computers. The Patch aspect lets
you view patches and perform related operations, and the Computer aspect
lets you view Computers and perform related operations.

The Patch aspect is made up of two views: the Patch List View and
Details View. The Details View shows essential details about a Patch and
gives access to Patch related functionalities.

**To open the Details View of Patch:**

-  Go to the :ref:`Patch List View <patch-list-view>`.

-  Click on a Patch from the list area to open its Details View.

.. _pf-26:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-26.png
   :align: center
   :alt: figure 26

.. _pf-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-27.png
   :align: center
   :alt: figure 27

-  Section-A identifies the Patch. It starts with the Patch ID then the
   Name and ends with the KB ID. None of them are editable.

-  Section-B shows the details of the Patch. The information shown in
   this section is deemed as critical, and the same information
   (excluding description) is available when you are glancing the
   details of a Patch from the :ref:`List View <quick-glance-patch>`. The data points that are
   shown are as follows:

   a. Severity information as stated by the Software Vendor.

   b. The related OS platform of the Patch.

   c. The related application name of the Patch.

   d. The Update category as provided by the Software Vendor.

   e. The Approval status of the Patch. It can be either Approved or
      Not-Approved. You can choose the method of Approval from Approval
      settings in the Admin.

   f. The Test Status which shows the result of an Automatic Patch Test.

   g. The KB ID of the Patch fetched from the update servers.

   h. Information about whether the Patch requires a reboot after
      installation.

   i. Information about whether the Patch supports uninstallation.

   j. The Download size of the Patch.

   k. The release date of the Patch.

-  Section-C shows you the description of the Patch. It is fetched from
   the update server.

-  Section-D gives you four features which are as follows:

   a. In the **Computer** tab, you can view all associated Computers
      that have performed or about to perform certain operations with
      the Patch. The Computers are divided across three categories:

      i.   **Available**: Shows all the Computers that are yet to deploy
           the Patch.

      ii.  **Installed**: Shows the Computers that have installed the
           Patch.

      iii. **Missing**: Shows the Computers that were supposed to have
           the Patch but they do not have the Patch. Learn more about
           :ref:`missing Patches <what-is-missing-patch>`.

      iv.  **Ignored**: Shows in how many Computers the Patch is
           ignored.

.. _pf-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-28.png
   :align: center
   :alt: figure 28
.. _advanced-search-computer:
::
    ::
        ::
            The tab provides a search bar for searching Computers. The search bar
            supports the Advance Search feature where you get search options by
            clicking on the search bar.

.. _pf-29:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-29.png
   :align: center
   :alt: figure 29

.. _pf-30:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-30.png
   :align: center
   :alt: figure 30

::
    ::
        ::
            You can also enter keywords to search for a Computer. When entering a
            keyword, the product explores all the Computers with the keyword in
            their Name, Hostname, Domain name, OS name and Service Pack. A Computer
            has to have at least one field matched (partial or full) with the
            keyword; in case there are multiple keywords, a Computer has to have at
            least one field matched for each keyword.

            You can combine search options with keywords. Between two different
            conditions of the same type OR logic is followed. Between different
            types AND logic is observed. Between keywords, and keywords and
            conditions AND logic is followed. An example of same type contradiction
            is OS Name contains Windows vs. OS Name contains Linux.

.. _pf-31:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-31.png
   :align: center
   :alt: figure 31

    b. In the **Affected Products** tab, you can view which application/OS
        is affected by the Patch.

    c. In the **Download URL** tab, you can view the download location of
        the Patch. You can also download the Patch file locally onto a
        machine using the **Download** button.

    d. In the **Deployment Status tab**, you can view all the associated
        Deployment Requests and their statuses. A Patch can be associated
        with multiple Deployment Requests, and the status shows two essential
        things: download status of the Patch (in the shared drive) and the
        installation status in the Computers.

-  Section-E houses the following options:

   a. The **Approve/Reject** button for manual approval of a Patch.

   b. You can directly open the Create page for deployment with the
      Patch preselected using the **Deploy** button.

   c. The Action menu is where you can :ref:`Configure Package <configuring-package-location-single-patch>` location and **Ignore/Un-Ignore** the Patch.