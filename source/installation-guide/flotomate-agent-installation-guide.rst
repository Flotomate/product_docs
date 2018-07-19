**************************************
Flotomate Agent Installation Guide
**************************************

Describes Installation Steps for Flotomate Windows Agent – 1.0.0

System Requirement :
====================

**Target Machine OS**: 

- Windows 7 and above.
- Linux.

**OS Architecture**: 

- Windows (32 & 64 bit).
- Linux (64bit).

.. note:: Currently we have tested the Linux Agent in Ubuntu 16 and above.

**Installation Links**

Windows(32bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x86/Agent.exe>`_

Windows(64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x64/Agent.exe>`_

Linux(64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/linux/x64/agent>`_


Installation in Windows
=======================

1. Download the latest agent.exe file from the given link.

2. Run Agent.exe as Administrator.

.. _aig-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-1.png
    :align: center
    :alt: figure 1

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

4. During installation setup, It will ask for URL. Write url of
   service-desk’s main-server with http or https. Note : http or https in
   url is must.

.. _aig-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-4.png
    :align: center
    :alt: figure 4

5. Then next and finish installation process.

.. _aig-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-5.png
    :align: center
    :alt: figure 5

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

