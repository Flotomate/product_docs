*****************************
Release Notes - Dolphin 2.7.0
*****************************

**Introduction of New Components**
==================================

1. Dashboard
------------

.. _re-2.7-0:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-2.7-0.png
    :align: center
    :alt: figure 0

Flotomate now has a customizable Dashboard that can provide a glance
view of key KPIs and relevant data. We have predefined Dashboards out of
the box; apart from that, users can create new Dashboards to reflect a
particular business process.

In a Dashboard, the user can add data blocks called Dashlets. Each
Dashlet can have its own set of conditions, based on which it will show
the information. Currently, we are providing three kinds of Dashlets:

-  **Widget**: A Widget is a graphical representation of data filtered
   by time and other parameters.

-  **KPI**: A KPI (Key Performance Indicator) is a measurable value
   which helps in determining the efficiency of a system. For example; a
   number of resolved Request tickets over the last 30 days is one of
   many indicators of efficiency of the Helpdesk.

-  **Shortcuts**: It is a list of Frequent Access Items (i.e. My Open
   Incidents, My Approval, My Tasks etc.).

A Dashboard can fetch data from the following modules:

-  Service Desk (Request, Problem, and Change)

-  Asset Management

**Benefits**:

-  A Dashboard allows a user to see, at a glance, an overall situation
   report of the desired information.

-  A Dashboard enables a user to drill down into the details by simply
   selecting the desired variable and object.

-  An easy graphical interface allows a user to play with data and do
   the easy cross-sectional analysis.

-  A Dashboard can be a one-page snapshot of key metrics of a business.
   A user of the Flotomate Dashboard can quickly judge how well the
   Helpdesk is functioning.

**Key Highlights of Flotomate Dashboard:**

-  A Dashboard is customizable; a user can add and modify Dashlets.

-  A user can create new Dashlets.

-  A user can control who can view a Dashboard and Dashlet separately.

-  Widgets support multiple chart types for data visualization.

-  Data fetched by a Dashboard is real time

-  A user can filter Dashboard data based on time and location.

-  Two out of box Dashboards.

**Documentation Link**: :ref:`Flotomate Dashboard Introduction` 

2. High Availability
--------------------

The concept of High Availability focuses on the maximum uptime of the
service by ensuring service and data recovery during an unplanned
disruption.

In an HA setup, there are three servers, the main server is called the
Master, the secondary server is called the Slave and there’s a proxy
server.

.. _re-2.7-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-2.7-1.png
    :align: center
    :alt: figure 1

The Master is the main server which is accessed by the users; the Slave
stays idle. The database between Master and Slave is synchronized on a
real-time basis. When the Master does down, the slave becomes the new
Master with the backed up database. An HA proxy acts as a load balancer
between Master and Slave.

**Use Cases of an HA**:

-  Maintaining availability of service during an unplanned shutdown of
   the Master (Main Server).
   For example, An organization maintaining an HA has to have two
   separate Servers, one for Master and other for Slave, this is to
   ensure that in an unforeseen event like a fire, natural calamity,
   etc. when the Master is down, the Slave can be kept alive from the
   last point of recovery.

-  High availability setup can be used for a planned outage of the
   Service Desk for the purpose of maintenance.

-  High Availability can be used in the event of a disaster recovery of
   data.

**Key Highlights**:

-  Easy setup in minutes

-  Automatic Slave to Master

-  Minimal efforts to restore HA again post failure.

**Documentation Link**: :ref:`Flotomate High Availability Server Setup` 

3. Desktop Automation Product (New Architecture and New Features)
-----------------------------------------------------------------

In our new architecture, we have deprecated the use of Shared Drive
instead we are using a File Server. A File Server centralizes the
storage of Patch, Packages and Agent file; this makes our tool scalable
and flexible, and increases the overall performance. In conjunction with
the File Server, we now support Relay Servers to distribute File storage
across multiple Remote Offices.

.. _re-2.7-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/release-note/RE-2.7-2.png
    :align: center
    :alt: figure 2

Our revamped Remote Desktop Automation now supports the following:

-  Package Deployment Support (MSI, MSP, MSI-MST, EXE etc.).

-  A Package can be deployed and Install as "Run As System User" or "Run
   as Current User".

-  Ubuntu Linux patches are supported via manual upload.

-  Both Patch & Package Support Installation & Uninstallation.

-  Agent Self Upgrade has been simplified.

3. Report -Revamped
-------------------

The Report module has been revamped with new UI elements and features.

The UI elements make creating and searching Reports faster and easy:

-  **New Report Create Flow**: Creating a report has been divided into
   two stages. The first stage explicitly shows the Report types and
   modules, and the second stage is where one selects the filters and
   columns.

-  **Folder:** All Reports are now categorized into folders.

-  **My Favourite:** A user can mark a Report as a favorite. Favorite
   Reports have a separate folder.

New Feature addition:

-  **Correlated Reports**: With correlation, one can generate a report
   using the data at the intersection/subset of two modules/feature.

-  **Column Sorting**: User can now sort columns of a report either in
   ascending or descending order.

-  **Subtotal per Group**: Now users can generate matrix reports with
   columns showing total count.

-  **Out of Box Report**: Module wise, we have added out of box reports.

4. Apple Mac Device Discovery
-----------------------------

-  We have released a new version of Mac Agent (A.2.7.0).

-  Now we support Agentless Discovery of Mac OS

-  User can generate Reports with data from Mac workstations.

5. Software Asset Automation
----------------------------

We have been able to identify three problems related to Software Asset
management:

-  Most users want to manage a small number of Software Assets.

-  Most users want to set structure data fields (i.e. Product etc.) upon
   discovery so, they can better report and compliance management.

-  Most users want to control what kind of software should be installed
   on their computers.

We have introduced the following features to address the above problems:

-  **Normalization Rules**: Automatic rule-based classification of
   Software.

-  **Consolidation Rules for Software Suite**: Automatic rule-based
   consolidation of Software.

-  **Blacklist and Whitelist for Software**: Rules-based prohibition of
   Software.

6. Asset Finance
----------------

Hardware and Non-IT Assets have a Financial tab with the following
features:

-  One can define a depreciation method or import through Product
   association. Products now support depreciation configuration.

-  Book Value is shown after adjustment of depreciation.

-  Total Cost of the asset is shown along with cost bifurcation.

**Features Improvement**
========================

1. **Software Meter - Revamped**

   -  Meter Architectural and new design and reliability

   -  Ability to analyze usage between timelapse

2. **SLA for Problem and Change.**

   -  Users can set Response and Resolution time with multiple escalations
      for Problems and Changes.

3. **Windows OS License Activation Status**

   -  Workstation (Hardware Asset) properties now show whether the OS is
      genuine or not.

4. **Enhanced Design of Customer Portal**

   -  Customer Portal has been revamped which now shows Service Catalog
      explicitly on the homepage.

5. **Requester Profile at fingertips**

   Technicians can search users using the keyboard shortcut and from
   Technician Portal, and view:

    -  Recent Requests.

    -  Profile.

    -  Used by Assets.

6. **Custom Field Support in Keywords/Placeholders**

   -  Users can now use custom field values (excluding Requestor field) in placeholders for creating
      custom emails.

.. important:: :ref:`Learn how to Upgrade Product License. <How to Update Product License>` 