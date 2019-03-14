********************************
Windows Agent Installation Guide
********************************

Describes Installation Steps for Flotomate Windows Agent.

System Requirement :
====================

**Target Machine OS**: 

- Windows 7 and above versions.

**OS Architecture**: 

- Windows (32 & 64 bit).

**Installation Links**

Windows(32bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x86/agent-32.msi>`_

Windows(64bit): `Click Here <https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/windows/x64/agent.msi>`_

.. important:: Requires sufficient space in Windows Temp file for the application to work.

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

.. note:: Must have system admin credential of computers for agent deployment. 

.. note:: All computers have to be in the same network and domain (if present).

1. Download PSTools.zip. Extract the zip file to a folder in one of the system.

2. Download the agent.msi file.

3. Put agent.msi in the PSTools folder.

4. Add IP list and system credential.

   .. code-block:: PsExec.exe \\host/ip -u domain/administrator -p password -c -d agent.msi /qn

5. Install agent using the following command.

   .. code-block:: PsExec.exe \\host/ip -u domain/administrator -p password cmd /c "msiexec.exe /I "C:\Windows\agent.msi" URL=itsm-url SECURE_PROP=code /quiet /norestart"

It will take time for installing agent in all Computers.