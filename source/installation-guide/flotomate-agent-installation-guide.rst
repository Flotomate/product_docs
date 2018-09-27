**********************************
Flotomate Agent Installation Guide
**********************************

Describes Installation Steps for Flotomate Windows & Linux Agent.

System Requirement :
====================

**Target Machine OS**: 

- Windows 7 and above.
- Linux.

**OS Architecture**: 

- Windows (32 & 64 bit).
- Linux (64bit).

.. note:: Currently we have only tested the Linux Agent in Ubuntu 16.04.

**Installation Links**

Windows(32bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x86/Agent.exe>`_

Windows(64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x64/Agent.exe>`_

Linux(64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/linux/x64/agent>`_


Installation in Windows
=======================

1. Download the latest msi file from the given link.

2. Run the msi file.

3. Follow the wizards as below mentioned screenshots

 a. Click Next

    .. _aig-2:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-2.png
        :align: center
        :alt: figure 2

 b. Click next

    .. _aig-3:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-3.png
        :align: center
        :alt: figure 3

4. It will ask for URL and Port. Select a Protocol based on what the URL supports. 
   If there's no Port, then leave it blank. 

.. _aig-4:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-4.png
    :align: center
    :alt: figure 4

5. Click next and finish installation process.

.. _aig-5:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-5.png
    :align: center
    :alt: figure 5

.. _aig-5.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-5.1.png
    :align: center
    :alt: figure 5.1    

Installation in Linux
=====================

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

6. Enter the URL of the product (Flotomate) server.

.. _aig-8:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-8.png
    :align: center
    :alt: figure 8   

Uninstall Linux Agent
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

Installation using PsExec (For Windows)
=======================================

1. Download PSTools.zip. Extract the zip file to a folder.

2. Download the Agent.exe file.

3. Put Agent.exe in the PSTools folder.

4. Add IP list in ip.txt file for installing agent in those computers.

5. Now run setup.bat.

6. Enter the Url of the main server.

7. Enter Domain Username and password then hit enter.

It will take time for installing agent in all Computers.

