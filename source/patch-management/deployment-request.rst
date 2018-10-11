*******************
Deployment Requests
*******************

Introduction
============

A Deployment Request is a set of instructions for Computers (with our
Agent application). The Admin creates it, or anyone with the rights, to
initiate a deployment cycle. A Deployment Request mainly contains the
following types of information:

-  **Request details**: Defining the installation criteria.

-  **Patch details**: Selection of Patches that need deployment.

-  **Computer details**: Selection of Computers that perform deployment
   in their respective nodes.

Learn :ref:`to create a Deployment Request <manually-create-request>` 

All Computers ping the Flotomate server every hour to check for
available Deployment Requests. On finding a Deployment Request,
Computer/Computers can acquire the Patches from the File Server, and
install them following a :doc:`Deployment Policy <deployment-policy>`. 
A Deployment Cycle refers to the end to end process involving getting and installing Patches.

**Methods of Deployment**

There are three ways to create a Deployment Request in the tool:

-  Manually creating a Deployment Request and publishing it.

-  Automatic Patch Deployment creates a Deployment Request (either in
   Draft or Publish).

-  Initiating an Automatic Patch Test which in turn creates and
   publishes a Deployment Request.

.. _manually-create-request:

Manually Creating a Request
===========================

- Click on the Launcher icon and select **Patch**.

- Select **Deployment Request** from the Patch menu.

.. _pf-62:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-62.png
   :align: center
   :alt: figure 62

- The Deployment Requests page opens. Here you can view all available
  requests in the tool. Click on **Deploy Patches** situated in the
  top right corner of the page.

- The Create page opens. The page is divided into four sections; they
  are as follows:

    a. **Request Details**:

        .. _pf-63:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-63.png
            :align: center
            :alt: figure 63

        i.  **Name**: You can provide a name to the Patch instead of the
            default placeholder. It is advisable to keep the date part of the
            placeholder.

        ii. **Deployment Policy**: Select a Deployment policy from the
            drop-down list. A Deployment Policy governs how the deployment of
            Patches is carried out. Learn about :doc:`Deployment
            Policies <deployment-policy>`.

        iii. **Install After**: Provide a date and time after which the request
             tells the Computers to commence the installation process

        iv. **Expire After**: This is the date and time after which the
            request ceases to be a valid request.

        v.  You can select whether you want to create the deployment for installation or uninstallation.
            When you select uninstallation, only the installed Patches are shown.     

    b. **Select Patch**: Here you add the Patch/Patches that you want to deploy.

        .. _pf-64:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-64.png
            :align: center
            :alt: figure 64

        i. Section-A (:numref:`pf-64`) is the area where you view the selected Patches.

        ii.  Section-B has a search bar for searching all available Patches for
             the selected platform. The search bar supports the Advanced Search
             feature. Learn how to use :ref:`Advanced Search <search-bar-list-view>`.

        iii.  Section-C is where you view the available Patches in the tool.
              Clicking a checkbox selects a Patch and transfers it to section-A.

        Select the Patches that you want to deploy.

    c. **Select Target**:

        .. _pf-65:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-65.png
            :align: center
            :alt: figure 65


       Here you set your target computers. Patch will be deployed in the target computers. Here you can set the
       following things:

       i. Set a :ref:`Remote Office <add-remote-office>`. This will allow auto selection of multiple computers from a Remote Office's 
          network may or may not be based on include and exclude conditions.

          You can use a :doc:`manage-computer-group` to filter a Remote office. Computers (of the Remote Office) in the Group will be
          either included or excluded.

          .. _pf-65.1:
          .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-65.1.png
            :align: center
            :alt: figure 65.1

       ii. Set :ref:`individual <Adding of Computers from List>` computers.

       iii. Set a different :ref:`Scope<Adding Multiple Scopes>` (Target) if there are multiple Remote Offices. 
      
    d. **Retry Configuration**

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
        In-Progress to Failed and vice-versa for a single patch till success is reached in deployment.     

Fill in all the necessary details. Now you have two options; you can
publish the request or save it as a draft.

If you save the request as a draft, then the request appears as drafted
in the Deployment Requests page. You can view all drafted requests using
the Quick Filter **Drafted**.

.. _pf-66:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-66.png
   :align: center
   :alt: figure 66

If you want to publish the request, then click on **Publish**. This
might or might not activate the request immediately, depending on Custom
Rules. If Patch :ref:`Custom Rules<Patch Custom Rules>` demand Approval, then you
have to seek Approval before you can publish the Request.

You can publish a drafted request from its Update page (clicking on a
request opens its Update page).

.. _other-ways-add-request:

Other Ways to Add a Manual Request
==================================

Deployment Request from the Patch List View:
--------------------------------------------

Flotomate allows you to select the Patches from the List View directly
and deploy them.

-  Go to the :ref:`Patch List View <patch-list-view>`.

-  Select a Patch or Patches from the list area. A Deploy button appears
   above the list area.

.. _pf-67:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-67.png
   :align: center
   :alt: figure 67

-  Click on **Deploy,** and the Create page opens. The selected
   Patch/Patches are preselected. Complete the request and deploy. Learn
   more about creating a :ref:`Deployment
   Request <manually-create-request>`.

Deployment Request from Patch Details View:
-------------------------------------------

-  Go to the :ref:`Details View <patch-details-view>` of the Patch that
   you want to deploy.

-  Click on the **Deploy** button situated in the top right corner of
   the page.

.. _pf-68:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-68.png
   :align: center
   :alt: figure 68

-  The Create page opens with the Patch preselected. Complete the
   Deployment Request. Learn more about :ref:`Deployment
   Request <manually-create-request>`.

Adding a Deployment Request from a Computer’s Details View:
-----------------------------------------------------------

-  Go to the :ref:`Computer List View <computer-list-view>`.

-  Click on a Computer. This takes you to the Details View of the
   Computer.

-  Click on **Deploy Patches** from the **Action Menu**.

.. _pf-69:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-69.png
   :align: center
   :alt: figure 69

-  The Create page of Deployment Request opens. Create your request and
   publish it, or you can save it as a draft. Learn more about :ref:`creating
   Deployment Requests <manually-create-request>`.

.. _deployment-request-approval:

Approval
========

In case there is a custom rule defined (Refer admin manual for Patch :ref:`Custom Rules<ad-custom-rule>`), 
then you have to make every drafted request go through an Approval process before publishing it. In
an Approval process, you seek approval from a set of approver/approvers.

Asking for an Approval:
-----------------------

-  Go to the :ref:`Deployment Request<manually-create-request>` page.

-  Click on the Quick Filter **Drafted** to sort all drafted requests.

.. _pf-70:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-70.png
   :align: center
   :alt: figure 70

-  Requests that haven't gone through the Approval process have the **Ask for Approval** button adjacent to them.

.. _pf-71:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-71.png
   :align: center
   :alt: figure 71

-  When :ref:`Allow Manual Approval` feature is turned on, you will be shown a dialog box that you can use to create a manual
  Approval. If you **skip** this dialog box, then the Approval goes to the Workflow.

Different States in an Approval
-------------------------------

-  Pending:

-  Rejected:

-  Pre-Approved:

-  Approved:

Approval Process:
-----------------

In case of automatic approval, first, the system checks all available Approval Workflows when an
Approval is asked. If there are no workflows or the workflow
conditions are not meet, then the drafted request/requests are
Pre-Approved, and you can proceed with publishing. If there is a
workflow/are workflows, and their conditions are met, then
approver/approvers are auto-assigned for each request.

When there are multiple requests, it may happen that some may trigger
the Approval conditions and are put in Approval, and some may not
trigger the conditions and are Pre-Approved.

.. _pf-72:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-72.png
   :align: center
   :alt: figure 72

When you **Ask for an Approval** for a request, an **Approval**
button appears adjacent to the request. The button gives you access
to the Approval details dialog box where you can view all the
approvers and their comments and even re-ask for an Approval (this
again checks for all available workflows).

.. _pf-73:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-73.png
   :align: center
   :alt: figure 73

For requests that have Approvers, the Approval Status changes to
Pending, and it stays there as long as the approver/approvers don’t
express a decision.

An approver can see his Approvals in the **My Approvals** section of
his account.

.. _pf-74:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-74.png
   :align: center
   :alt: figure 74

Clicking on **My Approvals** (:numref:`pf-74`) opens the My Approval page
where he can view his Approvals.

.. _pf-75:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-75.png
   :align: center
   :alt: figure 75

Clicking on an Approval in **My Approval** opens a new page. There he
can perform the following actions:

.. _pf-76:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-76.png
   :align: center
   :alt: figure 76


- View request details, target Patches, and Computers.

- Start a comment thread.

- Approve or Reject the Approval.

The outcome of an Approval process is decided in two ways:

- **Unanimous**: All of the Approvers have to approve else the
  Approval is rejected.

- **Majority**: If the majority of Approvers agree then Approval is
  successful.

  In case there are multiple Approvals, the decision to go with
  unanimous or majority can be set from **Admin** (A Navigation Tab)
  >> **Approval Workflow** (Automation) >> **Approval Settings**,
  but the rights to do it lies with the Super Admin.

On success, the Approval moves to the Approved stage where the author
can publish the draft. On failure, the Approval moves to the Reject
stage where the author has to reinitiate the Approval process. The
author reinitiates an Approval process using the **Re-Approve**
option. A **Re-Approve** puts a request back to the pending stage.

.. _pf-77:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-77.png
   :align: center
   :alt: figure 77

Any Technician with the **Can Ignore Approval** right can ignore
approvers and push the Approval towards the Approved stage; where he
can publish the draft. The ignored approvers can see their Approval
status as Ignored in Approval details dialog box of the Article.

.. _pf-78:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-78.png
   :align: center
   :alt: figure 78

.. _searching-deployment-request:

Searching Deployment Requests
=============================

There are two broad ways to search Deployment Requests in the tool:

-  Using Search Bar

-  Using Filters

.. _pf-79:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-79.png
   :align: center
   :alt: figure 79

.. _search-bar-1:

Search Bar
----------

In the :ref:`Deployment Request <manually-create-request>` page you
get a search bar to search through requests. The search bar supports the
Advanced Search feature where you get a set of search options. Click on
the search bar to access all search options.

.. _pf-80:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-80.png
   :align: center
   :alt: figure 80

In some options you have to enter a value and in others there are
predefined values. You can create conditions using multiple options.
Between two different conditions of the same option type OR logic is
followed. Between different types AND logic is observed. An example of
same option type contradiction is Name contains Patch vs. Name contains deploy.

.. _pf-81:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-81.png
   :align: center
   :alt: figure 81

.. _filters-1:

Filters
-------

You can search for requests in the Deployment Request page using Quick
Filters. There three types of filters available:

-  Filters based on time of deployment.

-  Filters based on publishing status.

-  Filters based on origin.

.. _pf-82:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-82.png
   :align: center
   :alt: figure 82

Section-A (:numref:`pf-82`) is a quick filter to toggle across the following
views:

-  **Current**: Shows all the published and drafted requests that can
   start the deployment process immediately.

-  **Future**: Shows all the published requests that can start the
   deployment after a future date and time.

-  **Past**: Shows all the requests that have expired.

-  **Drafted**: Shows all drafted requests that are yet to be published.

-  **Archived**: Shows requests that have been deleted, includes drafted
   requests.

Section-B (:numref:`pf-82`) allows you to filter request based on origin and
Approval status. There are three possible origins to a Deployment Request, 
and the Approval status shows both Approved and Pre-Approved requests.

-  :ref:`Approval (status) <deployment-request-approval>`

-  :ref:`Manually <manually-create-request>`

-  :ref:`Automatic Patch Deployment <Automatic Patch Deployment>`

-  :ref:`Automatic Patch Test <automatic-patch-test>`

.. _managing-deployment-requests-1:

Managing Deployment Requests
============================

.. _deployment-status:

Deployment Status
-----------------

In the Deployment Request page, every published request has a Status
button.

.. _pf-83:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-83.png
   :align: center
   :alt: figure 83

Using the Status button, you can check the download status of all
associated Patches of a request, and associated Computers and their
Deployment Status.

Clicking on a **Status** button opens a new page with the following
tabs:

      -  **Patch Download Status**: Here you can view all involved Patches and
         their download statuses. A Patch transitions through various statuses
         during a download cycle. Some of the statuses reflect a stage, and
         some are conclusions. Altogether there are six statuses:

            .. _pf-84:
            .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-84.png
                :align: center
                :alt: figure 84

            a. **Pending**: The Patch has been put in a queue by the Main Server
               for download. At this stage, you can cancel the process.

            .. _pf-85:
            .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-85.png
                :align: center
                :alt: figure 85

            b. **Downloading**: The Main Server is downloading the Patch. At this
               stage, you can cancel the process.

            c. **Downloaded**: The Main Server has finished downloading the
               Patch.

            d. **Transferring**: The Main Server is transferring the Patch to the
               File Server.

            e. **Available**: The Patch is available on the File Server for
               deployment.

            f. **Cancelled**: A user cancelled the downloading process, or there was
               an error in downloading the Patch. This error also comes when the File Server is not setup.
               You can restart the download process using the **Retry** button.

      -  **Computers**: Here you can view all the associated Computers. Each
         computer has a **Deploy Status** button which opens a dialog box
         where you can view the installation statuses of each Patch. Computer
         transitions through various statuses when installing a Patch. Some of
         the statuses reflect a stage, and some are conclusions. Altogether
         there are six statuses:

            .. _pf-86:
            .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-86.png
               :align: center
               :alt: figure 86

            .. _pf-87:
            .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-87.png
                :align: center
                :alt: figure 87

            a. **Yet to Receive**: The Computer is yet to receive instructions from
               the request to install the Patch.

            b. **In Progress**: The Computer is in the process of installing the
               Patch after receiving the instructions.

            c. **Success**: The Computer has successfully installed the Patch.

            d. **Failed**: The Computer has failed to install the Patch.

            e. **Cancelled**: The request was deleted before the Computer could
               receive the instructions for installation.

            f. **Not Applicable**: The Patch is not meant for the Computer.

            g. **FS Not Prepared**: The main server has lost connection with the file server.

            h. **DS Not Prepared**: If there are Computers in a Remote Office, Patches are locally stored in Distribution Servers.
               This status shows that the concerned Patch is not available in the distribution server.

.. _not-applicable:

Unsupported Computers in a Deployment
-------------------------------------

During deployment it may happen that certain target Computers don’t
support all the Patches; in that case, the Not Applicable status is
helpful.

Go to the **Status** of a request. Click on the **Deployment status** of
a Computer; there the Patches that don’t support the Computer have the
**Not Applicable** status.

.. _pf-88:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-88.png
   :align: center
   :alt: figure 88

Edit/Archive a Deployment Request:
----------------------------------

You can update Deployment Requests that are in draft mode (both created
manually and by an automatic process). Once published, a request cannot
be edited.

-  Go to the :ref:`Deployment Request Page <manually-create-request>`.

-  The **Status** button adjacent to a request shows that the request is
   a published request.

-  You can open a request in edit mode by clicking on it or by clicking
   the Edit icon.

.. _pf-89:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-89.png
   :align: center
   :alt: figure 89

**Archiving**

The tool allows you to delete published and drafted Deployment
Requests. You can delete multiple requests at a time.

-  Go to the :ref:`Deployment Request <manually-create-request>` page
   from the Patch Menu.

-  Select one and more requests. The **Archive** button appears.

.. _pf-90:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-90.png
   :align: center
   :alt: figure 90

-  Click on the **Archive** button. On confirmation, the
   request/requests are deleted.

**Deleting an Active Deployment Request:**

Deleting a published request has the following effects:

-  Installation of Patches is cancelled in Computers that are yet to
   receive instructions.

-  Downloading and transfer of Patches to the File Server continues
   even when the request is archived.

View Archived Deployment Requests
---------------------------------

You can view an archived request along with its status. An archived
request may have partially finished operations that might need scrutiny.
To view an archived request:

-  Go to the :ref:`Deployment Request <manually-create-request>` page.

-  Select **Archived** from the Quick Filter section.

.. _pf-91:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-91.png
   :align: center
   :alt: figure 91

-  Now you can view all archived requests. Use the **Status** button to
   view :ref:`deployment status <deployment-status>`.

.. _pf-92:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-92.png
   :align: center
   :alt: figure 92
