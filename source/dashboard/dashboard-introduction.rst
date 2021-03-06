********************************
Motadata Dashboard Introduction
********************************

Modern businesses are driven by data. Proper data plays the foundation for effective monitoring and improvement of service delivery. 
A Dashboard provides a glance-view of key KPIs and relevant data. Data shown on a Dashboard can be filtered to reflect a particular business
process. A Dashboard can also contain important links (as shortcuts). 

Motadata gives a robust Dashboard that is customizable and can show data in n number of ways. Some of the advantages of using the
Motadata Dashboard are as follows:

- A Dashboard is an empty canvas where a user can add custom data blocks (Dashlets) to present the most valuable and useful set of information.

- A Dashboard allows a user to see, at a glance, an overall situation report of the desired information.

- A Dashboard enables a user to drill down into the details by simply selecting the desired variable and object.

- An easy graphical interface allows a user to play with data and do easy cross-sectional analysis.

- A Dashboard can be a one page snapshot of key matrices of a business. A user of the Motadata Dashboard can quickly judge how
  well the Helpdesk is functioning.

Components of a Dashboard
=========================

A user can create multiple Dashboards, each can show different data blocks. A Dashboard can be shared with multiple users; even individual 
data blocks can be shared with multiple users. 

A Dashboard is like an empty canvas where a user can add multiple data blocks (Dashlets). A Dashboard is a container for multiple Dashlets (data blocks).
There are two main components of a Dashboard:

- **Filters**: A Dashboard has two filters based on which data is shown; they are: Date & Time range and Location filter.
  If both the filters are set, then a data point has to satisfy both the set filter conditions. 

  The location filter shows exclusively the data points having the set location; for example, if location is set to Ahmedabad then
  all KPIs and Widgets will show data of that particular location. Filters are not applicable on Shortcuts.

- **Dashlet**: A Dashlet is a single data block in a Dashboard. Currently, we support three kinds of Dashlets:

  a. **KPI**: A KPI (Key Performance Indicator) is a measurable value which helps in deducing efficiency of a system. For example;
     number of resolved Request tickets over the last 30 days is one of many indicators of efficiency of the Helpdesk.

  b. **Widgets**: A Widget is a graphical representation of data filtered by time and other parameters.
     
  c. **Shortcuts**: It is a list of Frequent Access Items (i.e. My Open Incidents, My Approval, My Tasks etc.).

Support Modules
===============

Currently, Dashboards can be created relating to the following modules:

- Incident/Service Request

- Problem

- Change

- Asset Management

- Patches

.. _dashboard-permissions:

Who Can Work with Dashboards?
=============================

A Technician with the following :ref:`roles <Technician Roles>` (Admin >> Technician Roles) can work with the Motadata Dashboard:

- **Manage Dashboard**: User can only create Dashboards and add Predefined Dashlets, but he/she can't create new Dashlets.

- **Manage KPI and Widget**: Same as above except he/she can create new Dashlets.