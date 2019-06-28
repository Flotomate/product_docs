*******************
Computer Management
*******************
Computers are pingable IT Assets that are capable of running our Agent
application. Computers communicate with the main server (product)
through the Agent and update the main server with Patch info, and fetch
instruction for deployment (installation) of Patches.

You have complete control over Computers with respect to the following:

-  What Patches to deploy?

-  How to deploy the Patches (:doc:`Deployment Policy <deployment-policy>` and :doc:`batch-deployment`).

The product shows you vital info about the Computers with respect to the
following:

-  What Patches are associated with a Computer?

-  A Computer is receiving instruction from how many Deployment Request?

-  Connection status of a Computer with the main server.

.. _computer-list-view:

Computer List View
==================

The UI is different for Computers and Patches. We have already covered
the Patch aspect of the product. Now we are going to talk about the
Computer aspect.

The Computer aspect is made up of two types of views: the Computer List
View and Computer Details View. The Computer List View shows all the
Computers that are available in the system.

1. Log in to your Dashboard.

2. Go to **Patch** from the **Launcher**.

.. _pf-98:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-98.png
   :align: center
   :alt: figure 98

3. Click on All Computers from the Patch menu.

.. _pf-99:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-99.png
   :align: center
   :alt: figure 99

4. The Computer List View opens.

.. _pf-100:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-100.png
   :align: center
   :alt: figure 100

-  Section A & B (:numref:`pf-100`) are the search features.

-  Section C is the list area where you view all Computers. You can view
   the following information about a Computer:

   a. Computer ID is given by the Main Server.

   b. Hostname of the Computer.

   c. The platform and OS name of the Computer.

   d. Architecture info either 32bit or 64bit.

   e. Service Pack Details.

   f. Agent Version details

   g. IP address of the Computer

   h. Name of the associated remote office.

-  Section D is where you can control the number of Computers visible on
   a page. You can set a default number from the Preference section.

.. _active-status-computer:

Active Status of a Computer
===========================

The tool has a marker that tells whether a Computer is active or
offline. Wherever you see Agent information in the product, you can see
the associated marker. The marker has two colours: **green** signifying
the Computer is active and communicating, and **yellow** signifying the
Computer is offline.

.. _pf-101.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-101.2.png
   :align: center
   :alt: figure 101.2

.. _searching-computer:

Searching Computers
===================

There are two broad ways to search Computers in the product’s :ref:`List
View <computer-list-view>`:

-  Using the Search Bar

-  Using Filters

.. _search-bar-2:

Search Bar
----------

There is a search bar for searching Computers in the :ref:`Computer List
View <computer-list-view>`. The search bar supports the Advanced
Search feature where you get a set of search options to narrow down your
searches. You can access all the available search options by clicking on
the search box. You can build conditions using a single option or
multiple options.

.. _pf-102:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-102.png
   :align: center
   :alt: figure 102

You can search Computers with keywords in the search field. When you
provide a keyword, Motadata searches all the Computers with the keyword
in their Service Pack, OS Name, Domain Name, Hostname, and Name. A
Computer has to have at least one field matched (partial or full) with
the keyword; in case there are multiple keywords, the Computer has to
have at least one field matched for each keyword.

A search query can be made up of options and keywords. In any case, the
output yields Computers that satisfy all the parameters of the search
query.

Between two different conditions of the same option type OR logic is
followed. Between different types AND logic is observed. Between
keywords, and keywords and conditions AND logic is followed. An example
of same option type contradiction is OS Name contains Windows vs. OS
Name contains Ubuntu.

.. _filters-2:

Filters
-------

The :ref:`Computer List View <computer-list-view>` has filters that allow
you to view all healthy Computers, Highly Vulnerable Computers, and
Vulnerable Computers. These filters are classifications based on
Computer health. The health of a Computer is ascertained based on the
number of missing Patches. Learn more about :ref:`Computer Health
Management <computer-health>`.

.. _computer-details-view:

Computer’s Details View
=======================

The UI is different for Computers and Patches. We have already covered
the Patch aspect. Now we are going to talk about the Computer aspect.

The Computer aspect is made up of two types of views: the Computer List
View and Computer Details View. The Computer Details View is Computer
specific which means every Computer in the system has a Details View
that shows additional information and provides deployment options.

-  Go to the :ref:`Computer List View <computer-list-view>`.

-  Click on a Computer from the list area to open its Details View.

.. _pf-103:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-103.png
   :align: center
   :alt: figure 103

-  Section-A shows the identity of the Computer. It starts with the
   Computer ID and then the Computer Name. It also shows additional
   information about the Computer. You can see the platform, OS details,
   IP address ,hostname of the Computer, Architecture, Remote Office
   details, Vendor and Domain Name

-  Section-B gives you two tabs to view all related Patches and
   Deployment Requests:

   **Patches:**

        .. _pf-104:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-104.png
            :align: center
            :alt: figure 104

        Under this tab, you can view all associated Patches categories into the
        following:

            a. **New Patches**: Shows newly discovered Patches that are yet to be
               deployed by the Computer.

            b. **Installed Patches**: Shows the Patches that have been installed by
               the Computer.

            c. **Missing Patches**: Shows the Patches that are being shown as
               Installed somewhere in the system but the Computer is yet to deploy
               them.

            d. **Ignored Patches**: Shows Patches that have been deemed as ignored
               for the Computer, Learn more about :doc:`Ignored
               Patches <ignore-patch>`.

        In each category, you can use a search bar to search for Patches. The
        search bar works in the same way as the one on :ref:`Patch List
        View <search-bar-list-view>`.

        You can access the :ref:`Details View <patch-details-view>` of a Patch
        by clicking on it.

   **Deployment Status:**

        .. _pf-105:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-105.png
            :align: center
            :alt: figure 105

        In this tab, you can view all Deployment Requests that are giving Patch
        Deployment instructions to the Computer. You also view their
        :ref:`statuses <deployment-status>`.

- Section-C is where you can deploy/uninstall patch and packages.

.. _computer-health:

Computer Health Management
==========================

We have discussed earlier that Patch Management ensures that all
administered IT Assets are updated with the latest Patch from the
Software Vendor; this enhances security and helps in thwarting external
and internal cyber-attacks.

Computers fetch and deploy Patches. So it becomes imperative to monitor
all Computers to keep yourself aligned with the idea of Patch
Management.

Our product has a feature called System Health that flags Computers that
are missing critical, essential Patches. This helps you to manage your
vulnerability and prevent any attacks.

.. _system-health-settings:

System Health Settings
----------------------

Go to **Admin** (A Navigation Tab) >> **System Health Settings**
(Patch/Package Management).

.. _pf-106:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-106.png
   :align: center
   :alt: figure 106

These settings help Motadata to flag Computers as either Highly
Vulnerable or Vulnerable. You can filter the flagged Computers on the
:ref:`Computer List View <filters-2>`. Clicking on **System Health
Settings** opens a page. Here you can set the conditions separately to
define Highly Vulnerable and Vulnerable.

.. _pf-107:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-107.png
   :align: center
   :alt: figure 107

Click on **Edit** to make the fields editable. You are expected to enter
the minimum number of missing Patches for each severity label.

Each vulnerability status has a set of four severity labels and their
counts. No two same labels can have the same numbers (Numbers in Highly
Vulnerable have to be higher than Vulnerable).

.. _pf-108:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-108.png
   :align: center
   :alt: figure 108

The number zero in a field signifies that there’s no condition for the
corresponding severity label.

If a Computer has a missing Patch number that is equal to or exceeds a
minimum value for a label, then the Computer is flagged with the
corresponding health status. In case a Computer satisfies multiple
labels then the label top in the hierarchy is considered (Critical
Patches having the highest priority and Low severity having the lowest).

.. _pf-109:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-109.png
   :align: center
   :alt: figure 109
