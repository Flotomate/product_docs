**********************
Consolidating Software
**********************

It is common for a computer to have a software suite like MS Office. A
Software suite is a collection of computer programs. Flotomate allows
you to create a bundle of software with one as the Primary and the rest
as Secondary. This way you can consolidate multiple Software Assets into
one.

1. Go to the :doc:`Asset List View<asset-list-view>` of the class
   Software IT Asset.

2. In the Asset List View, select the Software that you want to
   consolidate and click on **Consolidate**.

.. _amf-138:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-138.png
    :align: center
    :alt: figure 138

3. The Consolidate Software dialog box opens, where you make the
   consolidation:

    .. _amf-139:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-139.png
        :align: center
        :alt: figure 139

    a. Section-A shows the Primary Asset. By default, the first selection is
       selected as Primary.

    b. Section-B shows the Secondary Assets. You can remove a Secondary
       Asset by clicking on the adjacent X Icon.

    c. You can interchange Primary and Secondary Assets using the S and P
       Icons. For example, you can make the Primary Asset as Secondary by
       clicking the S Icon next to the Primary Asset. In this case, the
       first item in the Secondary List is promoted to the Primary list.

    d. Section-C houses the search bar that lets you search Software Assets
       in the CMDB. The search bar supports the Advanced Search (similar to
       the one in :doc:`List View<asset-list-view>`) feature. You can use the
       search box to find specific Assets by using keywords and predefined
       search options.

    e. Section-D is the display pane that shows all the Software Assets or
       the Software Assets resulting from a search query. You can select
       multiple Assets from here and add them to the Secondary List.

    .. _amf-140:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-140.png
        :align: center
        :alt: figure 140

   Once you decide on the Primary and Secondary Assets, click on
   **Consolidate** to make the Consolidation.

After the Consolidation, the Secondary Software Assets are visible only
in the **Consolidated Software** tab of the Primary Asset.

Unconsolidated Secondary Software Assets
========================================

-  Go to the Details View of a Primary Software.

-  Scroll down to the **Consolidated Software** tab. Here you see all
   the Secondary Assets.

-  Click on **Unconsolidate** adjacent to a Secondary Software. On
   confirmation, the Asset is unconsolidated and it goes back to the
   CMDB.