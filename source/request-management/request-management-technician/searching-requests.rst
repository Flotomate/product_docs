******************
Searching Requests
******************

Motadata gives you two broad ways to search Requests in :doc:`Request List
View <request-list-view>`.

-  Using custom and predefined filters.

-  Using a search bar.

Using a Search Bar
==================

The product allows you to perform Advanced Search using various
combinations of predefined search options and keywords. If you want to
see the list of available options, then click on the Search Box. You can
select an option or multiple options from a drop-down menu.

.. _rmf-9:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-9.png
    :align: center
    :alt: figure 9

    Search options for request tickets. 

You can search Requests with keywords. When you provide a keyword,
Motadata examines all the Requests with the keyword in Subject,
Description, Solution, Tags, Requestor Email, and ID fields. All matched
Requests get displayed in the list area. In case of multiple keywords,
all keywords need to be matched.

You can make a filter using a chain of search options and keywords. For example, if you are looking for all Requests containing the keyword SLA
and have an Impact on a Department. You have the search query in :numref:`rmf-10`.

.. _rmf-10:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-10.png
    :align: center
    :alt: figure 10

Between two different conditions of the same data type, the OR logic
prevails. Between different data types the AND logic prevails. An
example of same data type conditions is Status Open vs. Status Closed.
Between keywords and conditions AND logic is followed.

.. _rmf-11:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-11.png
    :align: center
    :alt: figure 11

Save Search queries
-------------------

You can save your search queries, refer :numref:`rmf-10`. Saved search queries
appear in the section-A’s menu list (:numref:`rmf-5`).

.. _rmf-9.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-9.1.png
    :align: center
    :alt: figure 9.1

Using Filters
=============

The product has filters to sort Requests List using the following
criteria:

-  Status

-  Priority

-  Assignee

-  SLA

Go to the :doc:`Request List View <request-list-view>`. In the List View,
clicking on the header section (Section-A :numref:`rmf-5`) gives you a popup
menu containing seven predefined filters.

.. _rmf-12:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-12.png
    :align: center
    :alt: figure 12

Selecting any one filter populates the list area with Requests
satisfying the filter’s conditions. All seven filters have different
conditions, which are:

+-----------------------------------+-----------------------------------+
| All Open Request                  | It shows all the Unclosed         |
|                                   | Requests available in the system. |
+-----------------------------------+-----------------------------------+
| My Unresolved Request             | It includes all the unclosed,     |
|                                   | unresolved Requests assigned to   |
|                                   | you.                              |
+-----------------------------------+-----------------------------------+
| My Urgent or High Priority        | It includes all the unclosed,     |
| Request                           | unresolved Requests assigned to   |
|                                   | you with either High or Urgent    |
|                                   | priority.                         |
+-----------------------------------+-----------------------------------+
| My Overdue Request                | Includes all the unclosed,        |
|                                   | unresolved Requests assigned to   |
|                                   | you that are past their due date. |
+-----------------------------------+-----------------------------------+
| Urgent or High Priority Request   | It includes all the unresolved,   |
| in My Group                       | unclosed Requests with either     |
|                                   | High or Urgent priority and with  |
|                                   | a Technician Group that you are   |
|                                   | part of.                          |
+-----------------------------------+-----------------------------------+
| Unassigned Request in My Group    | It includes all the open,         |
|                                   | unassigned Requests with a        |
|                                   | Technician Group that you are     |
|                                   | part of.                          |
+-----------------------------------+-----------------------------------+
| All Un-analysed Request           | It shows all the Requests without |
|                                   | a Diagnosis.                      |
+-----------------------------------+-----------------------------------+

There are status based filters in Section-B (:numref:`rmf-5`) of List View that
tell you about the distribution of Requests under various predefined and
custom statuses.

.. _rmf-13:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-13.png
    :align: center
    :alt: figure 13

You can create and manage custom statuses, but you cannot change some
statuses, which are:

-  Open

-  Pending on Requester

-  Pending in Approval (This :ref:`status <classify-requests>` can only be set by
   the system when the Request is in the :ref:`Approval <rm-asking-for-approval>` stage.)

-  Pending on Technician

-  Resolved

-  Closed

Please refer :doc:`Request Custom Status <admin-customization>` (Customization and Configuration) in
the Administration manual to learn how to create Custom Statuses.

The product can also show you the distribution of all the unclosed
Requests across the priority levels and SLA statuses.

.. _rmf-14:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-14.png
    :align: center
    :alt: figure 14

Additional tags appear when one or more Requests are about to reach
their Due-dates. The maximum time-frame to show due is 24 hours.