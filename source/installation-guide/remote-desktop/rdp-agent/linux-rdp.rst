***********************************
Ubuntu RDP Agent Installation Guide
***********************************

Describes Installation Steps for Ubuntu RDP Agent 3.0.0.

Minimum System Requirement:
===========================

**Target Machine OS:**

-  Ubuntu 16 and above for Ubuntu Linux Agent.

**Hardware Requirement:**

-  1GB System RAM

-  Two-Core Processor

-  Space: 250 MB Hard Drive

Downloading RDP Agent
=====================

You can download the RDP Agent (Ubuntu Linux) from the below link:

**Ubuntu Linux 64-bit**: `Download Link <https://flotomate-customer-releases.s3.ap-south-1.amazonaws.com/latest/rdp+server/linux/agent_rdp>`_

RDP Installation Setup:
==========================

After downloading the RDP Agent file, follow the below steps to install the
Agent on to a Computer:

1. Open terminal.

2. Go to the directory where you have downloaded the agent_rdp.

3. Check the permission of the file whether it is executable. If not run
   the following command.

   **sudo chmod 777 agent_rdp**

.. _rdp-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/RDP-3.png
    :align: center
    :alt: figure 3

4. Run the agent_rdp file (**don’t use sudo to run the file**).

   **./agent_rdp**

5. Wait for the installation to finish.