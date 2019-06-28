*******************
Agent Upgrade Guide
*******************

Upgrading Agent application allows for the following benefits:

- Addition of new features.

- Bug fixes.

- Security Patches to resolve vulnerability.

The below mentioned steps are applicable for existing customers having the following setup:

- Minimum main server version : 2.7.0 (Learn about :ref:`build upgrade <Motadata Service Desk - Server Upgrade Guide>`)

- Minimum starting Agent version 2.7.1.

**Prerequisite (Things to have before beginning the Upgrade process)**

- Latest Agent Monitor executable file.

- Latest Agent application executable file, which should be an increment over the minimum starting agent version for example 2.7.2.

- Latest product build if available.

**Steps for upgrading Agent application:**

1. Agent Monitor has to be installed manually in all the targets with the agent application. Learn how to :ref:`install the monitor <Windows Agent Monitor Installation Guide>`. 

2. Upgrade main server (If a new build is available); this is done to avoid incompatibility issues between new Agent and old main server.

3. Using the Agent Self Upgrade feature, we will upgrade all the Agents. 

Install Agent Monitoring (Step 1)
=================================

All the Windows machines where the agent-upgrade has to be performed have to have the agent monitor installed. Install the agent monitor in 
each machine following the given guide:

- :ref:`Windows Agent Monitor Installation Guide`.

.. note:: You can use GPO to deploy the agent monitor over a large number of machines in a domain. :ref:`Learn more <Agent & Monitor Bulk Installation Using GPO>`. 

Upgrade Main Server (Step 2)
============================

.. note:: This step is valid if new build is available.

Upgrade the Main Server following steps mentioned in the :ref:`link <server-upgrade>`.

Self Upgrade of Agent (Step 3)
==============================

We are now going to update the old Agent application using the Agent Self Upgrade feature.

- Go to **Admin** >> **All Computers**. 

.. _aup-7:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-7.png
    :align: center
    :alt: figure 7

- Click on **Upload New Agent** and upload the new Agent application file. View below image for reference.

.. _aup-8:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-8.png
    :align: center
    :alt: figure 8

.. important:: When uploading the 32 bit application don't forget to select the 32 bit option, see below.

.. _aup-8.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-8.1.png
    :align: center
    :alt: figure 8.1

- Select the computers that you want to update and click **Upgrade**. The Upgrade process will start on confirmation.