********************
Managing a Dashboard
********************

Once a Technician (should have necessary :ref:`Permissions <dashboard-permissions>`) has created a Dashboard he can perform the following operations:

- Modifying Existing Dashboards.

- Adding/Deleting Dashlets to/from a Dashboard.

- Duplicating a Dashboard.

- View Dashboards.

- Delete a Dashboard.

- Rearrange and resize Dashlets.

Setting Filters in a Dashboards
===============================

Inside a Dashboard (accessed from :ref:`Dashboard List` page), you can change the default time and location filters. This change
will not be permanent, for that you need to :ref:`edit <Modifying Existing Dashboard>` the Dashboard.

.. _das-3.1:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-3.1.png
    :align: center
    :alt: figure 3.1

Modifying Existing Dashboard
============================

A Dashboard can be modified only by its owner. In case of :ref:`Predefined <Out of the Box Dashboards>` Dashboards, the super user is the owner.

**To Edit a Dashboard:**

- Go to the :ref:`Dashboard List` page. Here you can view all your Dashboards.

- There are two ways to access the Update Dashboard dialog box.

  a. In the Dashboard List page, you can click on **Edit** from the Action Menu of the Dashboard (which you are an owner) that you want
     to edit.

  b. Click on the Dashboard and go inside, and click on the edit icon. 

  .. _das-4:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-4.png
    :align: center
    :alt: figure 4

- In the Update Dashboard dialog box, you can update the following information:

  a. **Dashboard Name**: Choose any name you want. 

  b. **Location**: Here you can add/remove a location filter.

  c. **Time Scale**: Data will be shown within the chosen Data & Time range.

  d. **Privacy (Technician and Technician Group)**: You can share/stop-sharing your Dashboard with another Technician or a Group. 
    
- When you are done, click on **Update** to save your changes.

.. note:: Learn what can be changed with respect to :ref:`Predefined Dashboards <modify-predefined-dashboard>`.

Deleting a Dashboard
--------------------

Only Custom Dashboards can be deleted by their owners. :ref:`Predefined <Out of the Box Dashboards>` Dashboards can't be deleted. In order to make a shared Dashboard
disappear, the user has to ask the owner to stop sharing the Dashboard with him/her.

**To Delete a Dashboard:**

- Go to :ref:`Dashboard List` page. Here you can see all your existing Dashboards.

- There are two ways you can delete a Dashboard:

  a. In the Dashboard List page, you can click on **Delete** from the Action Menu of the Dashboard (which you are an owner) that you want
     to delete.

  b. Click on the Dashboard and go inside, and click on the delete icon.
  
  .. _das-5:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-5.png
    :align: center
    :alt: figure 5
    
- On confirmation the Dashboard gets deleted.

Adding Dashlets to a Dashboard
==============================

An owner of a Dashboard can add n number of Dashlets to his/her Dashboard. When it comes to :ref:`Predefined` Dashboards, the super
user is the owner, and he/she can add more Dashlets.

.. note:: Learn more about Dashlets.

**To add Dashlets to a Dashboard:**

- Open the Dashboard, where you want to add Dashlets, from the :ref:`Dashboard List` page.

- Click on the **Add Dashlet** button situated in the top right corner of the page; this opens the Dashlet panel.

.. _das-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-6.png
    :align: center
    :alt: figure 6

- There are three kinds of Dashlets you can add: KPIs, Widgets and Shortcuts. Learn more about the Dashlet types.

  You will find tabs separating the Dashlet types; within a selection, you can do the following operations:

  a. Search KPIs and Widgets by keyword.

  b. Filter KPIs and Widgets by the following conditions:

     i. KPIs/Widgets created by the Owner.

     ii. KPIs/Widgets shared with the Owner.

  c. Select multiple KPIs/Widgets/Shortcuts. 

  .. _das-7:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-7.png
       :align: center
       :alt: figure 7

- You cannot select multiple Dashlet types; you have to select and add Dashlets of one type at a time. Preselected Dashlets are
  already added. Use the **Add Select KPIs/Widgets/Shortcuts** to add your selection.

Removing Dashlets from a Dashboard
==================================

An owner of a Dashboard can remove Dashlets from his/her Dashboard. When it comes to :ref:`Predefined` Dashboards, the super
user is the owner, and he/she can remove Dashlets from such Dashboards. 

.. note::  Related Topic: Learn what can be done with a :ref:`Predefined Dashboard <modify-predefined-dashboard>`.

**To Delete a Dashlet:**

- Open the Dashboard, where you want to remove Dashlets, from the :ref:`Dashboard List` page.

- Click on **Remove from Dashboard** from the Action menu. On confirmation the Dashboard is removed.

.. _das-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-8.png
    :align: center
    :alt: figure 8

Create a Duplicate Dashboard
============================

A user can create a duplicate of a Dashboard. Duplicating a Dashboard has the following output:

- A new Dashboard is created with all the Dashlets of the original Dashboard.

- The user who created the duplicate becomes owner of the new Dashboard regardless of whether he/she is the owner of the
  original Dashboard.

- The duplicate Dashboard is shared with the same people/groups as the original unless the owner changes the privacy settings
  of the duplicate.

**To Create a Duplicate:**

- Go to the :ref:`Dashboard List` page.

- There are two ways you can duplicate a Dashboard:

  a. In the Dashboard List page, click on the duplicate icon of the Dashboard that you want to duplicate. Or

  b. Go inside the Dashboard, you will find the create duplicate icon.
  
  .. _das-9:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-9.png
       :align: center
       :alt: figure 9

- On clicking the duplicate icon, a dialog box opens where you can modify the following:

  a. Name of the Dashboard.

  b. Default location filter.

  c. Default time range for showing the data.

  d. Privacy settings (Whom to share the duplicate Dashboard with, either Technicians, Technician Groups or both).

  e. Advance settings; you can ignore time and location filters.

- When done, click on **Duplicate** to finish the process.

Making a Dashboard the Default
==============================

A user, with the :ref:`Dashboard rights <dashboard-permissions>`, can make a Dashboard his/her default. A default Dashboard is like a 
homepage for a Technician Portal user. A user can have only one Dashboard selected as default; he/she can make anyone of the Dashboards
visible on the :ref:`Dashboard List` page.

**To make a Dashboard default:**

- Go to the :ref:`Dashboard List` page.

- There are two ways you can mark a Dashboard as default:

  a. In the Dashboard List page, click on the **Mark as Default Dashboard** from the Action Menu. Or

  b. Go inside the Dashboard, you will find the **Mark as Default** situated in the top right corner of the page.

.. _das-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-10.png
    :align: center
    :alt: figure 10

- The default Dashboard will have the default label.

.. _das-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-11.png
    :align: center
    :alt: figure 11

Resizing and Rearranging Dashlets in a Dashboard
================================================

An owner of a Dashboard can rearrange and resize the added Dashlets. 

.. _das-11.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-11.1.png
    :align: center
    :alt: figure 11.1

Change Visualization of a Widget
--------------------------------

An owner of a Dashboard can change the chart type (bar chart, column chart, line chart or pie chart) of a Widget.

.. _das-11.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/dashboard/DAS-11.2.png
    :align: center
    :alt: figure 11.2
