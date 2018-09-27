*****************
More Demo Reports
*****************

Creating a Correlation Reports
==============================

**Scenario**: Acme Inc is conducting an Audit to know the number of Workstations with Licensed Software. The IT Admin of Acme Inc 
decides to create a Report that lists the Asset ID, Host-name and Used By user-name of Workstations with at least one Licensed
Software. 

In order to achieve this, the IT Admin has to create an Asset Report that has correlation with the Hardware Assets. To start with, 
Admin decides to create the Report for a single Product: Dell XPS 13 (Windows Laptop).

**Action**:

-  Admin opens the :ref:`Create a Custom Report <new-custom-report>` dialog box.

-  He/she creates a Tabular Report called Licensed Asset List that is going to list the Asset ID, Host-name and Used by user for
   all Windows Laptop of Product Dell XPS 13 with at least one Licensed Software.

-  Following is the selections/inputs for the sections/fields in **Create a Custom Report** dialog box and **New Custom Report** page:

+-----------------------------------+---------------------------------------------+
| Values                            | Section Name                                |
+===================================+=============================================+
| Licensed Asset List               | :ref:`Add a Name to the Report`             |
+-----------------------------------+---------------------------------------------+
| Asset and Software (Asset Type)   | :ref:`selecting a module`                   |      
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Tabular Report                    | :ref:`selecting report type`                |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Asset (Report folder)             | :ref:`Setting the Folder of a Report`       |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Description of the Report         | :ref:`Editing the Description of a Report`  |
| (See below image for actual       |                                             |
| description)                      |                                             |
+-----------------------------------+---------------------------------------------+
| Portrait                          | :ref:`report layout`                        |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Report shared with no one.        | :ref:`report visibility`                    |
| Private report.                   |                                             |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Created Time                      | :ref:`filter data with time`                |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Primary Condition set for         | :ref:`Apply Filters with Single Module`     |
| Software Asset Type:              |                                             |
|                                   |                                             |
| *Software Type Equals to Managed* |                                             |
|                                   |                                             |
| Secondary Condition set for       | :ref:`Apply Filters with Correlated Modules`|                                                                       |
| Windows Laptop Asset type:        |                                             |
|                                   |                                             |
| *Product Equals to Dell XPS 13*   |                                             |
+-----------------------------------+---------------------------------------------+
| **Grouping**: None                | :ref:`grouping of data`                     |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+


- The Admin sets two filters which will have the following outcomes.

  a. First filter will create a subset of Assets with at least one Managed Software.

  b. The second filter will create a subset of the above subset with Product equals Dell XPS 13.

.. _rfd1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-D-1.png
      :align: center
      :alt: figure 1

- The Admin selects the following columns and creates the report.

.. _rfd2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-D-2.png
      :align: center
      :alt: figure 2

In order to generate the Report, the Admin can :ref:`download <Preview and Download>` the Report and create a :ref:`Schedule <Schedule a Report>`.  