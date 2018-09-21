*************************
Out of the Box Dashboards
*************************

Flotomate ITSM tool provides four predefined Dashboards out of the box. Each of them have a theme that showcases specific Dashlets.
These Dashboards have the following features:

- Predefined Dashboards are shared with all users having the :ref:`Dashboard rights`.

- The super user is the owner of all Predefined Dashboards.

- Only the super user can modify (even add Dashlets) a Predefined Dashboard but cannot delete it.

- The Helpdesk Dashboard (one of the Predefined Dashboards) is the Default Dashboard for every user regardless of :ref:`user rights <dashboard-permissions>`.

The Predefined Dashboards are as follows:

.. note:: A user can view the Predefined Dashboards from the :ref:`Dashboard List`. 

1. **Helpdesk Dashboard**: This Dashboard shows key metrics from the :ref:`Request Management <what-is-request>` module. The idea
   behind the Dashboard is to give a snapshot of the efficiency with which Technicians are solving Request tickets. Here you get the
   following Dashlets and filters:

   a. Data range (filter) of last 7 days and all locations.

   b. Count of Open and Closed filter (KPI).

   c. Count of overdue and unassigned tickets (KPI).

   d. Graphical representation (widget) of ticket count by categories (for the given time range).

   e. Graphical representation (widget) of ticket count by Priority (for the given time range).

   f. Graphical representation (widget) of ticket count by Technician's Request count by priority (for the given time range).

   g. Graphical representation (widget) of ticket count by Technician's SLA violation by day (for the given time range).

   .. note:: This is the default Dashboard when you open Dashboard for the first time.

.. _modify-predefined-dashboard:

What can be done to a Predefined Dashboard?
===========================================

Users can perform the following operations on a Predefined Dashboard:

- Any user can make a duplicate of a Predefined Dashboard.

- The super admin (only) can update the Name, Location filter and date range filter of a Predefined Dashboard.

- The super admin (only) can view definition of, update and delete a Dashlet from a Predefined Dashboard.

- The super admin (only) can create new Dashlets (KPIs and Widgets) and add them to a Predefined Dashboard.

- The super admin (only) can resize a Widget block on a Predefined Dashboard.