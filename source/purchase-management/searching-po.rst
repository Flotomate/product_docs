*************************
Searching Purchase Orders
*************************

The Purchase Management module gives you two broad ways to search Purchase Orders in :doc:`Purchase List
View <purchase-list-view>`.

-  Using custom and predefined filters.

-  Using a search bar.

Search bar
==========

Purchase List View has a search box for searching POs. The search box supports the Advanced Search feature
that allows you to use various combinations of predefined search options and keywords. If you want to
see the list of available options, then click on the Search Box. You can
select an option or multiple options from a drop-down menu.

.. _pur-13:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-13.png
    :align: center
    :alt: figure 13

Once you select a search option, you are required to input a value. The input area could be a text box or a drop-down list.

.. _pur-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-14.png
    :align: center
    :alt: figure 14
    
You can search POs with keywords. When you provide a keyword,
Motadata examines all the POs with the keyword in Name,
Description, Remark, Terms, Place, Signing Authority and PO ID fields. All matched
POs get displayed in the list area. In case of multiple keywords,
all keywords need to be matched.

You can make a filter using a chain of search options and keywords. For example; we can make a search 
query that searches all POs having the Vendor: Sales India and keyword: Dell.

.. _pur-15:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-15.png
    :align: center
    :alt: figure 15

Between two different conditions of the same data type, the OR logic
prevails. Between different data types the AND logic prevails. An
example of same data type conditions is Billing Location equals Pune vs. Billing Location equals Ahmedabad.
Between keywords and conditions AND logic is followed.   

Custom filters
--------------

You can save search queries that you create using search options and keywords. To save a search query, click on the
star icon to the far right of the box and give a name to the query.

.. _pur-16:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-16.png
    :align: center
    :alt: figure 15

The saved search queries appear on top of the :doc:`purchase-list-view`.

.. _pur-17:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-17.png
    :align: center
    :alt: figure 17

Using filters
=============

The module has filters to sort the Purchase Order List using the following
criteria:

- Due status and ownership of the POs.

- Stage wise filter

You get the following filters to filter POs based on due status and ownership.

.. _pur-18:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-18.png
    :align: center
    :alt: figure 18

+---------------------------+-----------------------------------------------------+
| All Purchase Order        | Shows all POs that are neither Closed or Cancelled. |
+---------------------------+-----------------------------------------------------+
| My Purchase Order         | Shows POs assigned to the Technician logged in.     |
+---------------------------+-----------------------------------------------------+
| My Overdue Purchase Order | Shows POs that have past their due date.            |
+---------------------------+-----------------------------------------------------+
| POs Overdue in 7 Days     | Shows POs that are going to past their due date in  |
|                           | 7 days.                                             |
+---------------------------+-----------------------------------------------------+
| POs Overdue in 30 Days    | Shows POs that are going to past their due date in  |
|                           | 30 days.                                            |
+---------------------------+-----------------------------------------------------+

You can filter POs based on their present status. There are eight statuses to choose from:

.. _pur-19:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/purchase-management/PUR-19.png
    :align: center
    :alt: figure 19
