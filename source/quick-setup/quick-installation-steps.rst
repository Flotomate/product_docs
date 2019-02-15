*********************************
Product Installation Quick Guides
*********************************

Our ITSM tool is a standalone service that runs on a ubuntu (16.04 and above) server with the following minimum configuration:

- 4GB System RAM.
- Two Core Processor.
- 100GB of Hard Drive Space.

Once installed, it is accessed from a web browser using the server IP or an associated domain name. 

Downloading ITSM Build (Guide 1)
================================

Once you are done setting up the server/servers, cd into a empty directory and run the following command 
to install the latest product build.

.. code-block:: sudo wget https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/main/linux/service_desk_master_CI

Installation of ITSM as a Standalone Server (Guide 2)
=====================================================

Once downloaded, follow the installation steps in :ref:`Fresh Installation Guide`.

When everything is done, the product will be accessible from a browser after 5 minutes. 

Installation of ITSM using High Availability Feature (Guide 3)
==============================================================

You can opt for the High Availability option which will allow you to maintain service even when the main server is down.
This installation process is different from standalone installation method in guide 2. 

In HA setup you would require two ubuntu server instances. 

Learn :ref:`What is High Availability Setup?`.

Follow the installation steps in :ref:`the HA guide <Setting up High Availability Servers>`. 

Installation of Relay Servers (Guide 4)
=======================================

Once you are done with the ITSM setup, you can connect remote locations/offices using a relay server. 
A relay server is a separate server that you have to setup and link it with the main server (ITSM).

Follow the installation steps in the :ref:`File Server Installation Guide`.

Installation of File Server (Guide 5)
=====================================

Patch and Package management is disabled by default. To enable this feature, you have to setup a file server, and link it with the main 
server. A file server stores all patches and packages before deployment. 

Follow the installation steps in the :ref:`File Server Installation Guide`.

Agent Installation for Asset and Patch/Package Management (Guide 6)
===================================================================

Agent is an application that you install in a workstation. Agent is required for the following operations:

- Asset discovery.
- Software metering.
- Patch and package management.
- Remote desktop access. 

Follow the installation steps in:

- :ref:`Windows Agent Installation Guide`
- :ref:`Ubuntu Linux Agent Installation/Uninstallation Guide`
- :ref:`Mac-OS Agent Installation Guide`

Agent Self-Upgrade Feature (Guide 7)
====================================

Agent Monitor is a separate application that you install along with the Agent. Its sole function is to remotely upgrade the Agent 
application. 

Currently, remote monitor is available for Windows only. Follow the installation steps in :ref:`Windows Agent Monitor Installation Guide`.

You can remotely deploy remote-monitor application across a network using the package management module. :ref:`Learn more <Deploy Agent Monitoring as a Package (Step 1)>`.

Remote Desktop Feature (Guide 8)
================================

The RDP feature allows remote access of a workstation. 

The RDP agent is a separate application, and it's available for Windows and Ubuntu. RDP agent has to be installed along side the agent
application in a workstation. 

You can install and setup the RDP agent from the following guides:

- :ref:`Windows RDP Agent Installation Guide` 
- :ref:`Ubuntu RDP Agent Installation Guide`

Once the agents are setup, you have to configure the main server. For this, you have to install
the RDP middleware in the main server. :ref:`Learn more <Flotomate RDP Middleware Installation Guide>`. 

Running Plugins in Flotomate (Guide 9)
======================================

You can add more features into the tool using plugins. Plugins are small piece of code that interact with the main server.
In order to run plugins in Flotomate, you have to setup a plugin server and connect that with the main server. 

Learn how to setup a plugin server from:

- :ref:`Plugin Server Setup Guide`