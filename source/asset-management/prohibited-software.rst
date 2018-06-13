*******************
Prohibited Software
*******************

In an organization, there could be restrictions on the kind of Software
that can be used. For example, torrent clients are prohibited at most
workplaces.

Flotomate has a default Software Type called Prohibited, which can be
used to flag certain Software Assets in the CMDB. The process of
flagging can be done both manually and through automation.

We have `notifications <#different-types-of-notifications>`__ that
notify people about the discovery of Prohibited Assets. The notification
can go to the users (Used By) of the Assets and the Administrators.

Manually Flagging a Software Asset as Prohibited
================================================

**Flagging from the Asset List View**:

-  Go to the `Asset List View <#asset-list-view>`__ of the class
   Software IT Asset.

-  Select one or more Software from the list area. The **Mark as
   Prohibited** button appears above the pane.

.. _amf-141:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-141.png
    :align: center
    :alt: figure 141

-  Click on **Mark as Prohibited**. Your selected Assets are marked as
   Prohibited.

**Flagging from the Software Details View:**

.. note:: Using this method you can flag Software Assets one at a time.

-  Go to the `Details View <#classifying-assets>`__ of a Software Asset.

-  There expand the **More Details** section.

.. _amf-142:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-142.png
    :align: center
    :alt: figure 142

-  In the expanded section, changing Software Type to **Prohibited**
   flags the Software as Prohibited.

Every time an Asset is marked as Prohibited, the **Prohibited Software**
counter gets updated.

.. _amf-143:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-143.png
    :align: center
    :alt: figure 143

Managing Prohibited Software Expressions
========================================

In Flotomate, you can automate the process of flagging Software Assets.
The feature works during discovery and for Software Assets already
included in the CMDB.

The process runs a regex expression against the names of the Software
Assets. Assets with matched characters are flagged as Prohibited. Users
provide the regex expressions.

**To Provide an Expression:**

1. Go to the `Asset List View <#asset-list-view>`__ of the class
   Software IT Assets.

2. Select one or more Software from the list area. **Manage Prohibited
   Software Expressions** button appear above the pane.

.. _amf-144:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-144.png
    :align: center
    :alt: figure 144

3. Click on **Manage Prohibited Software Expression**. The Prohibited
   Software Expressions dialog box opens.

.. _amf-145:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-145.png
    :align: center
    :alt: figure 145

4. The Prohibited Software Expressions dialog box has the following
   fields:

    .. note:: Refer to :numref:`amf-145`.

    a. In section-A, you add emails of people who want a notification
       every time a Prohibited Software Asset is discovered. The
       `notification <#managing-software-licenses>`__ for Admin is sent
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

-  Go to the `List View <#asset-list-view>`__ of class Software Assets.

-  Click on Computer Exclusion above view pane.

.. _amf-146:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-146.png
    :align: center
    :alt: figure 146

-  Add Global Exclusion dialog box opens. There you can search for
   Assets (it supports `Advanced Search <#using-search-bar>`__). Select
   the Assets that you want to ignore and add them for exclusion.

.. _amf-147:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-147.png
    :align: center
    :alt: figure 147
