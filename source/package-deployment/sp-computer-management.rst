*******************
Computer Management
*******************

Computers are pingable IT Assets that are capable of running our Agent
application. Computers communicate with the main server (product)
through the Agent and update the main server with Patch info, and fetch
instruction for deployment (installation) of Patches, Packages, and
Registry.

You have complete control over Computers with respect to the following:

-  What Packages/Registry entries to deploy?

-  How to deploy the Packages (:doc:`Deployment Policy <sp-setting-up-a-deployment-policy>`).

Package Deployment shows you vital info about the Computers with respect
to the following:

-  What Packages are associated with a Computer?

-  A Computer is receiving instruction from how many Deployment Request?

-  Connection status of a Computer with the main server.

.. _sp-computer-list-view:

Computer List View
==================

The UI is different for Computers and Packages. We have already covered
the Package aspect of the tool. Now we are going to talk about the
Computer aspect.

The Computer aspect is made up of two types of views: the Computer List
View and Computer Details View. The Computer List View shows all the
Computers that are available in the system.

1. Log in to your Dashboard.

2. Go to **Deployment** from the **Launcher**.

.. _spf-61:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-61.png
    :align: center
    :alt: figure 61

3. Click on All Computers from the Package menu.

.. _spf-62:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-62.png
    :align: center
    :alt: figure 62

4. The Computer List View opens.

.. _spf-63:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-63.png
    :align: center
    :alt: figure 63

-  Section A & B (:numref:`spf-63`) are the :ref:`search features <sp-searching-computers>`. Section A also segregates computers
   based on :ref:`sp-computer-health-management`. 

-  Section C is the list area where you view all Computers. You can view
   the following information about a Computer:

   a. Computer ID is given by the Main Server.

   b. Hostname of the Computer.

   c. The OS platform of the Computer.

   d. The architecture of the Computer.

   e. Service Pack Details.

   f. Domain Details

   g. IP address of the Computer

   h. Version of the Agent application.

-  Section D is where you can control the number of Computers visible on
   a page. You can set a default number from the Preference section.

Active Status of a Computer
===========================

The tool has a marker that tells whether a Computer is active or
offline. Wherever you see Agent information in the tool, you can see
the associated marker. The marker has two colours: **green** signifying
the Computer is active and communicating, and **yellow** signifying the
Computer is offline.

.. _spf-64.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-64.1.png
    :align: center
    :alt: figure 64.1

.. _spf-64.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-64.2.png
    :align: center
    :alt: figure 64.2

.. _sp-searching-computers:

Searching Computers
===================

There are two broad ways to search Computers in the tool’s :ref:`List View <sp-computer-list-view>`:

-  Using the Search Bar

-  Using Filters

.. _search-bar-2:

Search Bar
----------

There is a search bar for searching Computers in the :ref:`Computer List
View <sp-computer-list-view>`. The search bar supports the Advanced
Search feature where you get a set of search options to narrow down your
searches. You can access all the available search options by clicking on
the search box. You can build conditions using a single option or
multiple options.

.. _spf-65:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-65.png
    :align: center
    :alt: figure 65

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
Name contains Ubuntu Linux.

.. _filters-2:

Filters
-------

The :ref:`Computer List View <sp-computer-list-view>` has filters that allow
you to view all healthy Computers, Highly Vulnerable Computers, and
Vulnerable Computers. These filters are classifications based on the
health of a Computer. The health of a Computer is ascertained based on
the number of missing Patches. Learn more about :ref:`Computer Health
Management <sp-computer-health-management>`.

Computer’s Details View
=======================

The UI is different for Computers and Packages. We have already covered
the Package aspect. Now we are going to talk about the Computer aspect.

The Computer aspect is made up of two types of views: the Computer List
View and Computer Details View. The Computer Details View is Computer
specific which means every Computer in the system has a Details View
that shows additional information and provides deployment options.

-  Go to the :ref:`Computer List View <sp-computer-list-view>`.

-  Click on a Computer from the list area to open its Details View.

.. _spf-66:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-66.png
    :align: center
    :alt: figure 66

-  Section-A shows the identity of the Computer. It starts with the
   Computer ID and then the Computer Name. It also shows additional
   information about the Computer. You can see the platform, OS details,
   IP address ,hostname of the Computer, Architecture, Remote Office
   details, Vendor and Domain Name

-  Section-B gives you two tabs to view all related Patches and
   Deployment Requests:

   **Patches:**

    .. _spf-67:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-67.png
        :align: center
        :alt: figure 67

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
       for the Computer, Learn more about :ref:`Ignored Patches <Ignoring_a_Patch_1>`.

   In each category, you can use a search bar to search for Patches. The
   search bar works in the same way as the one on :doc:`Patch List
   View <patch-list-view>`.

   You can access the Details View of a Patch by clicking on it.

   **Deployment Status:**

    .. _spf-68:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-68.png
        :align: center
        :alt: figure 68

   In this tab, you can view all Deployment Requests that are giving
   Patch/Package/Registry Deployment instructions to the Computer. You also
   view their :ref:`statuses <sp-deployment-status>`.

- Section-C is where you can deploy/uninstall patch and packages.

.. _sp-computer-health-management:

Computer Health Management
==========================

Patch Management ensures that all administered IT Assets are updated with the
latest Patch from the Software Vendor; this enhances security and helps
in thwarting external and internal cyber-attacks.

Computers fetch and deploy Patches. So it becomes imperative to monitor
all Computers to keep yourself aligned with the idea of Patch
Management.

System Health Settings flags Computers that are missing critical, essential Patches. This helps you to manage your
vulnerability and prevent any attacks.

You can filter computers based on System Health from the Computer List View. 

.. _spf-68.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-68.1.png
    :align: center
    :alt: figure 68.1

Learn how configure :ref:`system-health-settings`. 
