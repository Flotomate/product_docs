*******************
Agent Upgrade Guide
*******************

Upgrading Agent application allows for the following benefits:

- Addition of new features.

- Bug fixes.

- Security Patches to resolve vulnerability.

The below mention steps are applicable for existing customers having the following setup:

- Main server version : 2.5.0 

- Agent version : 2.3.0

- New Agent version : 2.5.0

- New Agent Monitor version : 1.0.0

**Prerequisite (Things to have before beginning the Upgrade process)**

- Complete File Server setup (:ref:`Learn more <File Server Installation Guide>`)

- Download Latest Agent Monitor executable file.

- Download Latest Agent application executable file.

- Download Latest product build if available.

**Steps for upgrading Agent application:**

1. Deploy Agent Monitoring as a Package in all computers using the the old Agent application; this enables the Agent Self Upgrade 
   feature in the main server. 

2. Upgrade main server (If a new build is available); this is done to avoid incompatibility issues between new Agent and old main server.

3. Using the Agent Self Upgrade feature, we will upgrade all the Agents. 

Deploy Agent Monitoring as a Package (Step 1)
=============================================

We are going to create a Deployment Request for Agent Monitor.

- Login to the Main Server (Technician Portal).

- Go to **Launcher** >> **Deployment**.

.. _aup-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-1.png
    :align: center
    :alt: figure 1

- Click on **Add Software Package**.

- Complete the fields on the Add page. View below images for reference.

.. _aup-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-2.png
    :align: center
    :alt: figure 2

.. note:: Related topic: :ref:`Adding a Software Package`. 

- Now you have added the Monitor as a Package. Select the new Package and click on **Deploy**.

.. _aup-5:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-5.png
    :align: center
    :alt: figure 5

.. note:: You would require a Deployment Policy. Learn how to create a :doc:`Deployment Policy <sp-setting-up-a-deployment-policy>`. 

- We will publish our Deployment Request of our Package. Select all computers where you want to deploy. View below image for reference.

.. note:: While selecting the package, make sure to set the **User** as **Current User**.
..note:: Related topic: :ref:`adding-a-package-deployment-request`.

.. _aup-6:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-6.png
    :align: center
    :alt: figure 6

This step is complete when the deploy status is success.

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

- Select the computers that you want to update and click **Upgrade**. The Upgrade process will start on confirmation.















