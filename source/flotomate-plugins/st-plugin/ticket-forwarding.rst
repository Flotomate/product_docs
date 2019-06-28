************************************
ITSM Plugin - Ticket SMS Integration
************************************

This is a standard plugin offered by Motadata to all our users.

**Purpose**: The plugin can forward a ticket to a third party server.

**Perquisite**: Plugin server needs to be setup with the main server (:ref:`Learn More <Plugin Server Setup Guide>`). 

**Plugin Setup**

1. Download the plugin .fp file and transfer it to the plugin server (:ref:`Learn More <plugin-transfer>`).

2. Restart the plugin server.

3. Register the plugin in the ITSM tool (:ref:`Learn more <Register a Plugin>`) from **Admin** >> **Plugins** >> **Register New Plugin**. 

.. _plgm-11:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-11.png
    :align: center
    :alt: figure 11

While registering the plugin, the admin has to provide the following inputs:

- **Server URl**

- **Server Header Value**: Depends on the server/application where you want to send the ticket. Primarily would contain 
  a token to authenticate the  request. 

.. _plgm-12:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-12.png
    :align: center
    :alt: figure 12

**Triggering the Plugin**

The ticket forwarding plugin is triggered from a Workflow. Learn more about :ref:`Workflow <ad-workflow>`.

In the below example, a ticket is forwarded when it is created in the tool. The following parameters are forwarded.

- **Incident ID**: Ticket id 
- **Incident Name**: Ticket subject.
- **Incident Description**: Ticket Description. 
- **Contact Number**: Phone number of the requester. Admin has to create a custom field to capture this info, :ref:`learn more <ad-custom-field>`.
- **Contact Person**: Name of the requester. 
- **Location**: Assigned location of the ticket. 

.. note:: In the below figure, placeholders have been used to capture the necessary data whenever a new ticket is created. 

.. _plgm-13:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-13.png
    :align: center
    :alt: figure 13