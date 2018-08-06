******************
Searching Problems
******************

Flotomate gives you two broad ways to search Problems in the :ref:`Problem List
View <problem-list-view>`.

-  Using custom and predefined filters.

-  Using a search bar.

Using a Search Bar
==================

Flotomate allows you to perform an Advanced Search using various
combinations of predefined search options and keywords. If you want to
see the list of available options, then click on the search box. You can
select an option or multiple options from the drop-down list.

.. _pmf-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/problem-management/PM-9.png
    :align: center
    :alt: figure 9

You can also search Problems with keywords in the search field. When you
provide a keyword, the module searches all the Problems with the keyword
in Subject, Description, Tags, Symptom, Root Cause, Requester Email and
ID fields. All matched Problems are displayed under their respective
statuses. In case of multiple keywords, all keywords need to be matched.

You can make a filter using a chain of predefined search options and
keywords. You can save your search queries, refer :numref:`pmf-10`. Saved
search queries appear in the section-A’s menu list (:numref:`pmf-5`).

For example; if you are looking for all Problems containing the word
email in the Subject line and have a low priority. You would have the
following search query (:numref:`pmf-10`):

.. _pmf-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/problem-management/PM-10.png
    :align: center
    :alt: figure 10

Between two different conditions of the same data (option) type OR logic
prevails. Between different data (option) types, AND logic prevails. An
example of a same type conditions is Status Open vs. Status Closed.
Between keywords and conditions AND logic is followed.

.. _pmf-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/problem-management/PM-11.png
    :align: center
    :alt: figure 11

Using Filters
=============

The product has filters to sort the Product List by following criteria:

-  Status

-  Resolution

-  Priority

-  Error Type

-  Assignee

-  Due-date status

Go to the Problem List View. In the List View, clicking on the header
section (Section-A :numref:`pmf-5`) gives you a popup menu containing seven
predefined filters.

.. _pmf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/problem-management/PM-12.png
    :align: center
    :alt: figure 12

Selecting any one filter populates the list with Problems satisfying the
filter’s conditions. All seven filters have different conditions, which
are:

+-----------------------------------+-----------------------------------+
| **All Open Problems**             | It includes all the Unclosed      |
|                                   | Problems available in the system. |
+-----------------------------------+-----------------------------------+
| **All Reactive Problems**         | It shows all the unclosed         |
|                                   | Problems with the                 |
|                                   | Nature-of-Problem as Reactive.    |
+-----------------------------------+-----------------------------------+
| **All Unanalyzed Problems**       | It shows all the unclosed,        |
|                                   | unresolved Problems with          |
|                                   | incomplete Investigation          |
|                                   | (Systems, Root Cause, and         |
|                                   | Impact).                          |
+-----------------------------------+-----------------------------------+
| **My Unresolved Problems**        | It includes all the unclosed,     |
|                                   | unresolved Problems assigned to   |
|                                   | you.                              |
+-----------------------------------+-----------------------------------+
| **My Urgent or High Priority      | It includes all the unclosed,     |
| Problems**                        | unresolved Problems assigned to   |
|                                   | you with either High or Urgent    |
|                                   | priority.                         |
+-----------------------------------+-----------------------------------+
| **My Overdue Problems**           | Includes all the unclosed,        |
|                                   | unresolved Problems assigned to   |
|                                   | you that are past their due date. |
+-----------------------------------+-----------------------------------+
| **Unassigned Problems in My       | Includes all the unclosed,        |
| Group**                           | unresolved Problems with a        |
|                                   | Technician Group that you are     |
|                                   | part of.                          |
+-----------------------------------+-----------------------------------+

There are status based filters in Section-B (:numref:`pmf-5`) of List View that
tells you about the distribution of Problems under various predefined
and custom statuses.

.. _pmf-13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/problem-management/PM-13.png
    :align: center
    :alt: figure 13

You can create and manage custom statuses, but you cannot change some
statuses, which are:

-  Open

-  Pending on Requester

-  Pending in Approval (This :ref:`status <classify-a-problem>` can only be set by
   the system when the Problem is in :ref:`Approval <pm-asking-for-approval>`
   stage.)

-  Pending on Technician

-  Resolved

-  Closed

Please refer Problem Custom Status (Customization and Configuration) in
the Administration manual to learn how to create Custom Statuses.

The product can also show you the distribution of all the unclosed
Problems across the priority levels, error type, assignment status, and
Due-date statuses.

.. _pmf-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/problem-management/PM-14.png
    :align: center
    :alt: figure 14

Additional tags appear when one or more Problems are about to reach
their Due-dates. The maximum time-frame to show due is 24 hours.