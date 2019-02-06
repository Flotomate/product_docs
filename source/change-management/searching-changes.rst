*****************
Searching Changes 
*****************

There are two broad ways to search a Change in the :doc:`List View <change-workflow>`.

-  Using a search bar

-  Using custom and predefined filters

Using Search Bar
================

Flotomate has a search bar for searching all available Changes in the
system. It supports the Advanced Search feature which allows a technician to use
a combination of pre-defined search options and keywords. If the technician want to
see the list of available options, then he has to click on the search bar. Technician can
select an option or multiple options from the drop-down list.

.. _cmf-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-10.png
    :align: center
    :alt: figure 10

A technician can search Changes with keywords from the search field. When the technician
provide a keyword, Flotomate searches all the Changes with the keyword
in Subject, Description, Tags, Symptom, Root Cause, Requester Email and
ID fields. The tool shows all matched Changes in the list area. In
case of multiple keywords, all keywords need to be matched.

.. _cmf-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-11.png
    :align: center
    :alt: figure 11

A technician can make a query using a chain of predefined options and keywords.
The technician can save a search query as a filter, refer :numref:`cmf-11`. Saved search
queries appear in the section-A of :numref:`cmf-6`.

For example, a technician looking for all Changes containing the word Server
in the Subject line and have a medium Priority; he would have the
following search query:

.. _cmf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-12.png
    :align: center
    :alt: figure 12

Between two different conditions of the same data type OR logic
prevails. Between different data types, AND logic prevails. An example
of same type conditions is Change Type Emergency vs. Change Type Normal
Change. Between keywords and conditions AND logic is followed.

Using Filters
=============

-  The header section of the List View offers five quick filters to sort
   the Change list. They are as follows:

    .. _cmf-13:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-13.png
        :align: center
        :alt: figure 13

    a. **All Open Changes**: It shows all the unclosed Changes in the
       system.

    b. **All Emergency Changes**: It shows all Changes with the Change Type
       set to Emergency.

    c. **My Open Changes**: It shows all unclosed Changes with the signed-in technician as the
       assignee.

    d. **My Over Due Changes**: It shows all Changes past their due date
       with the signed-in technician as the assignee.

    e. **All Open Changes in My Group**: It shows all the Changes with a
       Technician Group that the signed-in technician is part of.

-  A technician can filter the available Changes in the List View based on their
   stage. The tools for this is available in Change List View. The tool
   also gives the technician a quick view of the distribution of all the Changes
   across all the stages.

.. _cmf-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/change-management/CM-14.png
    :align: center
    :alt: figure 14
