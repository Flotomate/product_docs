**************************************
Flotomate Agent Installation Guide
**************************************

Describes Installation Steps for Flotomate Windows Agent – 1.0.0

System Requirement :
====================

**Target Machine OS:** Windows 7 and above.

Manual Installation Setup:
==========================

1. Run Agent.exe as Administrator.

.. _aig-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-1.png
    :align: center
    :alt: figure 1

2. Follow the wizards as below mentioned screenshots

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

3. During installation setup, It will ask for URL. Write url of
   service-desk’s main-server with http or https. Note : http or https in
   url is must.

.. _aig-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-4.png
    :align: center
    :alt: figure 4

4. Then next and finish installation process.

.. _aig-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AIG-5.png
    :align: center
    :alt: figure 5

Installation using PsExec
=========================

1. Download PSTools.zip. Extract the zip file to a folder.

2. Download the Agent.exe file.

3. Put Agent.exe in the PSTools folder.

4. Add IP list in ip.txt file for installing agent in those computers.

5. Now run setup.bat.

6. Enter the Url of the main server.

7. Enter Domain Username and password then hit enter.

It will take time for installing agent in all Computers.

