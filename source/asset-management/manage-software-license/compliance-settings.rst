***************************
Managing License Compliance
***************************

A company is exposed to different kinds of risks when it is not aware of
the proper usage of Software that are being run on its machines. One such risk is
over-utilization of a Licensed Software, and such risks come under the
umbrella term compliance management. Compliance Management tries to enforce the pre-agreed upon
conditions related to the usage of a Software.

Flotomate tracks all the Software that are installed on various Hardware
Assets, and the process helps in compliance management. Currently,
Flotomate supports the generation of notifications upon nine types of
compliance related violations.

There is a separate thread in Flotomate that checks all Licensed
Software and their installation instances against specified parameters;
those parameters are as follows:

-  Utilization

-  Purchase Count

-  Installation Count

-  Expiry Date of the License

-  Hostname (Node-Locked)

-  Software Type

-  Allocated Machines

Out of all the above parameters, Utilization Count, Installation Count, Purchase Count,
Expiry Date and Allocated Machines are License specific parameters.

License Usage Counters (Allocation Count, Installation Count and Purchase Count)
--------------------------------------------------------------------------------

The counters are of :doc:`Allocation<allocating-assets-users>`, Installation and Purchase. The 

.. _amf-136.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-136.2.png
    :align: center
    :alt: figure 136.2

Currently the counters appear in Licencees with the type either Single Machine,
Multiple Machines, or Node Lock. It shows the following data points:

- :doc:`Allocations <allocating-assets-users>`: This shows the number of machines allocated to
  the License. Flotomate allows more Allocation than the Purchase
  Count.

- :ref:`Purchase Count`

- :ref:`Installation Count`

.. _am-utilization:

Utilization Count
-----------------

Utilization refers to the total utilization of the Licensed Software
across all managed IT Assets. The tool denotes it as a percentage
where the numerator is the Installation Count and denominator, Purchase
Count.

Installation Count
------------------

Installation Count is the total number of installation of a Licensed
Software. It does not discriminate between licensed installation and
unlicensed installation.

Purchase Count
--------------

Purchase Count refers to the total allowable installation of a Licensed
Software.

+------------------------+-------------------------------------------+
| License Type           | Purchase Count                            |
+========================+===========================================+
| Single Machine         | Default value set to one                  |
+------------------------+-------------------------------------------+
| Multiple Machines      | Can be set to as many as possible         |
+------------------------+-------------------------------------------+
| Enterprise (Perpetual) | Not applicable                            |
+------------------------+-------------------------------------------+
| Unlimited Machines     | Not applicable                            |
+------------------------+-------------------------------------------+
| OEM                    | Not applicable                            |
+------------------------+-------------------------------------------+
| Single User            | The Count is equal to the number of users |
+------------------------+-------------------------------------------+
| Node Locked            | Default value set to one                  |
+------------------------+-------------------------------------------+
| Volume Users           | The Count is equal to the number of users |
+------------------------+-------------------------------------------+
| Unlimited Users        | Not applicable                            |
+------------------------+-------------------------------------------+
| Free License           | Not applicable                            |
+------------------------+-------------------------------------------+

Adding Purchase Count
^^^^^^^^^^^^^^^^^^^^^^

In certain Licenses, where there's a scope of more than one user/machine usage, a Technician can manually set the
Purchase Count. 

**To set a Purchase Count:**

- Go to the Detains View of a License.

- The Purchase Count field is in the **License Info** section under **Details** tab. Click the edit icon.

- A dialog box opens where you can edit the Purchase Count.

.. _amf-136.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-136.3.png
    :align: center
    :alt: figure 136.3

Compliance Settings
-------------------

Flotomate allows you to set under and over utilization notifications for
Multiple Machines and Volume Users License Types. You have to define the
under-utilization and over-utilization threshold for above mentioned
License Types to enable utilization monitoring.

**Over-utilization**: Talks of an event when utilization(Installation/Purchase Count) exceeds a specified percentage.

**Under-utilization**: Talks of an event when utilization(Installation/Purchase Count) falls below a specified percentage.

For every other License Types, except Free License, you have to add
Requester Groups and Emails to enable compliance violation
notifications.

1. Go to **Asset** (A Navigation Tab) >> **Software Licenses**.

2. Select a License and head to its Details View.

3. On the Details View, click the **Action Menu** and select **Compliance Settings**.

.. _amf-136.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-136.4.png
    :align: center
    :alt: figure 136.4

.. _amf-137:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-137.png
    :align: center
    :alt: figure 137

.. note:: Please refer to :numref:`amf-137`.

-  Section-A allows you to add Requestor Groups that are going to
   receive notifications (group members are the :ref:`admin for the notification <different types of notifications>`).

-  Section-B is where you add emails of individuals who are going to
   receive notifications along with the groups (recipients are the
   :ref:`admin for the notification <different types of notifications>`).

-  In section-C is where you decide the threshold for over-utilization
   and under-utilization in percentage. For example, if Installation
   Count of a Licensed Software is equal to its Purchase Count then
   utilization is 100 percent.

   a. If over-utilization limit is set to 90%, then 91% utilization
      would trigger a notification to the admin.

   b. If under-utilization limit is set to 80% and utilization is 98%,
      then a fall of utilization below 80% would trigger a notification
      to the admin.