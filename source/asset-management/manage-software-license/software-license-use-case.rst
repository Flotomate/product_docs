*************************
Software License Use Case
*************************

**Scenario**: Acme Inc has bought 3D MAX photo editing software with a Multiple Machines License for five workstations. Software has been installed
and are in use. Now a Technician has to create a License for the Software so as to manage compliance (with respect to not using it in more
than five workstations). 

**Actors**: Technician and Administrator.

**Actions**: 

- A Technician creates a Multiple Machines License for 3D MAX (:ref:`Learn More <Adding a License>`).

.. _amf-sl-us-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-SL-US-1.png
    :align: center
    :alt: figure 1

- The Technician updates the :ref:`License Details <Updating License Details>` and sets the :ref:`Purchase Count` (which is five workstations). 

.. _amf-sl-us-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-SL-US-2.png
    :align: center
    :alt: figure 2

- The 3D Max is already in use. The Technician updates the CMDB (Asset Management) using :ref:`Polling <Run on Demand Polling>`.

.. _amf-sl-us-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-SL-US-3.png
    :align: center
    :alt: figure 3

- Technician then links the Software Asset (3D Max) with the Software License; this enables Compliance Management for the
  Software 3D MAX (:ref:`Learn More <Associating a Software License with a Software Asset>`). 

.. _amf-sl-us-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-SL-US-4.png
    :align: center
    :alt: figure 4

- Now the Technician goes to the License details page and :doc:`allocates five workstations <allocating-assets-users>` that are suppose to use the Software. 
  This helps the system to generates notifications when an unauthorized machine installs the software.

.. _amf-sl-us-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-SL-US-5.png
    :align: center
    :alt: figure 5

- In the License details page, the Technician opens the :ref:`Compliance Settings <Compliance Settings>` dialog box and sets 
  over and under utilization thresholds. This settings enables utilization based notifications.

.. _amf-sl-us-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-SL-US-6.png
    :align: center
    :alt: figure 6

- An admin sets the content and subscribers of other notifications related to Software License from
  **Admin** >>  **Email Notifications** >> Asset. Learn about :ref:`Different Types of Notifications`.            

