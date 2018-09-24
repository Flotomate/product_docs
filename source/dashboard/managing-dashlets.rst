*****************
Managing Dashlets
*****************

A Dashboard is like an empty canvas, and Dashlets are data blocks showing specific data. Multiple Dashlets together give contextual 
meaning to a Dashboard. There are n number of permutations that can be achieved using different kinds of Dashlets all showing 
different data. 

We currently have three kinds of Dashlets:

- **KPI**: The abbreviation stands for Key Performance Indicator which is a counter of occurrences satisfying a preset condition.
  For example, there could be a KPI that shows the number of Request tickets having reopen count greater than 0. 

.. _das-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-12.png
    :align: center
    :alt: figure 12

- **Widget**: A widget shows data points graphically across x and y coordinates or as proportions. For example, count of Problem
  tickets can be shown across priorities using a bar chart. 

.. _das-13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-13.png
    :align: center
    :alt: figure 13

- **Shortcut**: It is a predefined box that shows specific system data; for example, there is a Shortcut box called My Open Request
  that shows recent open Requests assigned to you. 

.. _das-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-14.png
    :align: center
    :alt: figure 14

A user having the necessary :ref:` Dashboard permissions <dashboard-permissions>` can perform the following operations with Dashlets:

- View Dashlets, along with their parameters.

- Create custom Dashlets (not possible with Shortcuts).

- Edit existing Dashlets (not possible with Shortcuts).

- Create duplicate of a Dashlet (not possible with Shortcuts).

- Delete a custom Dashlet (not possible with Shortcuts and predefined Dashlets).

Creating a Custom Dashlet
=========================

If you have the necessary :ref:`permissions <dashboard-permissions>`, you can create n number of  custom Dashlets (only KPIs and Widgets) apart from the 
predefined Dashlets. 


Accessing the Dashlet panel
---------------------------

- Go to the :ref:`Dashboard List` page.

- Go inside a Dashboard (only a super user can open a predefined Dashlet).

- Click on **Add Dashlet** situated in the top right corner.

.. _das-15:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-15.png
    :align: center
    :alt: figure 15

Create a KPI
------------

- In the :ref:`Dashlet panel <Accessing the Dashlet panel>`, select the KPI tab and click on **Create KPI**.

.. _das-15.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-15.1.png
    :align: center
    :alt: figure 15.1

- A dialog box opens where you can provide the following inputs:

    .. _das-16:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-16.png
        :align: center
        :alt: figure 16

  a. Name of KPI.

  b. Name of the module of which the KPI belongs (either Request, Problem, Change or Asset).

  c. **Data Filter Parameter**: It allows you to filter data using time. When
     filtering ticket and Asset data, one of the below mentioned type of time data is considered, depending on your module selection.

        i.  **Created Time**: This option is valid for all modules. A Dashboard has a time filter; using this option makes a KPI to
            show only those data points whose create time falls within the selected time period. For example, a KPI that shows the 
            number of Assets added in a time period will consider the create time of each Asset.  

        ii.  **Updated Time**: This option is valid for all modules. Instead of Create Time, the system uses the Update
             Time in checking data.

        iii.  **Closed Time**: This option is valid for only Request, Problem and Change. 
              The closed time of a ticket/item is considered to check whether it falls within a specified period.

  d. Selecting an Asset Type when Asset module is selected. Accordingly the parameter list will be updated. 
  
  e. Description of the KPI.

  f. **Data Filter**: A KPI is a counter that shows the number of times a condition/set of conditions were satisfied.
     A condition is created using parameters. For example; **Priority Equals to Low** for Request module will show the count of 
     Requests with Priority Low for a specific time period. 

     Multiple conditions can be clubbed together using AND and OR. See below for example:

     .. _das-17:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-17.png
         :align: center
         :alt: figure 17

     With the above conditions, the KPI will show all computers with the Windows OS that have been manually added. 

     We can also group the conditions and put a AND and OR between them. A condition group supports up to two conditions.

     .. _das-18:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-18.png
         :align: center
         :alt: figure 18
      
     With the above conditions, the KPI will show all computers that have been manually added either with Windows OS or Hostname Hulk or both.

  g. **Privacy Settings**: You can share the KPI with specific Technicians and Groups; they will able to view the KPI but not edit or
     delete it. 
     
     .. _das-19:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-19.png
         :align: center
         :alt: figure 19

  h. **Advance Settings**: By checking the Time and Location options, you can make the KPI ignore the Time and Location filters of a 
     Dashboard.

- When done, click on **Create** to add the KPI under the KPI tab.

Creating a Widget
-----------------

- In the :ref:`Dashlet panel <Accessing the Dashlet panel>` select the Widget tab.

.. _das-20:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-20.png
    :align: center
    :alt: figure 20

- Click on **Create Widget** in the top right corner.

- A dialog box opens where you can provide the following inputs:

    .. _das-21:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-21.png
        :align: center
        :alt: figure 21

    a. Name of the Widget.

    b. Module name of which the widget will show data.

    c. **Data Filter Parameter**: It allows you to filter data using time. When
       filtering ticket and Asset data, one of the below mentioned type of time data is considered, depending on your module selection.

        i. **Created Time**: This option is valid for all modules. A Dashboard has a time filter; using this option makes a widget to
           show only those data points whose create time falls within the selected time period. For example, a widget that shows the 
           number of Assets added in a time period will consider the create time of each Asset.  

        ii. **Updated Time**: This option is valid for all modules. Instead of Create Time, the system uses the Update
            Time in checking data.

        iii. **Closed Time**: This option is valid for only Request, Problem and Change. 
             The closed time of a ticket/item is considered to check whether it falls within a specified period.
 
        iv.  **Warranty Expiration Date**: Warranty Expiration Date of an Hardware Asset (including all its children) 
             is considered to check whether it falls within a specified period.
 
        v. **Acquisition Date**: Acquisition Date of an Hardware Asset (including all its children) 
           is considered to check whether it falls within a specified period.

        vi. **Audit Date**: Audit Date of an Hardware Asset (including all its children) 
            is considered to check whether it falls within a specified period.    
    
    d. Description of the widget. 

    e. **Data Filter**: A widget graphically shows the count/average of data points categorically as a chart. Here what data to use you
       can decide using a condition or set of conditions (filters). A condition is created using parameters. For example; **SLA Violation Equals to True** for Request module will show tickets
       that have violated the SLA resolution time for a specific time period. 

       Filters can be made using multiple conditions all connected by logical operators: AND and OR. Conditions can be grouped together as well.

       .. _das-21.1:
       .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-21.1.png
        :align: center
        :alt: figure 21.1

       With the above conditions, the widget will filter all Request tickets with SLA violation either with Priority anything other
       than low or Impact on Department or both. 

    f. **Charting Options**: Here you decide how to represent the filtered data.

       .. _das-21.2:
       .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-21.2.png
        :align: center
        :alt: figure 21.2

       i. The filter data will have parameters, which any one you can choose to show on the X axis. The above diagram, 
          The Priority parameter has been selected to be represented on x axis.

       ii. The y axis holds functions; here (:numref:`das-21.2`) we use the Count function to count Request tickets across priorities.
           We disable the value **Low** for the parameter Priority.

           .. _das-21.3:
           .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-21.3.png
                :align: center
                :alt: figure 21.3

       iii. We select a Chart type from bar (column) chart, line chart and pie chart. 

       iv.  We can select a Count Type from: 

            **First**: X axis will be sorted (based on count) in descending order.
 
            **Last**: X axis will be sorted (based on count) in ascending order.

    g. Learn more about :ref:`Privacy <Sharing a Dashlet>` and :ref:`Advanced Settings <Ignoring Time and Location Filters (Advanced Settings)>`.

- When done, click on **Create** to add the Widget under the Widget tab.
    
Searching and Filtering Dashlets
================================

In the :ref:`Dashlet panel <Accessing the Dashlet panel>`, a user can search and filter Dashlets across KPIs and Widgets; the search
features are not available for Shortcuts. There are two ways you can search for a Dashlet:

.. _das-SFD1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-SFD1.png
     :align: center
     :alt: figure 1

1. Keyword based search box.

2. **Filters**: You get three filters for KPIs and Widgets.

   a. All Predefined KPIs/Widgets.
   
   b. All KPIs/Widgets created by you.

   c. All KPIs/Widgets shared with you.

Viewing and Editing Dashlets
============================

.. note:: Only the super user can edit predefined Dashlets (barring Shortcuts).

All user with the :ref:`Dashboard rights <dashboard-permissions>` can view the definition of a KPI and Widget. But only a owner of 
a Dashlet (KPI or Widget) can edit its definition.

- Go to the :ref:`Dashboard List` page and open a Dashboard.

- You can view the definition of a KPI and Widget. 

.. _das-22:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-22.png
    :align: center
    :alt: figure 22

- The definition dialog box shows the parameters and details of a KPI and Widget.

.. _das-23:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-23.png
    :align: center
    :alt: figure 23

- If you are an owner, a edit button will be visible on the definition box, which you can use to edit the details and parameters
  of a KPI and Widget.

- You can also access the definition box from the :ref:`Dashlet panel <Accessing the Dashlet panel>` by clicking on the Dashlet name.

.. note:: Related topic: Learn how to :ref:`create a Dashlet <Creating a Custom Dashlet>`.

Sharing a Dashlet
=================

.. note:: Predefined Dashlets are shared with all by default.

The following Dashlet types can be shared: KPIs and Widgets.

An owner can share a Dashlet when creating it and later from its :ref:`definition <Viewing and Editing Dashlets>`. Sharing
can be done with specific Technicians or a Group/Groups.

.. _das-24:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-24.png
    :align: center
    :alt: figure 24

A shared Dashlet can only be viewed and added.

Create a Duplicate Dashlet
==========================

A user can create a duplicate of a Dashlet (barring Shortcuts). Duplicating a Dashlet has the following output:

- A new Dashlet is created with all the parameters and details of the original Dashlet.

- The user who created the duplicate becomes owner of the new Dashlet regardless of whether he/she is the owner of the
  original Dashlet.

- The duplicate Dashlet is shared with the same people/groups as the original unless the owner changes the privacy settings
  of the duplicate.

**To Create a Duplicate:**

- Open a Dashboard from the :ref:`Dashboard List` page and access the Dashlet panel by clicking **Add Dashlet**.
 
- Barring from Shortcuts, all KPIs and Widgets have the duplicate icon. Click the duplicate icon of the Dashlet that you want to
  duplicate. 

- A dialog box opens where you can edit the following things:

  a. Name of the Dashlet.

  b. Data Filter Parameters.

  c. Description of the Dashlet.

  d. Data filter condition/conditions.

  e. In widgets, you can change the default chart type, and the associated data and function with the axises. 

  f. Top count type.

  g. Privacy and advance settings.

- When done, click on **Duplicate**, and the new Dashlet will be added to the Dashlet panel.

Deleting a Dashlet
==================

.. note::  Predefined Dashlets cannot be deleted by any user. 

Owner of a custom Dashlet (KPI or widget) can delete it from the :ref:`Dashlet panel <Accessing the Dashlet panel>`.

.. _das-25:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-25.png
    :align: center
    :alt: figure 25

Ignoring Time and Location Filters (Advanced Settings)
=====================================================

When :ref:`editing a custom Dashlet <Viewing and Editing Dashlets>` (barring Shortcuts). You can make it ignore the time and Location
filter of a Dashboard; the options are under the Advanced settings. 