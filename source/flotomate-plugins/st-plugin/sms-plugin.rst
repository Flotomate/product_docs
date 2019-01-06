**********************************
ITSM Plugin - Text SMS Integration
**********************************

This is a standard plugin offered by Flotomate to all our users.

**Purpose**: The plugin can send an SMS using a third party API with the required authentication. 

**Perquisite**: Plugin server needs to be setup with the main server (:ref:`Learn More <Plugin Server Setup Guide>`). 

**Plugin Setup**

1. Download the plugin .fp file and transfer it to the plugin server (:ref:`Learn More <plugin-transfer>`).

2. Restart the plugin server.

3. Register the plugin in the ITSM tool (:ref:`Learn more <Register a Plugin>`).

.. _plgm-9:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-9.png
    :align: center
    :alt: figure 9.

**Triggering SMS**

The SMS plugin is triggered from a Workflow. Learn more about :ref:`Workflow <ad-workflow>`. 

Below we have created a workflow that sends an sms to the requester when he/she creates a ticket. 

A request can have custom fields to capture requester information. In the following example, a request
has the custom field {#Phone#}, which captures the phone number. Learn how to create :ref:`custom fields <ad-custom-fields>`.

The authentication for the API has been passed in the **others** field using *key* and *psw*. The same parameters have been entered in the 
above field: **api**.

.. _plgm-10:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-10.png
    :align: center
    :alt: figure 10