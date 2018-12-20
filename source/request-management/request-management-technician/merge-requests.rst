**************
Merge Requests
**************

Sometimes two or more Requests are similar, or they are duplicates The
Merge function in Flotomate helps in dealing with duplicates and similar
Requests.

In the Merge process, one is the Primary Request, and all others are
Secondary. The outcome of a merge is always the Secondary Requests
linked to the Primary Request. If the Merge process happens between
Requests created by the same Requestor, then all the Secondary Requests
are closed, but they stay linked with the Primary Request.

Doing a Merge:
==============

1. Log in to the Technician Portal.

2. Go to **Request** >> :doc:`Request List View <request-list-view>`.

.. _rmf-69:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-69.png
    :align: center
    :alt: figure 69

3. Select two or more Requests, and the **Merge** option appears over
   the list area.

.. _rmf-70:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-70.png
    :align: center
    :alt: figure 70

4. Clicking on **Merge** takes you to a new dialog box. Here you can
   choose which one to keep as Primary and which one, Secondary.
   Referring to :numref:`rmf-70`, section-A shows the Primary Request (which
   can only be one) and section-B lists the Secondary. Clicking on the
   symbol adjacent to a Request (S & P) changes a Request from Primary
   to Secondary and vice-versa.

   Section-C is the search area. You can use the search area to find
   specific Requests by using custom keywords and predefined search
   options. The Search Box works similarly to the :doc:`Search Box <searching-requests>` in List View.

   Below the Search Box is a list of other Requests. If no search filter
   is applied, then the list contains all the other Requests not
   selected for merge. Section-D allows you to select multiple Requests.
   The total number of selected Requests appears on top of the Search
   Box along with the symbol S. Click on the S symbol to add them to the
   Secondary Request area.

5. Click **Merge** once you are done with the setup. The Merge process
   closes all those Secondary Requests with the same Requestor email,
   treating them as duplicate, as in the Primary Request. Requests with
   a different email stay open.

Viewing the Relation of a Primary Request:
==========================================

You can see the effect of merge under **Relations** tab in the Primary
Request’s Details View.

.. _rmf-71:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-71.png
    :align: center
    :alt: figure 71