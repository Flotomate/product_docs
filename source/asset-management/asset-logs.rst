**********
Asset Logs
**********

.. _am-viewing-audit-trail:

Viewing Audit Trail
===================

An Audit Trail provides an active log of changes made to an Asset (of details stored locally in the tool) in a
CMDB with timestamp and info about the user responsible for the change.
This is a tracking feature that allows monitoring of Technicians
activities in relation to an Asset.

You can view the Audit Trail in the following ways:

-  **History Tab**: You can view the Audit Trail in the History tab (in
   :doc:`Asset Details View<manage-asset-details>`) of a Hardware, Service,
   Cloud and Other Asset types.

    .. _amf-94:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-94.png
        :align: center
        :alt: figure 94

   You can filter the data using a Start date-time and End date-time. 

-  **Asset List View**: You can access the Audit Trail from the Action
   Menu of an Asset in the :doc:`Asset List View<asset-list-view>`.

.. _amf-95:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-95.png
    :align: center
    :alt: figure 95

-  **Asset Details View**: You can access the Audit Trail from the
   Action Menu of an Asset in the :doc:`Asset Details View<manage-asset-details>`.

.. _amf-96:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-96.png
    :align: center
    :alt: figure 96

Change and Scan Log
===================

Asset types other than Software provide two important logs; you can find
them in the **History** tab on the :doc:`Details View<manage-asset-details>` of an Asset, they are:

-  **Scan Log**: Here you can view the number of times the Asset was
   scanned along with the timestamp and mode of scan.

   The log also shows whether a scan was done by an Agent or through an Agent-less method.

   .. _amf-97:
   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-97.png
       :align: center
       :alt: figure 97
   
   Here, you can filter the data using a Start date-time and End date-time. 

-  **Change Log**: During a Polling process, Assets in the CMDB are
   updated for changes in Software and Hardware. A Change log lists the
   discrepancies between a source (Asset in network) and a destination
   (Asset in CMDB). For example: a new addition of a software to an
   already discovered Asset gets reflected in the Change Log during
   polling.

   You can filter the data by Hardware, Software and Users.

    .. _amf-98:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-98.png
        :align: center
        :alt: figure 98

   Here, you can filter the data using a Start date-time and End date-time.

   You can open the details of a change by clicking on the adjacent
   **View**.

    .. _amf-99:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-99.png
        :align: center
        :alt: figure 99
