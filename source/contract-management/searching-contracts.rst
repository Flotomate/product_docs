*******************
Searching Contracts
*******************

Motadata gives you two broad ways to search Contracts in the :doc:`Contract List View <contract-list-view>`.

-  Using custom and predefined filters.

-  Using a search bar.

.. _con-search-bar:

Using a Search bar
==================

You can search Contracts in the Contract module using a search bar. The search bar supports the Advanced Search feature 
that allows you to use various combinations of predefined search options and keywords. If you want to
see the list of available options, then click on the search box. You can
select an option or multiple options from the drop-down list.

.. _con-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-9.png
    :align: center
    :alt: figure 9

Once you select a search option, you are required to input a value. The input area could be a text box or a drop-down list.

.. _con-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-10.png
    :align: center
    :alt: figure 10

You can also search Contracts with keywords in the search field. When you
provide a keyword, the module searches all the Contracts with the keyword
in Name, Display-name, Description, Tags, ID, and Department. 
All matched Contracts are displayed under their respective
statuses. In case of multiple keywords, all keywords need to be matched. 

You can make a filter using a chain of search options and keywords. For example; we can make a search 
query that searches all Contracts having the Vendor: Adode and keyword: 3D max.

.. _con-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-11.png
    :align: center
    :alt: figure 11

Between two different conditions of the same data type, the OR logic
prevails. Between different data types the AND logic prevails. An
example of same data type conditions is Contract Type equals Lease vs. Contract Type equals Maintenance.
Between keywords and conditions AND logic is followed.

Custom Filter
-------------

You can save search queries that you create using search options and keywords. To save a search query, click on the
star icon to the far right of the box and give a name to the query.

.. _con-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-12.png
    :align: center
    :alt: figure 12

The saved search queries appear on top of the :doc:`contract-list-view`.

.. _con-13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-13.png
    :align: center
    :alt: figure 13

.. _con-using-filters:

Using Filters
=============

The module has filters to sort the Contracts List using the following
criteria:

- Duration of the Contracts.

- Status of the Contracts.

- Contract Type.

The module has time based filters with regards to Open, Expired and Cancelled Contracts out of the box.
You can find them in the header section of the :doc:`contract-list-view`. 

.. _con-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-14.png
    :align: center
    :alt: figure 14

Selecting any one filter populates the list area with Contracts
satisfying the filter’s conditions. All six filters have different
conditions, which are:

+-----------------------------------+---------------------------------------------------------------------+
| All Open Contracts                | Shows all Contracts with the status Open.                           |
+-----------------------------------+---------------------------------------------------------------------+
| Contract Expired in Last 15 days  | Contracts that went into the Expired status in the last 15 days.    |
+-----------------------------------+---------------------------------------------------------------------+
| Contract Expiring in Next 15 days | Contracts that will go into the Expired status in the next 15 days. |
+-----------------------------------+---------------------------------------------------------------------+
| Contract Expiring in Next 30 days | Contracts that will go into the Expired status in the next 30 days. |
+-----------------------------------+---------------------------------------------------------------------+
| All Expired Contracts             | Shows all Contracts with the status Expired.                        |
+-----------------------------------+---------------------------------------------------------------------+
| All Cancelled Contracts           | Shows all Contracts with the status Cancelled.                      |
+-----------------------------------+---------------------------------------------------------------------+ 

You can also filter Contracts by status. There are currently four statuses. Selecting any one populates the
list area with Contracts having that status.

.. _con-15:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-15.png
    :align: center
    :alt: figure 15

.. note:: Learn more about :ref:`Statuses<con-status>`.

You can filter Contracts by Contract Type (ref: :numref:`con-15`). We provide four types out of the box. You can add more types
(Learn more about :doc:`contract-type`). 