*******************************
Mac-OS Agent Installation Guide
*******************************

Describes Installation Steps for Flotomate MacOS Agent-2.7.0

System Requirement :
====================

**Target Machine OS**: 

- macOS High Sierra 14 above

**Installation Links**

Mac OS (64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/mac/x64/agent>`_

Installation in Mac OS
======================

1. Download the latest Mac agent file from the given link.

2. Open terminal and change directory to where the agent file is downloaded.

3. Check the permissions of the Mac Agent file whether it is executable. If not run the following command.

   **sudo chmod 777 agent**

.. _aig-9:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-9.png
    :align: center
    :alt: figure 9

4. Now run the Mac agent file using the following command:

   **sudo ./agent**

.. _aig-10:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-10.png
    :align: center
    :alt: figure 10

5. The installation process will begin, and it will ask for the URL of the main server. 

   .. note:: You can get the activation code from Flotomate ITSM tool in **Admin** >> **Account** 
             (under Organization).

.. _aig-11:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-11.png
    :align: center
    :alt: figure 11

6. The installation process will complete after providing the URL.

Uninstall Mac Agent 
-------------------

Open Terminal and follow the below mentioned commands:

- Stop Agent Service:

  **sudo launchctl unload /Library/LaunchDaemons/com.flotomate.agent.plist**

- Remove Agent Service:

  **Sudo rm /Library/LaunchDaemons/com.flotomate.agent.plist**

- Delete Agent dir:

  **Sudo rm -rf /opt/it-service-desk**