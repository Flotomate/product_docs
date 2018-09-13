*****************************
Getting to Know About Reports
*****************************

Reports in Flotomate are multi-dimensional, which means data can be shown in different ways. In Flotomate, reports are of two types:

- Pre-defined Reports
- Custom Reports

We give thirty nine Reports out of the box, referred as Pre-defined
Reports. These Reports are standard Reports commonly used by most of our
users.

Custom Reports are user generated reports, and there's no limit to the number of Reports a user can generate. 

Folders for Managing Reports
============================

All reports (both Pre-defined and Custom Reports) in the system are grouped into folders. 
There are 11 folders (based on the number of modules) of out of the box, but a user can create more folders. 

To view all the folders, a user has to go to **Launcher** >> **Report** (:ref:`Report List View`).

.. _rf0:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-0.png
      :align: center     
      :alt: Figure 0


Rearranging Folders
-------------------

A user can change the order of the Folders from the :ref:`Report List View`.

.. _rf0.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-0.1.png
      :align: center     
      :alt: Figure 0.1

.. _Create a Report:

Stages to Create a Custom Report
================================

We have a standard interface to create reports across different modules.

All Custom Reports are created using the New Custom Reports page. Creating a Custom Report is a multi-stage process, which
involves the following stages:

.. _new-custom-report:

Create a Custom Report
----------------------

Log in to the Dashboard using the Technician Portal.

Go to **Launcher** >> **Report** (:ref:`Reports List View`).

The Report List View opens. Click on **Create a Custom Report** button
situated in the top right corner of the page. Create a Custom Report dialog box opens where you have to 
perform the following actions:

.. _rf1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-1.png
      :align: center     
      :alt: Figure 1

.. _rf1.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-1.1.png
      :align: center     
      :alt: Figure 1.1

.. _add name and description:

Add a Name to the Report
^^^^^^^^^^^^^^^^^^^^^^^^

Section-A (:numref:`rf1.1`) is where you enter the name of the Report. The best
practice is having a name which is descriptive and concise.

Selecting Report Type
^^^^^^^^^^^^^^^^^^^^^

Section-B (:numref:`rf1.1`) lets you select the Report type. There are three
types shown which are as follows:

-  **Tabular Report**: These are simple reports that allow you list
   items in columns grouped by criteria in section-J.

-  **Matrix Report**: This type of Reports show cumulative item counts
   in a grid format (C X R). The counts are group based on criteria in
   section-J.

-  **Summary Report**: This type of Reports can summarize properties,
   details, milestones, and components of items in Asset, Projects,
   Patches, and Software License.

*Note: This is a onetime selection meaning that you cannot change it
later.*

Selecting a Module
^^^^^^^^^^^^^^^^^^

Section-C (:numref:`rf1.1`) is where you search and select the module for which you are
making the Report. You are allowed to select one module from the
following modules:

-  **Request**: Refers to the Request Management module.

-  **Problem**: Refers to the Problem Management module.

-  **Change**: Refers to the Change Management module.

-  **Asset**: Refers to the Asset Management module. You can drill down
   to an Asset Report Type (you can further drill down to an Asset Type in the next stage) 
   with the selection in :numref:`rf2`. The Report will be generated based on the Asset and type you select.

    .. _rf2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-2.png
        :align: center
        :alt: figure 2


-  **Project**: Refers to the Project Management module.

-  **Remote Deployment**-**Patch**: Refers to the Patch Management
   module.

   When selecting this module you also have to select a platform. 

-  **Remoter Deployment**-**Agent**: Refers to the Flotomate Agent used
   for Asset discovery and remote deployment of patches and packages.

-  **Software License**: This allows you to create exclusive reports on Software License usage.   

-  **Multi-Module**: This module helps you to combine two or more
   existing Reports into one Report. This module is visible when the
   Report Type is set to Summary Report.

-  **Contract**: Refers to the Contract Management module.

-  **Purchase**: Refers to the Purchase Management module.

Depending on the module selected, the Criteria parameters, data columns
and group by properties are updated.

*Note: This is a onetime selection meaning that you cannot change it
later.*

After completing the dialog box, click on **Proceed to Report Wizard** to move to the New Custom Report page. 

Completing the New Custom Report Page 
-------------------------------------

The next stage in creating the Report is to complete the New Custom Report page. Here you construct the report by:

- Deciding the layout of the Report.
- Adding data filters based on time and other criteria.
- Setting visibility (public or private).
- Adding of Group By criterion.
- Selecting of columns.

There are slight differences in the way columns are selected for different report types; and the available columns also differ with
different modules. To further elaborate the steps follow the below explanation:

.. _rf2.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-2.1.png
      :align: center
      :alt: figure 2.1

.. _rf2.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-2.2.png
      :align: center
      :alt: figure 2.2

.. note:: Please refer :numref:`rf2.1` & :numref:`rf2.2` for below descriptions.

Editing the Description of a Report
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In section-A (:numref:`rf2.1`),  you can enter the description of the Report. Write a
suitable description because it is used as a body when the Report is
sent via email.

Setting the Folder of a Report
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

It is compulsory to set a folder for a report. In section A (:numref:`rf2.1`), you can set a folder by clicking on **Select Folder**.
A dialog box opens, where you can select an existing folder or create a new one and then select.

.. _rf2.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-2.3.png
      :align: center
      :alt: figure 2.3

Learn more about :ref:`Folders for Managing Reports`. 

.. _report layout:

Setting Layout of a Report
^^^^^^^^^^^^^^^^^^^^^^^^^^

Section-B (:numref:`rf2.1`) houses the layout options that decide the
orientation of the final Report. You can see the orientation when the
Report is opened either in PDF or Excel format. There are two
orientations to choose from:

-  Portrait

-  Landscape

Report Visibility
^^^^^^^^^^^^^^^^^

Section-B (:numref:`rf2.1`) houses the visibility options. There are two
options to choose from:

-  **Public**: The Report is visible to anyone having access to the
   Technician Portal. But the right to edit and delete still lies with
   the creator of the Report.

-  **Private**: The Report is visible only to the creator.

*Note: This option is non-changeable if the visibility is set to Public;
changeable, if set to Private.*

Filter Data with Time
^^^^^^^^^^^^^^^^^^^^^

Section-B (:numref:`rf2.1`) allows you to filter data using time. When
filtering tickets and CIs, one of the below mentioned type of time data is considered, depending on your selection.

-  **Created Time**: Whenever data is fetched, by Flotomate, from a
   module, the Create Time is considered in checking conditions, if any.
   For example, in a Report that shows total Requests with the Urgency
   set to High and group by Technicians for last 60 days, the Flotomate
   checks the Create Time of all the Requests to see eligibility for the
   period.

-  **Updated Time**: Instead of Create Time, the system uses the Update
   Time in checking data.

-  **Closed Time**: The closed time of a ticket/item is considered to check whether it falls within a specified period.

-  **Warranty Expiration Date**: Warranty Expiration Date of an Hardware Asset (including all its children) 
   is considered to check whether it falls within a specified period.

-  **Acquisition Date**: Acquisition Date of an Hardware Asset (including all its children) 
   is considered to check whether it falls within a specified period.

-  **Audit Date**: Audit Date of an Hardware Asset (including all its children) 
   is considered to check whether it falls within a specified period.

You can altogether ignore this filter by selecting **None**.

Set Asset Type
^^^^^^^^^^^^^^

When creating an Asset Report, you can specify a particular Asset Type (even a sub-type) in Section-B (:numref:`rf2.1`). 
This option allows you to generate reports, for example, of only Hardware Assets. 

.. _rf2.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-2.4.png
      :align: center
      :alt: figure 2.4

Setting Conditions to Filter Data
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Section-C (:numref:`rf2.2`) is where you set conditions to filter data before
it is used for generating Reports

The condition parameters are different for each module, but the way they
work is same for all.

You can add multiple condition groups with the **Add Condition Group**
option. Within each group, you can add multiple condition statements.

.. _rf3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-3.png
      :align: center
      :alt: figure 3


Each condition statement talks about a parameter being equal/not equal
to something. You can form a condition statement by clicking on the
three components marked by red boxes in Figure 3. Condition statements
exist within a group, and you can add multiple conditions by clicking on
the plus sign.

The conditions are checked following a hierarchy: first conditions are
checked within a group, and then within groups. The outcome of a
condition statement or a group of statements, or groups of statements is
either true or false. The word AND & OR helps in deriving an outcome
when there are multiple statements or groups, or both.

Multiple condition statements can be evaluated using two basic
operators: AND & OR. These two operators describe the relationship
between two statements, and the outcome is always either true or false.

Grouping of data
^^^^^^^^^^^^^^^^

Section-D (:numref:`rf2.2`) houses the Group By feature that groups the data
rows in a Report by:

.. note:: This field always has a value when the Report type is Matrix.

-  **Time Unit**: You can group the data row either Daily, Weekly or
   Monthly. This option is available when a :ref:`data filter <Filter Data with Time>` is selected. 

-  **Property**: Each module has a list of properties that you can use
   to group the data rows in the Report.
.. _rf4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-4.png
      :align: center
      :alt: figure 4

.. note:: The above figure shows the properties of the module Request Management.

You can ignore the group by feature in tabular reports by selecting the **None** option.

Selecting Columns
^^^^^^^^^^^^^^^^^

The last step in creating a Report is selecting the columns of the report. What
columns are available depends on the Report type and module selected.

.. _rf5.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-5.1.png
      :align: center
      :alt: figure 5.1
.. _rf5.2:      
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-5.2.png
      :align: center
      :alt: figure 5.2

-  **Tabular Report**:

   a. You add columns by selecting (Learn what is a :ref:`Tabular Report <Types of Reports>`) them and clicking on **Done**.

   b. You can search a column by its name.

-  **Matrix Report**:

   a. You select a column from a drop-down list (:numref:`rf5.2`). You can add multiple columns. Each column
      is accompanied by a function. You can filter the column list by Count or Average function.
      
      Columns with the Count function shows a cumulative count of items grouped by either time or a product property. 
      Columns with the Average function shows the average of items grouped by either time or a product property.

   b. Some columns have sub-columns which you can access by clicking the
      down icon next to a column name.

      .. _rf6:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-6.png
            :align: center
            :alt: figure 6

      You can choose what sub-columns to include in report from the dialog box. Learn more about :ref:`Matrix Reports <Types of Reports>`. 

   c. You add more columns using the plus icon (:numref:`rf5.1`).

-  **Summary Report**:

   a. You add properties/details by selecting them (multiple selections are allowed) and clicking on
      **Done**.

   b. Some properties/details have sub-items which you can access by
      clicking the arrow icon next to a name.

      .. _rf7:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-7.png
            :align: center
            :alt: figure 7

      You can choose what sun-columns to include in the dialog box. Learn more about :ref:`Summary Reports <Types of Reports>`. 

-  **Multi-Module Report**:

   You search and select Reports that you want to merge into one Report. Learn what is a :ref:`Multi-Module Report <Types of Reports>`. 

      .. _rf8:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-8.png
            :align: center
            :alt: figure 8

Sorting Columns
^^^^^^^^^^^^^^^

Once a Technician is done selecting columns, he/she can sort the rows by applying the sort function to a particular column.
The sort option is available in Tabular and Matrix Reports. 

There are two types of sorting Ascending and Descending. When doing sort, a Technician first selects a sort type, and then selects a 
column; if the selected column has sub-columns, then the Technician has to select that also. 

.. _rf8.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-8.1.png
      :align: center
      :alt: figure 8.1

.. _rf8.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-8.2.png
      :align: center
      :alt: figure 8.2