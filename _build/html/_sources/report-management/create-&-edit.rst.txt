Create & Edit Reports
=====================

Create a Report
---------------

We have a standard interface to create reports across different modules.

We give twenty-three Reports out of the box, referred as Pre-defined
Reports. These Reports are standard Reports commonly used by most of our
users.

All Reports are created using the New Custom Reports page. To access the
page follow the below steps.

.. _new-custom-report:
New Custom Report
~~~~~~~~~~~~~~~~~

-  Log in to the Dashboard using the Technician Portal.

-  Click on **Report** from the Navigation Tabs.

-  The Report List View opens. Click on **Create a Report** button
   situated in the top right corner of the page. The New Custom Report
   page opens.

.. _rf1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-1.png
      :align: center     
      :alt: Figure 1
               

Creating a Report involves nine stages which have been described below:

Add Name and Description
^^^^^^^^^^^^^^^^^^^^^^^^

Section-A (:numref:`rf1`) is where you enter the name of the Report. The best
practice is having a name which is descriptive and concise.

Section-B is where you enter the description of the Report. Write a
suitable description because it is used as a body when the Report is
sent via email.

Selecting a Module
^^^^^^^^^^^^^^^^^^

Section-C (:numref:`rf1`) is where you select the module for which you are
making the Report. You are allowed to select one module from the
following modules:

-  **Request**: Refers to the Request Management module.

-  **Problem**: Refers to the Problem Management module.

-  **Change**: Refers to the Change Management module.

-  **Asset**: Refers to the Asset Management module. You can drill down
   to an Asset Type with this selection in section-E (:numref:`rf1`). Reports
   are generated based on Asset and the type you select.

.. _rf2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-2.png
      :align: center
      :alt: figure 2


-  **Project**: Refers to the Project Management module.

-  **Remote Deployment**-**Patch**: Refers to the Patch Management
   module.

-  **Remoter Deployment**-**Agent**: Refers to the Flotomate Agent used
   for Asset discovery and remote deployment of patches and packages.

-  **Multi-Module**: This module helps you to combine two or more
   existing Reports into one Report. This module is visible when the
   Report Type is set to Summary Report.

Depending on the module selected, the Criteria parameters, data columns
and group by properties are updated.

*Note: This is a onetime selection meaning that you cannot change it
later.*

Selecting Report Type
^^^^^^^^^^^^^^^^^^^^^

Section-D (:numref:`rf2`) lets you select the Report type. There are three
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

Report Layout
^^^^^^^^^^^^^

Section-F (:numref:`rf1`) houses the layout options that decide the
orientation of the final Report. You can see the orientation when the
Report is opened either in PDF or Excel format. There are two
orientations to choose from:

-  Portrait

-  Landscape

Report Visibility
^^^^^^^^^^^^^^^^^

Section-G (:numref:`rf1`) houses the visibility options. There are two
options to choose from:

-  **Public**: The Report is visible to anyone having access to the
   Technician Portal. But the right to edit and delete still lies with
   the creator of the Report.

-  **Private**: The Report is visible only to the creator.

*Note: This option is non-changeable if the visibility is set to Public;
changeable, if set to Private.*

Filter Data with Time
^^^^^^^^^^^^^^^^^^^^^

Section-H (:numref:`rf1`) allows you to filter data using time. When
filtering tickets and CIs three times are considered; which one to use
depends on your selection?

-  **Create Time**: Whenever data is fetched, by Flotomate, from a
   module, the Create Time is considered in checking conditions, if any.
   For example, in a Report that shows total Requests with the Urgency
   set to High and group by Technicians for last 60 days, the Flotomate
   checks the Create Time of all the Requests to see eligibility for the
   period.

-  **Update Time**: Instead of Create Time, the product uses the Update
   Time in checking data.

-  **Closed Time**: Here the product uses the Closed Time in checking
   data.

Closed Time is not applicable to the Asset module and its Types, and
Remote Deployment.

Setting Conditions to Filter Data
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Section-I (:numref:`rf1`) is where you set conditions to filter data before
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

Section-J (:numref:`rf1`) houses the Group By feature that groups the data
rows in a Report by:

*Note: This is a required field when the Report type is Matrix*

-  **Time Unit**: You can group the data row either Daily, Weekly or
   Monthly.

-  **Property**: Each module has a list of properties that you can use
   to group the data rows in the Report.
.. _rf4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-4.png
      :align: center
      :alt: figure 4

The above figure shows the properties of the module Request Management.

Selecting Columns
^^^^^^^^^^^^^^^^^

The last step in creating a Report is selecting the columns. What
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

   a. You add columns by selecting them and clicking on **Done**.

   b. You can search a column by its name.

-  **Matrix Report**:

   a. You select a column from a drop-down list (:numref:`rf5`). Each column
      is accompanied by the count function which tells of giving a
      cumulative count of items grouped by either time or a product
      property.

   b. Some columns have sub-columns which you can access by clicking the
      down icon next to a column name.

.. _rf6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-6.png
      :align: center
      :alt: figure 6
::
      You can choose what sun-columns to include in the dialog box.

   c. You add more columns using the plus icon (:numref:`rf5.1`).

-  **Summary Report**:

   a. You add properties/details by selecting them and clicking on
      **Done**.

   b. Some properties/details have sub-items which you can access by
      clicking the arrow icon next to a name.

.. _rf7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-7.png
      :align: center
      :alt: figure 7

::
      You can choose what sun-columns to include in the dialog box.

-  **Multi-Module Report**:

   You search and select Reports that you want to merge into one Report.

.. _rf8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-8.png
      :align: center
      :alt: figure 8

.. _create-tabular-report: 
Create a Tabular Report
~~~~~~~~~~~~~~~~~~~~~~~

-  Open the :ref:`New Custom Report <new-custom-report>` page.

-  We are going to create a Tabular Report called Computer Asset List
   that lists all computers managed by a particular Technician, group by
   Product.
-  Following is our selections for the sections in New Custom Reports:

+-----------------------------------+-----------------------------------+
| Values                            | Section Name                      |
+===================================+===================================+
| Asset and Computer (Sub-Asset     | `Selecting a                      |
| Type)                             | Module <#selecting-a-module>`__   |
+-----------------------------------+-----------------------------------+
| Tabular Report                    | `Selecting Report                 |
|                                   | Type <#selecting-report-type>`__  |
+-----------------------------------+-----------------------------------+
| Portrait                          | `Report                           |
|                                   | Layout <#report-layout>`__        |
+-----------------------------------+-----------------------------------+
| Public                            | `Report                           |
|                                   | Visibility <#report-visibility>`_ |
|                                   | _                                 |
+-----------------------------------+-----------------------------------+
| Created Time                      | `rfilter Data with                 |
|                                   | Time <#filter-data-with-time>`__  |
+-----------------------------------+-----------------------------------+
| Technician name                   | `Setting Conditions to Filter     |
|                                   | Data <#setting-conditions-to-filt |
|                                   | er-data>`__                       |
+-----------------------------------+-----------------------------------+
| Product                           | `Grouping of                      |
|                                   | Data <#grouping-of-data>`__       |
+-----------------------------------+-----------------------------------+

.. _rf9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-9.png
      :align: center
      :alt: figure 9

-  Scroll down to the Select Column section of the page.

.. _rf10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-10.png
      :align: center
      :alt: figure 10

-  Here you see all the data columns available in a module. Each module
   has different columns to select. In Asset, you get different columns
   for each Asset Type; there could be hidden columns that you have to
   unhide by checking a box highlighted in Figure 10.

   You can also search for a column using the search bar in that
   section.

-  We select three columns for this Report. We can rearrange them using
   drag & drop. We finalize our selections by clicking on **Done**.
.. _rf11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-11.png
      :align: center
      :alt: figure 11

-  We save the Report by clicking on **Create**.

The process to create a Report is same for all the modules in the
system. We get the following Report when we
:doc:`preview <preview-a-report>` for the past 3 months and group by
Product.

.. _rf12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-12.png
      :align: center
      :alt: figure 12

.. _create-matrix-report:
Create a Matrix Report
~~~~~~~~~~~~~~~~~~~~~~

-  Open the :ref:`New Custom Report <new-custom-report>` page.

-  We are going to create a Matrix Report called Average Resolution Time
   that shows the average resolution time of each Technicians along with
   the Request number bifurcated across support levels.

-  Following is our selections for the sections in New Custom Reports:

+-----------------------------------+-----------------------------------+
| Values                            | Section Name                      |
+===================================+===================================+
| Request                           | `Selecting a                      |
|                                   | Module <#selecting-a-module>`__   |
+-----------------------------------+-----------------------------------+
| Matrix Report                     | `Selecting Report                 |
|                                   | Type <#selecting-report-type>`__  |
+-----------------------------------+-----------------------------------+
| Portrait                          | `Report                           |
|                                   | Layout <#report-layout>`__        |
+-----------------------------------+-----------------------------------+
| Public                            | `Report                           |
|                                   | Visibility <#report-visibility>`_ |
|                                   | _                                 |
+-----------------------------------+-----------------------------------+
| Created Time                      | `rfilter Data with                 |
|                                   | Time <#filter-data-with-time>`__  |
+-----------------------------------+-----------------------------------+
| Status Equals to Closed           | `Setting Conditions to Filter     |
|                                   | Data <#setting-conditions-to-filt |
|                                   | er-data>`__                       |
+-----------------------------------+-----------------------------------+
| Technician                        | `Grouping of                      |
|                                   | Data <#grouping-of-data>`__       |
+-----------------------------------+-----------------------------------+

.. _rf13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-13.png
      :align: center
      :alt: figure 13

-  Scroll down to Select Column section of the page.

.. _rf14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-14.png
      :align: center
      :alt: figure 14

-  A Matric Report gives you a cumulative count of data; for example,
   the total number of Requests assigned to each Technician. In Figure
   14, Count is the function mentioned in the first box, and the second
   box shows you all the column names available in the module. Each
   module has different column names. You can add more columns using the
   Plus Icon.

   We select two columns and click on **Done** to finalize our decision.

   It may happen a column name may generate additional columns. You can
   control the visibility of those columns.

.. _rf15:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-15.png
      :align: center
      :alt: figure 15

::
   In the above figure, we have selected a column name Support Level.
   Clicking on the arrow icon adjacent to the column name opens a dialog
   box where you can check what sub-columns to show.

.. _rf16:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-16.png
      :align: center
      :alt: figure 16

-  We save the Report.by clicking on **Create**.

We get the following Report when we :doc:`preview <preview-a-report>` for
the past 3 months and group by Technicians.

.. _rf17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-17.png
      :align: center
      :alt: figure 17

.. _create-summary-report:
Create a Summary Report
~~~~~~~~~~~~~~~~~~~~~~~

-  Open the :ref:`New Custom Report <new-custom-report>` page.

-  We are going to create a Summary Report called Asset Summary that
   summarizes OS name, memory size and hostname of computers managed by
   a Technician.

-  Following is our selections for the sections in New Custom Reports:

+-----------------------------------+-----------------------------------+
| Values                            | Section Name                      |
+===================================+===================================+
| Asset and Computer (Sub-Asset     | `Selecting a                      |
| Type)                             | Module <#selecting-a-module>`__   |
+-----------------------------------+-----------------------------------+
| Summary Report                    | `Selecting Report                 |
|                                   | Type <#selecting-report-type>`__  |
+-----------------------------------+-----------------------------------+
| Portrait                          | `Report                           |
|                                   | Layout <#report-layout>`__        |
+-----------------------------------+-----------------------------------+
| Public                            | `Report                           |
|                                   | Visibility <#report-visibility>`_ |
|                                   | _                                 |
+-----------------------------------+-----------------------------------+
| Created Time                      | `rfilter Data with                 |
|                                   | Time <#filter-data-with-time>`__  |
+-----------------------------------+-----------------------------------+
| Technician name                   | `Setting Conditions to Filter     |
|                                   | Data <#setting-conditions-to-filt |
|                                   | er-data>`__                       |
+-----------------------------------+-----------------------------------+

.. _rf18:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-18.png
      :align: center
      :alt: figure 18

-  Scroll down to the Selection Section.

.. _rf19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-19.png
      :align: center
      :alt: figure 19

-  A Summary Report can summarize properties and components of Assets.
   In this Report, we are going to summarize properties which is why we
   have selected **Computer Property Details**. We confirm our column
   selection by clicking **Done**.

.. _rf20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-20.png
      :align: center
      :alt: figure 20

-  We only want OS name, memory size and host-name which we select as
   sub-columns (Refer :numref:`rf20`).

.. _rf21:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-21.png
      :align: center
      :alt: figure 21

-  We save the Report.by clicking on **Create**.

We get the following Report when we :doc:`preview <preview-a-report>` for
the past 3 months.

.. _rf22:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-22.png
      :align: center
      :alt: figure 22

.. _create-multi-module:
Creating Multi-Module Report
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can create a Report that summarizes the output of multiple Reports.
The feature that allows you to do this is called multi-module.

-  Open the :ref:`New Custom Report <new-custom-report>` page.

-  We are going to create a Report called Multi-Module Report that has
   the output of two Reports (Computer Asset List and Average Resolution
   Time).

-  Following is our selections for the sections in New Custom Reports:

+----------------+----------------------------------------------------+
| Values         | Section Name                                       |
+================+====================================================+
| Multi-Module   | `Selecting a Module <#selecting-a-module>`__       |
+----------------+----------------------------------------------------+
| Summary Report | `Selecting Report Type <#selecting-report-type>`__ |
+----------------+----------------------------------------------------+
| Portrait       | `Report Layout <#report-layout>`__                 |
+----------------+----------------------------------------------------+
| Public         | `Report Visibility <#report-visibility>`__         |
+----------------+----------------------------------------------------+
| Created Time   | `rfilter Data with Time <#filter-data-with-time>`__ |
+----------------+----------------------------------------------------+

.. _rf23:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-23.png
      :align: center
      :alt: figure 23

-  Scroll down to the Report selection area.

.. _rf24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-24.png
      :align: center
      :alt: figure 24

-  We select the Reports that we want to add using the search features.
   We finalize our selection by clicking on **Done**.

.. _rf25:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-25.png
      :align: center
      :alt: figure 25

-  We can rearrange the order of the Reports by drag and drop.

-  We save the Report.by clicking on **Create**.

We get the following Report when we :doc:`preview <preview-a-report>` for
the past 3 months.

.. _rf26:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-26.png
      :align: center
      :alt: figure 26

.. _editing-report:
Editing a Report
----------------

*Note: A user can edit Reports that he creates.*

-  Go to the `Report List View <#_report_list_view>`__.

-  In the list area, click on the **Edit Report** button of the Report
   which you want to edit. The Update Custom Report page opens.

.. _rf27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-27.png
      :align: center
      :alt: figure 27

-  The Update Custom Report page is similar to the New Custom Report
   page.

-  You can edit the following things in Update Custom Report page:

   a. The layout of the Report.

   b. You can change the Visibility if it is already set to Private.
      Once set to public, you cannot change Visibility.

   c. The Date filter field.

   d. You can modify existing conditions or add new ones in the Criteria
      section.

   e. You can change the Group by options.

   f. Add and rearrange columns.

-  Once you are over with your editing, click **Update**.

You can also access the Update Custom Report page from :ref:`Custom
Reports <open-custom-reports>` page.

Add and Rearrange Columns
~~~~~~~~~~~~~~~~~~~~~~~~~

In the Update Custom Report page, you can change the
Column/Report/Section selection using **Modify Column/Reports/Section
Selection** button. You can rearrange the order using drag and drop.

.. _rf28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-28.png
      :align: center
      :alt: figure 28

**Deleting a Report**

*Note: A Technician is allowed to delete Reports that he/she has
created.*

-  Go to the `Report List View <#report-list-view>`__.

-  Click on **Delete Report** from the Action Menu of a Report. On
   Confirmation, the Report is deleted.

.. _rf29.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-29.1.png
      :align: center
      :alt: figure 29.1
.. _rf29.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-29.2.png
      :align: center
      :alt: figure 29.2

You can delete a Report from its :ref:`Update Custom Repor <editing-report>` page and :ref:`Custom
Reports <open-custom-reports>` page.

.. _rf30:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-30.png
      :align: center
      :alt: figure 30

.. _rf31:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-31.png
      :align: center
      :alt: figure 31
