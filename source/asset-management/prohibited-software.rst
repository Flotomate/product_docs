*******************
Prohibited Software
*******************

In an organization, there could be restrictions on the kind of Software
that can be used. For example, torrent clients are prohibited at most
workplaces.

Motadata has a default Software Type called Prohibited, which can be
used to flag certain Software Assets in the CMDB. The process of
flagging can be done both manually and through automation.

Flagging a Software as Prohibited has the following behavior:

- When a prohibited Software is discovered during discovery, a notification is sent to the user of the Installed Asset (Used by)
  and the Admins. Learn more about :ref:`notifications <different types of notifications>`.

- A prohibited Software shows in the **All Prohibited Software** filter.     

Manually Flagging a Software Asset as Prohibited
================================================

Flagging from the Asset List View
---------------------------------

-  Go to the :ref:`Asset List View <Asset List View>` and select **All Software IT Assets**.

-  Select one or more Software from the list area. The **Mark as** button appears above the pane.

.. _amf-141:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-141.png
    :align: center
    :alt: figure 141

-  Click on **Mark as Prohibited Software**. The selected Software Assets are marked as
   Prohibited.

Flagging from the Software Details View
---------------------------------------

.. note:: Using this method you can flag Software Assets one at a time.

-  Go to the :ref:`Details View <Manage Asset Details>` of a Software Asset.

-  There expand the **More Details** section.

.. _amf-142:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-142.png
    :align: center
    :alt: figure 142

-  In the expanded section, change Software Type to **Prohibited**; this flags the Software as Prohibited.

Every time an Asset is marked as Prohibited, the **Prohibited Software**
counter gets updated.

.. _amf-143:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-143.png
    :align: center
    :alt: figure 143

Flagging from Asset List View
-----------------------------

.. note:: Using this method you can flag multiple Software.

- Go to the :ref:`List View <asset list view>` and select **All Software IT Assets**.

- Apply filter **All Prohibited Software**. 

.. _amf-143.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-143.1.png
    :align: center
    :alt: figure 143.1

- All Prohibited Software are filtered. Click on **Add Prohibited Software**. 

.. _amf-143.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-143.2.png
    :align: center
    :alt: figure 143.2

- In the new dialog box, you can search and select multiple Software, and mark them as prohibited. Learn how to use the :ref:`search bar <am-using-search-bar>`. 

.. _amf-143.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-143.3.png
    :align: center
    :alt: figure 143.3

Flagging Using Software Normalization
-------------------------------------

.. note:: Following methods require Admin rights.

A user can mark multiple Software as prohibited by creating a Normalization rule. A Normalization rule, when run, will flag
all Software satisfying the rule conditions. Learn :ref:`how to create a Normalization rule <Setting Software Normalization>`.

A user can also prohibit Software using :ref:`Software Installation Control Settings`.

Managing Prohibited Software Expressions
========================================

In Motadata, you can automate the process of flagging (Prohibit) Software Assets.
The feature works during discovery and for Software already
included in the CMDB.

The process runs a regex expression against the names of the Software
Assets. Assets with matched characters are flagged as Prohibited. Users
provide the regex expressions.

**To Provide an Expression:**

1. Go to the :doc:`Asset List View <asset-list-view>` and select **All Software IT Assets**.

2. Apply the filter **All Prohibited Software**. 

.. _amf-143.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-143.1.png
    :align: center
    :alt: figure 143.1

3. Click on **Manage Prohibited Software Expression**. The Prohibited
   Software Expressions dialog box opens.

.. _amf-144:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-144.png
    :align: center
    :alt: figure 144

4. The Prohibited Software Expressions dialog box has the following
   fields:

    .. _amf-145:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-145.png
        :align: center
        :alt: figure 145

    a. In section-A, you add emails of people who want a notification
       every time a Prohibited Software Asset is discovered. The
       :ref:`notification <managing software licenses>` for Admin is sent
       to the mentioned email address/addresses.

    b. In section-B, you add your expression. You can add multiple
       expressions and can view them in section-D. Type in your
       expression and click on **Add Pattern**.

    c. In section-C, selecting this option scans all Software Assets
       that are already in the CMDB for expression matching. If you
       don’t select this option then the system performs a scan in the
       next discovery.

    d. In section-D, you can view all the expressions already added.
       Prohibition of a Software happens when any one of the given
       expressions is matched against its name. You can delete any
       expression using the Delete Icon.

5. Click on **Done** to save your changes. Scanning process starts
   immediately if you have checked the box.

Computer Exclusion
==================

You can ignore Prohibited Software in certain Hardware Assets. Computer
Exclusion lets you add Assets that you want to ignore for Prohibited
Software.

- Go to the :doc:`Asset List View <asset-list-view>` and select **All Software IT Assets**.

- Apply the filter **All Prohibited Software**. 

.. _amf-143.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-143.1.png
    :align: center
    :alt: figure 143.1

- Click on **Computer Exclusion** button.

.. _amf-146:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-146.png
    :align: center
    :alt: figure 146

- *Add Global Exclusion* dialog box opens. There you can search for
  Assets (it supports :ref:`Advanced Search <am-using-search-bar>`). Select
  the Assets that you want to ignore and add them for exclusion.

.. _amf-147:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-147.png
    :align: center
    :alt: figure 147
