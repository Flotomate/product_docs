.. _create-matrix-report:

**********************
Create a Matrix Report
**********************

-  We open the :ref:`Create a Custom Report <new-custom-report>` dialog box.

-  We are going to create a Matrix Report called Average Resolution Time
   that shows the average resolution time of each Technicians along with
   the Request number bifurcated across support levels.

-  Following is our selections/inputs for the sections in **Create a Custom Report** dialog box and **New Custom Report** page:

+-----------------------------------+---------------------------------------------+
| Values                            | Section Name                                |
+===================================+=============================================+
| {Name of the Report}              | :ref:`Add a Name to the Report`             |
+-----------------------------------+---------------------------------------------+
| Request                           | :ref:`selecting a module`                   |      
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Matrix Report                     | :ref:`selecting report type`                |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Request (Report folder)           | :ref:`Setting the Folder of a Report`       |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Description of the Report         | :ref:`Editing the Description of a Report`  |
+-----------------------------------+---------------------------------------------+
| Portrait                          | :ref:`report layout`                        |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Public                            | :ref:`report visibility`                    |
|                                   |                                             |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Created Time                      | :ref:`filter data with time`                |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Status Equals to Closed           | :ref:`setting conditions to filter data`    |
|                                   |                                             |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+
| Technician                        | :ref:`grouping of data`                     |
|                                   |                                             |
+-----------------------------------+---------------------------------------------+

.. _rf13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-13.png
      :align: center
      :alt: figure 13

-  Scroll down to *Select Column* section of the page.

.. _rf14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-14.png
      :align: center
      :alt: figure 14

-  A Matrix Report gives you a cumulative count of data; for example,
   the total number of Requests assigned to each Technician. In :numref:
   `rf14`, Average is the function mentioned in the first box, and the second
   box shows you the column names supporting the average function. Each
   module has different column names. You can add more columns using the
   Plus Icon.

   We select two columns and click on **Done** to finalize our decision.

   It may happen a column name may generate additional columns. You can
   control the visibility of those columns.

    .. _rf15:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-15.png
          :align: center
          :alt: figure 15

   In the above figure, we have selected a column name Support Level.
   Clicking on the arrow icon adjacent to the column name opens a dialog
   box where you can check what sub-columns to show.

    .. _rf16:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-16.png
          :align: center
          :alt: figure 16

- We don't apply any sort function to any column; we select **None** for sorting. 

-  We save the Report.by clicking on **Create**.

We get the following Report when we :doc:`preview <preview-a-report>` for
the past 3 months and group by Technicians.

.. _rf17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/report/R-17.png
      :align: center
      :alt: figure 17