********************************
Windows Agent Installation Guide
********************************

Describes Installation Steps for Flotomate Windows Agent -2.7.0.

System Requirement :
====================

**Target Machine OS**: 

- Windows 7 and above.

**OS Architecture**: 

- Windows (32 & 64 bit).

**Installation Links**

Windows(32bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x86/agent_32bit.msi>`_

Windows(64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x64/agent.msi>`_

Installation in Windows
=======================

Note: :ref:`.Net-Framework required <question1>` 

1. Download the latest msi file from the given link.

2. Run the msi file.

3. Follow the wizards as below mentioned screenshots:

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
   If there's no Port, then leave it blank. You can get the activation code from Flotomate ITSM tool in **Admin** >> **Account** 
   (under Organization).

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