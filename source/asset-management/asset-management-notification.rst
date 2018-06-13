*********************************
Notifications in Asset Management
*********************************

Marking for Notification
========================

Marking Software Assets
-----------------------

Flotomate allows you to mark certain Software Assets for notification.
Whenever new instance of a marked Software Asset is found during a
discovery, a notification is sent to subscribers.

For this notification to work, you have to add people as subscribers.
Learn how to add `subscribers <#managing-subscribers>`__.

.. _amf-45:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-45.png
    :align: center
    :alt: figure 45

**From List View:**

-  Go to the `List View <#asset-list-view>`__ of class Software IT
   Assets.

-  Select one or more Software Assets. **Mark for Notification** button
   appears above the pane.

.. _amf-46:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-46.png
    :align: center
    :alt: figure 46

-  Clicking on the button marks the selected Software Assets.

**From Details View:**

-  Go to the `Details View <#classifying-assets>`__ of a Software Asset.

-  Click on the Action Menu situated in the top right corner beside
   barcode/Add Barcode.

.. _amf-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-47.png
    :align: center
    :alt: figure 47

-  Clicking on **Mark for Notification** from the pop-up menu marks the
   Asset.

Marking Other Assets
--------------------

Certain product notifications require Asset Groups and Technicians
(Subscribers). The Asset Groups determine which Assets to mark for
notification, and Technicians are the people who receive the
notification.

You can mark Non-Software Assets for notifications by adding them in to
an Asset Group and mentioning the Group when adding
`subscribers <#managing-subscribers>`__ to an Email Notification.

Different Types of Notifications
================================

Flotomate gives you thirteen predefined notifications related to Asset
Management. By default all of them are turned on. You need admin rights
to configure them and change the content of each notification. To view 
all available notifications:

1. Go to **Admin** (A Navigation tab) >> **Email Notifications**
   (Automation)

2. In the Email Notification page, click on **Asset** from the filter
   section.

.. _amf-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-48.png
    :align: center
    :alt: figure 48

.. _amf-49:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-49.png
    :align: center
    :alt: figure 49

3. Here you can view all the notifications and configure them.

+-----------------------------------+-----------------------------------+
| **Notify Admin upon Non-Licensed  | Upon turning this notification    |
| Installation Found**              | on, if a Licensed Software is     |
|                                   | found on an unallocated machine   |
|                                   | then the people and groups        |
|                                   | mentioned in the License’s        |
|                                   | compliance settings get a         |
|                                   | notification.                     |
|                                   |                                   |
|                                   | All License Types, except Free    |
|                                   | License, have a Compliance        |
|                                   | Settings dialog box with options  |
|                                   | to add Requester Groups and       |
|                                   | Emails. Learn how to access       |
|                                   | `Compliance                       |
|                                   | Settings <#compliance-settings>`_ |
|                                   | _.                                |
+-----------------------------------+-----------------------------------+
| **Notify Admin upon Unauthorized  | If Software with a Node Lock      |
| Host Detected**                   | License is found in an            |
|                                   | unallocated host, then a          |
|                                   | notification is sent to people    |
|                                   | mentioned in the License’s        |
|                                   | Compliance Settings.              |
+-----------------------------------+-----------------------------------+
| **Notify Admin upon Software      | If the installation of a Licensed |
| Installation Exceed**             | Software exceeds the Purchase     |
|                                   | Count, then a notification is     |
|                                   | sent to people mentioned in the   |
|                                   | License’s Compliance Settings.    |
+-----------------------------------+-----------------------------------+
| **Licence Expired Notification**  | When a License expires, a         |
|                                   | notification is sent to people    |
|                                   | mentioned in the License’s        |
|                                   | Compliance Settings.              |
+-----------------------------------+-----------------------------------+
| **Licence about to expire         | When a License is about to        |
| notification**                    | expire, a notification is sent,   |
|                                   | 15 days prior, to people          |
|                                   | mentioned in the License’s        |
|                                   | Compliance Settings.              |
+-----------------------------------+-----------------------------------+
| **Licence Under-Utilization       | When                              |
| notification**                    | `utilization <#utilization>`__ of |
|                                   | a Licensed Software comes below   |
|                                   | the `underutilization             |
|                                   | threshold <#_Understanding_Compli |
|                                   | ance_Settings>`__,                |
|                                   | then a notification is sent to    |
|                                   | people mentioned in the License’s |
|                                   | Compliance Settings.              |
+-----------------------------------+-----------------------------------+
| **Licence Over-Utilization        | When                              |
| notification**                    | `utilization <#utilization>`__ of |
|                                   | a Licensed Software exceeds the   |
|                                   | `overutilization                  |
|                                   | threshold <#_Understanding_Compli |
|                                   | ance_Settings>`__,                |
|                                   | then a notification is sent to    |
|                                   | people mentioned in the License’s |
|                                   | Compliance Settings.              |
+-----------------------------------+-----------------------------------+
| **Notify User upon Prohibited     | When a Prohibited Software is     |
| Software Installation**           | detected in an Asset, then the    |
|                                   | user of the Asset gets a          |
|                                   | notification from the system.     |
|                                   |                                   |
|                                   | Every Asset in the CMDB has the   |
|                                   | used-by detail which is used      |
|                                   | here.                             |
+-----------------------------------+-----------------------------------+
| **Notify Admin upon Prohibited    | When a Prohibited Software is     |
| Software Installation**           | detected in an Asset, then users  |
|                                   | mentioned in the Prohibited       |
|                                   | Software Expressions dialog box   |
|                                   | get a notification.               |
+-----------------------------------+-----------------------------------+
| **Notify Subscriber When Software | When an instance of a marked      |
| Installation Found.**             | Software is found during a        |
|                                   | discovery then a notification is  |
|                                   | sent to the                       |
|                                   | `subscribers <#managing-subscribe |
|                                   | rs>`__.                           |
+-----------------------------------+-----------------------------------+
| **Notify Subscriber When Hardware | A notification can be set for     |
| Change Detects**                  | Hardware Assets in an Asset       |
|                                   | Group. Whenever any change is     |
|                                   | detected during discovery a       |
|                                   | notification is sent to           |
|                                   | `subscribers <#managing-subscribe |
|                                   | rs>`__.                           |
+-----------------------------------+-----------------------------------+
| **Notify Subscriber When Warranty | A notification can be set for     |
| Expired**                         | Hardware Assets in a particular   |
|                                   | Asset Group. Whenever warranty of |
|                                   | a Hardware Asset (in the group)   |
|                                   | expires then a notification is    |
|                                   | sent to                           |
|                                   | `subscribers <#managing-subscribe |
|                                   | rs>`__.                           |
+-----------------------------------+-----------------------------------+
| **Notify Subscriber When Warranty | A notification can be set for     |
| is About to Expire**              | Hardware Assets in a particular   |
|                                   | Asset Group. Whenever warranty of |
|                                   | a Hardware Asset (in the group)   |
|                                   | is about to expire in 30 days     |
|                                   | then a notification is sent to    |
|                                   | `subscribers <#managing-subscribe |
|                                   | rs>`__.                           |
+-----------------------------------+-----------------------------------+

Editing Notification Content
----------------------------

You can modify the content of each type of
`notifications <#_Different_Types_of>`__ for Asset Management.

-  In the Email Notifications page (**Admin** >> **Email
   Notification**), click on a notification that you want to edit.
   content. An editor opens.

    .. _amf-50:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-50.png
        :align: center
        :alt: figure 50

    a. You can give your notification a subject with placeholders.
       Placeholders are words that are replaced with specific data by the
       system before sending the notification.

       In section-A & B (:numref:`amf-50`), you get a plethora of placeholders to
       choose.

    .. _amf-51:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-51.png
        :align: center
        :alt: figure 51

    b. You can create impressive content with placeholders from section-B.
       Place your cursor where you want to insert and choose a placeholder
       from the Placeholders dialog box.

    c. The editor provides you toolbars to format your content the way you
       want.

   Hit **Update** to save your content.

-  You can toggle notification on/off from the Email Notifications page
   and the editor mentioned above.

Managing Subscribers
====================

There are notifications that require you to add subscribers who receive
the notifications.

Adding Subscribers:

-  Go to the `Emails Notifications <#_Different_Types_of>`__ (**Admin**
   >> **Email Notifications**) page.

-  Click on a notification that supports adding subscribers; click and
   open **Manage Subscribers** dialog box.

-  There you can add subscribers in the following ways depending on the
   notification:

    a. **Add only Technicians**: Certain notifications just require you
       to add Technicians from the Technician List.

        .. _amf-52:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-52.png
            :align: center
            :alt: figure 52

    b. **Add Asset Group and Technicians**: Certain notifications require
       you to mark Assets by mentioning an Asset Group and Technicians as
       subscribers. These notifications are related to:

        i. Hardware Change

        ii. Warranty Expired

        iii. Warranty is about to expire

        .. _amf-53:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-53.png
            :align: center
            :alt: figure 53

      The Asset Group determines which Assets to mark for notification.