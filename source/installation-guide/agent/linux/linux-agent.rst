.. _Ubuntu Linux Agent Installation Guide:

*********************************************
Ubuntu Linux Agent Installation/Uninstallation Guide
*********************************************

Describes Installation Steps for Motadata Ubuntu Linux Agent-3.0.0

System Requirement :
====================

**Target Machine OS**: 

- Ubuntu (64bit).

.. note:: Currently we have only tested the Ubuntu Linux Agent in Ubuntu 16.04.

**Installation Links**

Ubuntu Linux(64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/linux/x64/agent>`_

.. _Installation in Ubuntu Linux:

Installation in Ubuntu
======================

1. Download the latest agent file from the given link.

2. Open terminal and go to the directory where you have downloaded the file.

3. Check the permissions of the file whether it is executable. If not run the following command.

   **sudo chmod 777 agent**

.. _aig-6:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-6.png
    :align: center
    :alt: figure 6

4. Now run the agent file using sudo.

   **sudo ./agent**

.. _aig-7:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-7.png
    :align: center
    :alt: figure 7

5. Enter your system password.

6. Enter the URL of the product (Motadata) server. You can get the activation code from Motadata ITSM tool in **Admin** >> **Account** 
   (under Organization).

.. _aig-8:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-8.png
    :align: center
    :alt: figure 8   

.. _Uninstall Ubuntu Linux Agent:

Uninstall Ubuntu Linux Agent
---------------------

Open Terminal and follow the below mentioned commands:

- Stop Agent Service:

  **sudo systemctl stop  agent_service**

- Disable Agent Service:

  **sudo systemctl disable  agent_service**

- Remove Agent Service:

  **sudo rm /etc/systemd/system/agent_service.service**

- Delete Agent dir:

  **sudo rm -rf /opt/it-service-desk**