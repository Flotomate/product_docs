******************
Deployment Request
******************

Introduction
============

A Deployment Request is a set of instructions for Computer/Computers.
The Admin creates it, or anyone with the rights, to initiate a
deployment cycle. A Deployment Request mainly contains the following
information:

-  **Request details**: Defining the installation criteria.

-  **Package details**: Installation of which Packages?

-  **Computer details**: Computers that are going to install the
   Packages.

Learn how :ref:`Deployment Requests <adding-a-package-deployment-request>`
are created.

All Computers ping the Flotomate server periodically to check for
available Deployment Requests. On finding a Deployment Request,
Computers/Computer can acquire the Packages from the Shared Drive or a
Remote URL, and install them following a Deployment Policy. A single end
to end process of fetching and installing/deploying Packages or registry
values is called Deployment Cycle.

Adding a Package Deployment Request
===================================

Currently, all package deployment requests are created by users. To
create a deployment request:

1. Click on the Launcher icon and select **Package**.

2. Select **Deployment Request** from the Package menu.

.. _spf-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-32.png
    :align: center
    :alt: figure 32

3. The Deployment Requests page opens. Here you can view all available
   requests in the product. Click on **Deploy Packages** situated in
   the top right corner of the page.

4. The Create page opens. The page is divided into three sections; they
    are as follows:

    a. **Request Details**:

        .. _spf-33:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-33.png
            :align: center
            :alt: figure 33

        i. **Name**: You can provide a name to the Deployment Request instead
           of the default placeholder. It is advisable to keep the date part
           of the placeholder.

        ii. **Platform**: Select the platform for which you are deploying
            Package/Packages. Currently, we support only Windows and Linux.

        iii. **Deployment Policy**: Select a Deployment policy from the
             drop-down list. A Deployment Policy governs how the deployment of
             Packages is carried out. Learn about :doc:`Deployment
              Policies <sp-setting-up-a-deployment-policy>`.

        iv. **Install After**: Provide a date and time after which the request
            tells the Computers to commence the installation process

        v.  **Expire After**: This is the date and time after which the
            request ceases to be a valid request.

    b. **Select Package**: Here you add the Package/Packages that you want to deploy.

        .. _spf-34:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-34.png
            :align: center
            :alt: figure 34

        i. Section-A (:numref:`spf-34`) is the area where you view the selected
           Packages.

        ii. Section-B has a search bar for searching all available Packages
            for the selected OS. The search bar supports the Advanced Search
            feature. Learn how to use Advanced Search (refer to how search
            works in :doc:`Package List View <package-registry-list-view>`).

        iii. Section-C is where you view the available Packages in the main
             server. Clicking a checkbox selects a Package and transfers it to
             section-A.

      Select the Packages that you want to deploy.

    c. **Select Target**:

        .. _spf-35:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-35.png
            :align: center
            :alt: figure 35

       Target refers to Computer/Computers where Packages are going to be
       installed. You can select a Computer Group or Groups, or individual
       Computers as a target. You can select both Computer Groups and Computers
       as a target.

       You can create a new group using the **Create Computer Group** button.
       It opens a dialog box where you can create a group; learn :doc:`how to create
       a group <sp-manage-computer-groups>`. You also get a search bar to
       search Computers. The search bar supports the Advanced Search feature.
       Learn how to use :doc:`Advanced Search. <package-registry-list-view>`

    d. **Retry Configuration**:

        .. _spf-36:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-36.png
            :align: center
            :alt: figure 36

       The retry configuration limits the number of times an Agent tries
       deployment when faced with failure.

        i. You can define the maximum number of times to try deployment during
           system start-up.

        ii. You can define the maximum number of times to try deployment once
            at each refresh cycle (by default refresh cycle is set to 1 hour).

     During each retry cycle, the deployment status swings from
     In-Progress to Failed and vice-versa when all cycles fail to deploy
     the packages.

   Fill in all the necessary details. Now you have two options; you
   can publish the request or save it as a draft.

   If you save the request as a draft, then the request appears as
   drafted in the Deployment Requests page. You can view all drafted
   requests using the Quick Filter **Drafted**.

        .. _spf-37:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-37.png
            :align: center
            :alt: figure 37

   If you want to publish the request, then click on **Publish**. This
   might or might not activate the request immediately, depending on Custom
   Rules. If Deployment Custom Rules (refer Admin Manual) demand Approval,
   then you have to seek Approval before you can publish the Request.

   You can publish a drafted request from its Update page (clicking on a
   request opens it in edit mode), or you can click on the publish button
   adjacent to a request.

Other Ways to Add a Deployment Requests
=======================================

Adding a Deployment Request from the Package/Registry List View:
----------------------------------------------------------------

Our product allows you to select a Package/Packages from the List Page
directly and deploy them.

1. Go to the :doc:`Package List View <package-registry-list-view>` of
   either Windows or Linux.

2. Select a Package or Packages from the list area. A **Deploy** button
   appears above the list area.

.. _spf-38:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-38.png
    :align: center
    :alt: figure 38

3. Click on **Deploy** which opens the
   :ref:`Create <adding-a-package-deployment-request>` page. Use the page
   to create the request. The dialog box has the Package/Packages
   preselected.

Adding a Deployment Request from a Computer’s Details Page:
-----------------------------------------------------------

1. Go to the Computer List Page.

2. Click on a Computer. This takes you to the Details Page.

3. Click on **Deploy Packages** from the Action Menu.

.. _spf-39:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-39.png
    :align: center
    :alt: figure 39

4. :ref:`Create <adding-a-package-deployment-request>` page for request
   opens. Create your request and publish it, or you can save it as a
   draft.

Approval
========

In case there is a custom rule (Refer admin manual for Patch Custom
Rules) defined, then you have to make every drafted request go through
an Approval process before publishing it. In an Approval process, you
seek approval from a set of approver/approvers.

Asking for an Approval:
-----------------------

-  Go to the :doc:`Deployment Request <sp-deployment-request>` page.

-  Click on the Quick Filter **Drafted** to sort all drafted requests.

.. _spf-40:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-40.png
    :align: center
    :alt: figure 40

-  You can initiate an Approval process for a request by click on the
   adjacent **Ask for Approval** button.

.. _spf-41:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-41.png
    :align: center
    :alt: figure 41

Different States in an Approval
-------------------------------

-  Pending:

-  Rejected:

-  Pre-Approved:

-  Approved:

Approval Process:
-----------------

-  First, the system checks all available Approval Workflows when an
   Approval is asked. If there are no workflows or the present workflow
   conditions are not meet, then the drafted request/requests are
   Pre-Approved, and you can proceed with publishing. If there is a
   workflow/are workflows, and their conditions are met, then
   approver/approvers are auto-assigned for each request.

   When there are multiple requests, it may happen that some may trigger
   the Approval conditions and are put in Approval, and some may not
   trigger the conditions and are Pre-Approved.

.. _spf-42:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-42.png
    :align: center
    :alt: figure 42

-  When you **Ask for Approval** for a request, an **Approval** button
   appears adjacent to the request. The button gives you access to the
   Approval details dialog box where you can view all the approvers and
   their comments and even re-ask for an Approval (this again checks for
   all available workflows).

    .. _spf-43:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-43.png
        :align: center
        :alt: figure 43

   For requests that have Approvers, the Approval Status changes to
   Pending, and it stays there as long as the approver/approvers don’t
   express a decision.

-  An approver can see his Approvals in the **My Approvals** section of
   his account.

    .. _spf-44:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-44.png
        :align: center
        :alt: figure 44

   Clicking on **My Approvals** (:numref:`spf-44`) opens the My Approval page
   where he can view his Approvals.

    .. _spf-45:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-45.png
        :align: center
        :alt: figure 45

   Clicking on an Approval in **My Approval** opens a new page. There he
   can perform the following actions:

    .. _spf-46:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-46.png
        :align: center
        :alt: figure 46

    a. View request details, target Packages, and Computers.

    b. Start a comment thread.

    c. Approve or Reject the Approval.

-  The outcome of an Approval process is decided in two ways:

   a. **Unanimous**: All of the Approvers have to approve else the
      Approval is rejected.

   b. **Majority**: If the majority of Approvers agree then Approval is
      successful.

      In case there are multiple Approvals, the decision to go with
      unanimous or majority can be set from **Admin** (A Navigation Tab)
      >> **Approval Workflow** (Automation) >> **Approval Settings**,
      but the rights to do it lies with the Super Admin.

-  On success, the Approval moves to the Approved stage where the author
   can publish the draft. On failure, the Approval moves to the Reject
   stage where the author has to reinitiate the Approval process. The
   author reinitiates an Approval process using the **Re-Approve**
   option. A **Re-Approve** puts a request back to the pending stage.

.. _spf-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-47.png
    :align: center
    :alt: figure 47

-  Any Technician with the **Can Ignore Approval** right can ignore
   approvers and push the Approval towards the Approved stage; where he
   can publish the draft. The ignored approvers can see their Approval
   status as Ignored in Approval details dialog box of the Article.

.. _spf-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-48.png
    :align: center
    :alt: figure 48

Searching Deployment Requests
=============================

There are two broad ways to search Deployment Requests in the product:

-  Using Search Bar

-  Using Filters

.. _spf-49:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-49.png
    :align: center
    :alt: figure 49

.. _search-bar-1:
Search Bar
----------

In the :doc:`Deployment Request <sp-deployment-request>`
page, you get a search bar to search through requests. The search bar
supports the Advanced Search feature where you get a set of search
options. Click on the search bar to access all search options.

.. _spf-50:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-50.png
    :align: center
    :alt: figure 50

In some options, you have to enter a value, and in others, there are
predefined values. You can create conditions using multiple options.
Between two different conditions of the same option type OR logic is
followed. Between different types AND logic is observed. An example of
same option type contradiction is Platform equals Windows vs. Platform
equals Linux.

.. _spf-51:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-51.png
    :align: center
    :alt: figure 51

.. _filters-1:

Filters
-------

You can search for requests in the Deployment Request page using Quick
Filters. There three types of filters available:

-  Filters based on time of deployment.

-  Filters based on publishing status.

-  Filters based on origin.

.. _spf-52:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-52.png
    :align: center
    :alt: figure 52

Section-A (:numref:`spf-52`) is a quick filter to toggle across the following
views:

-  **Current**: Shows all the published and drafted requests that can
   start the deployment process immediately.

-  **Future**: Shows all the published requests that can start the
   deployment after a future date and time.

-  **Past**: Shows all the requests that have expired.

-  **Drafted**: Shows all drafted requests that are yet to be published.

-  **Archived**: Shows requests that have been deleted, includes drafted
   requests.

Section-B (:numref:`spf-52`) allows you to filter request based on origin and
Approval status. There is one possible origin to a Deployment Request,
and the Approval status shows both Approved and Pre-Approved requests.

-  :doc:`Manually <sp-deployment-request>`

Managing Deployment Requests
============================

.. _sp-deployment-status:
Deployment Status
-----------------

In the Deployment Request page, every published request has a Status
button.

.. _spf-53:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-53.png
    :align: center
    :alt: figure 53

Using the Status button, you can check the Deployment Status of all
associated Computers.

Clicking on a **Status** button opens a new page where you can view all
associated Computers that are going to deploy the Package/Packages.

Each computer has a **Deployment Status** button which opens a dialog
box where you can view the installation statuses of each Package.
Computer transitions through various statuses when installing a Package.
Some of the statuses reflect a stage, and some are conclusions.
Altogether there are six statuses:

.. _spf-54:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-54.png
    :align: center
    :alt: figure 54

.. _spf-55:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-55.png
    :align: center
    :alt: figure 55

-  **Yet to Receive**: The Computer is yet to receive instructions from
   the request to install the Package.

-  **In Progress**: The Computer is in the process of installing the
   Package after receiving the instructions.

-  **Success**: The Computer has successfully installed the Package.

-  **Failed**: The Computer has failed to install the Package.

-  **Cancelled**: The request was deleted before the Computer could
   receive the instructions for installation.

-  **Not Applicable**: The Package is not meant for the Computer.

Unsupported Computers in a Deployment
-------------------------------------

During deployment it may happen that certain target Computers don’t
support all the Packages; in that case, the **Not Applicable** status is
helpful.

Go to the **Status** of a request. Click on the **Deployment status** of
a Computer; there the Packages that don’t support the Computer have the
**Not Applicable** status.

.. _spf-56:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-56.png
    :align: center
    :alt: figure 56

Edit/Archive a Deployment Request:
----------------------------------

You can update Deployment Requests that are in draft mode. Once
published, a request cannot be edited.

-  Go to the :doc:`Deployment Request Page <sp-deployment-request>`.

-  The **Status** button adjacent to a request shows that the request is
   a published request.

-  You can open a request in edit mode by clicking on it or by clicking
   the Edit icon.

.. _spf-57:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-57.png
    :align: center
    :alt: figure 57

**Archiving**

The product allows you to delete published and drafted Deployment
Requests. You can delete multiple requests at a time.

-  Go to the :doc:`Deployment Request <sp-deployment-request>` page from the
   Package Menu.

-  Select one and more requests. The **Archive** button appears.

.. _spf-58:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-58.png
    :align: center
    :alt: figure 58

-  Click on the **Archive** button. On confirmation, the
   request/requests are deleted.

**Deleting an Active Deployment Request:**

Deleting a published request has the following effects:

-  Installation of Packages is canceled in Computers that are yet to
   receive instructions.

View Archived Deployment Requests
---------------------------------

You can view an archived request along with its status. An archived
request may have partially finished operations that might need scrutiny.
To view an archived request:

-  Go to the :doc:`Deployment Request <sp-deployment-request>` page.

-  Select **Archived** from the Quick Filter section.

.. _spf-59:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-59.png
    :align: center
    :alt: figure 59

-  Now you can view all archived requests. Use the **Status** button to
   view :ref:`deployment status <sp-deployment-status>`.

.. _spf-60:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-60.png
    :align: center
    :alt: figure 60
