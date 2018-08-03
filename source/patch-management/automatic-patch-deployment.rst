**************************
Automatic Patch Deployment
**************************

Deploying Patches is a recurring task that requires time and effort, and
the effort to download and deploy new Patches increases with the
increase in the number of managed IT Assets.

An Automatic Patch Deployment task helps you to download and deploy
Patches, based on a set criterion, periodically. Setting up an
auto-deployment task is a one-time activity, and you can turn it off
anytime later. You can create multiple auto-deployment tasks.

Few of the benefits of using Automatic Patch Deployment:

-  Periodic download and deployment of newly found Patches without any
   misses.

-  Schedule download of Patches at a time when the network is least
   likely to have heavy traffic.

.. _create-auto-deployment:

Creating an Automatic Patch Deployment
======================================

-  Go to the Flotomate **Launcher** and select **Patch**.

-  Select **Automatic Patch Deployment** from the Patch menu.

-  The Automatic Patch Deployment page opens. Here you can view all your
   existing auto-deployments tasks if any. Click on **Create Auto Deploy
   Task** situated in the top right corner of the page.

-  A new page opens with the following fields and options:

    .. _pf-93.1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-93.1.png
        :align: center
        :alt: figure 93.1

    .. _pf-93.2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-93.2.png
        :align: center
        :alt: figure 93.2

    .. _pf-93.3:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-93.3.png
        :align: center
        :alt: figure 93.3

    .. _pf-93.4:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-93.4.png
        :align: center
        :alt: figure 93.4            

    a. Section A (:numref:`pf-93.1`) is where you provide a name to the task and select
       a :doc:`Deployment Policy <deployment-policy>`. You also get a toggle to turn the deployment task off later.

    b. Section B is where you decide from which applications to select the Patches. You get three options:

       i.  **All Application**: As the name suggests, this includes all available applications for searching Patches.   
       ii. **Include Application**: You include applications from which Patches are selected.

            .. _pf-47:
            .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-47.png
               :align: center
               :alt: figure 47
    
       iii. **Exclude Application**: You exclude applications that are ignored when searching for Patches.

       There is a search bar for Application that supports filtering using Package Type.

       You can filter application Patches using criteria Categories and Severities; 
       for example, you can make the Test Task select Patches with the Category Service Packs and Severity, Critical and Important.

       .. _pf-48:
       .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-48.png
           :align: center
           :alt: figure 48  
   
    c. Section C is where you select task and Patch type:

        **Task Type:**

            i.  Download only Approved Patch types in the :ref:`Shared Drive <share-drive>`.

            ii. Download only Approved Patch types in the :ref:`Shared Drive <share-drive>`, and create a drafted Deployment Request.

            iii.  Download only Approved Patch types in the :ref:`Shared Drive <share-drive>`, and create and publish a Deployment Request.

        **Patch Type:**

            i.  Only consider Approved Patches that are newly added to the tool.

            ii.  Only consider Approved Patches that are :doc:`missing <missing-patch>`.

            iii.  Only consider Approved Patches that are newly added missing.

    d. Section D is where you set your target computers. Patch will be deployed in the target computers. Here you can set the
       following things:

       i. Set a :ref:`Remote Office <add-remote-office>`. This will allow auto selection of multiple computers from a Remote Office's 
          network may or may not be based on include and exclude conditions. 

       ii. Set :ref:`individual <Adding of Computers from List>` computers.

       iii. Set a different :ref:`Scope<Adding Multiple Scopes>` (Target) if there are multiple Remote Offices.

-  Complete filling the fields and selecting the options. Click on
   **Create** to create your auto-deployment task.

In order to run the auto-deployment task, you have to create a schedule.

**Edit/Delete a Deployment Task**

You can open a task in edit mode by clicking on the Edit Icon adjacent
to a task. Similarly, you can delete a task using the Delete Icon.

.. _auto-deployment-schedule:

Create an Auto-Deployment Schedule
==================================

Scheduling tells the tool when to start an :doc:`auto-deployment
task <automatic-patch-deployment>`. The outcome of an
auto-deployment task is a Pre-Approved Deployment Request for Patches
satisfying the Patch type of the task.

-  Go to the Automatic Patch Deployment Page.

-  Click on the **Schedule** button adjacent to the task for which you
   want to set a schedule.

.. _pf-94:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-94.png
   :align: center
   :alt: figure 94

-  A dialog box opens. Click on the **Schedule** button.

.. _pf-95:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-95.png
   :align: center
   :alt: figure 95

-  Set a Schedule frequency:

   .. note:: Except Interval, every other option requires you to set a Time Zone.

   a. **Once**: Deployment happens only once at a specific date and
      time.

   b. **Daily**: The deployment task activates on a start date & time.
      After that, the deployment happens every day at a specified time
      mentioned in the Hour and Minute field.

   c. **Weekly**: Deployment happens on a specific day/days of a week at
      a specified time.

   d. **Monthly**: Discovery happens in selected month/months of a year
      on a particular day at a specified time.

   e. **Interval**: Discovery happens after every specified minutes,
      hours, days or month.

-  An auto-deployment task generates a :doc:`notification <patch-notification>` whenever it creates a
   Deployment Request. Set the recipients; it can either be a Technician
   Group/Groups or an individual (email)/individuals.

-  Click on **Save Schedules** to save your settings.

You can edit the schedule settings of any task.

.. _auto-deployment-status:
View Status of an Auto Patch Deployment Task
============================================

.. _pf-96:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-96.png
   :align: center
   :alt: figure 96

Using the **Status** button, you can check the download status of all
associated Patches of a request, and associated Deployment Requests.

Clicking on a **Status** button opens a new page with the following
tabs:

.. _pf-97:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-97.png
   :align: center
   :alt: figure 97

-  **Download Status**: Here you can view all involved Patches and their
   download statuses. A Patch transitions through various statuses
   during a download cycle. Some of the statuses reflect a stage, and
   some are conclusions. Altogether there are six statuses:

   a. **Pending**: The Patch has been put in a queue by the Product
      Server for download.

   b. **Downloading**: The Product Server is downloading the Patch.

   c. **Downloaded**: The Product Server has finished downloading the
      Patch.

   d. **Transferring**: The Product Server is transferring the Patch to
      the Shared Drive.

   e. **Available**: The Patch is available on the Shared Drive for
      deployment.

   f. **Cancelled**: There was an error in downloading the Patch.

-  **Deployment Requests**: Here you can view all Deployment Requests
   created by the Auto Patch Deployment Task. Each request has a
   **Status** button to view its :ref:`Deployment
   Status <deployment-status>`.