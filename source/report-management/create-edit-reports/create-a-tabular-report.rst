.. _create-tabular-report: 

***********************
Create a Tabular Report
***********************

-  We open the :ref:`Create a Custom Report <new-custom-report>` dialog box.

-  We are going to create a Tabular Report called Computer Asset List
   that lists all computers managed by a particular Technician, group by
   Product.
-  Following is our selections/inputs for the sections in **Create a Custom Report** dialog box and **New Custom Report** page:

+-----------------------------------+--------------------------------------------+
| Values                            | Section Name                               |
+===================================+============================================+
| {Name of the Report}              | :ref:`Add a Name to the Report`            |
+-----------------------------------+--------------------------------------------+
| Asset and Computer                | :ref:`selecting a module`                  |
| (Sub-Asset Type)                  |                                            |
+-----------------------------------+--------------------------------------------+
| Tabular Report                    | :ref:`selecting report type`               |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Asset (Selecting a folder)        | :ref:`Setting the Folder of a Report`      |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Description of the Report         | :ref:`Editing the Description of a Report` |
+-----------------------------------+--------------------------------------------+
| Portrait                          | :ref:`report layout`                       |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Public                            | :ref:`report visibility`                   |
|                                   |                                            |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Created Time                      | :ref:`filter data with time`               |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Technician name                   | :ref:`setting conditions to filter data`   |
|                                   |                                            |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| Product                           | :ref:`grouping of data`                    |
|                                   |                                            |
+-----------------------------------+--------------------------------------------+
| (Sort of Status column)           |                                            |
| Ascending                         | :ref:`Sorting Columns`                     |
+-----------------------------------+--------------------------------------------+

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
   un-hide by checking a box highlighted in the above figure.

   You can also search for a column using the search bar in that
   section.

-  We select three columns for this Report. We can rearrange them using
   drag & drop. We finalize our selections by clicking on **Done**.

.. _rf11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-11.png
      :align: center
      :alt: figure 11

-  Before creating the Report, we apply the sort function to the Status column; this will sort the entire report. 

-  We save the Report by clicking on **Create**.

The process to create a Report is same for all the modules in the
system. We get the following Report when we :doc:`preview <preview-a-report>` for the past 3 months.

.. _rf12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-12.png
      :align: center
      :alt: figure 12