**************************************
Flotomate RDP Agent Installation Guide
**************************************

Describes Installation Steps for Flotomate RDP Agent – 1.0.0

Minimum System Requirement:
===========================

**Target Machine OS:**

-  Windows 7 and above for Windows Agent.

-  Ubuntu 16 and above for Linux Agent.

**Hardware Requirement:**

-  1GB System RAM

-  Dual-Core Processor

-  Space: 250 MB Hard Drive

Downloading RDP Agent
=====================

**Windows 32-bit & 64-bit:**

You can download the RDP Agent (Windows) from the below link:

https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/rdp+server/windows/RDP+Agent.exe

**Linux 64-bit**:

You can download the RDP Agent (Linux) from the below link:

https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/rdp+server/linux/agent_rdp

Manual Installation Setup:
==========================

After downloading the RDP Agent, follow the below steps to install the
Agent on to a Computer:

**Windows Installation**

1. Run the RDP Agent file as Administrator.

.. _rdp-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/RDP-1.png
    :align: center
    :alt: figure 1

2. Click Next to continue the installation wizard.

3. Click **Install** to begin the installation process.

4. Click on **Finish** when installation is done.

.. _rdp-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/RDP-2.png
    :align: center
    :alt: figure 2

**Linux Installation**

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

