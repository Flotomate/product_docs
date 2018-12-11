*************************
Flotomate Discovery Agent 
*************************

Not all workstations in an organization are part of a network, but
still, they need discovery. By using our Agent Application, Flotomate
can fetch data from such workstations remotely.

Flotomate’s Agent Application is a lightweight application that runs in
the background of a workstation, acquires data, and pushes it directly
to the main server.

Minimum System Requirements
===========================

The following table highlights the hardware and software requirements
for a system to run the Agent Application.

+----------------------+----------------------+
| **Processor Type**   | Intel Dual Core      |
+======================+======================+
| **Processor Speed**  | 2.6 GHz              |
+----------------------+----------------------+
| **RAM**              | 1 GB                 |
+----------------------+----------------------+
| **Free Hard Disk**   | 100 MB               |
+----------------------+----------------------+
| **Operating System** | Windows 7 and higher/|
|                      | Ubuntu 16 and higher |
+----------------------+----------------------+

Installing the Discovery Agent Application
==========================================

Installing in Windows:
----------------------

Installing the Agent on a Windows machine can be done in three ways:

**Using the Application Installer:**

1. Download the Agent Application installer on the workstation.

2. Go to the directory where the agent.msi file is situated.

3. Run agent.msi as Administrator.

.. _amf-189:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-189.png
    :align: center
    :alt: figure 189

4. The installation wizard opens. Click Next and set destination path.

.. _amf-190:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-190.png
    :align: center
    :alt: figure 190

5. In the URL field, enter the URL of Service Desk’s main server and
   click **Next**.

   .. note:: http or https in URL is a must.

.. _amf-191:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-191.png
    :align: center
    :alt: figure 191

6. In the next dialog box, click Install to complete your
   installation.

**Using the Application Installer (Non-Interactive):**

1. You can also install the Agent Application from the Command Prompt
   without the hassle of seeing multiple dialog boxes.

2. Open CMD and change the target path to agent.msi.

3. Type agent.msi and the URL of the main server, and hit enter. Your
   installation is done.

.. _amf-192:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-192.png
    :align: center
    :alt: figure 192

**Using PsExec for installation:**

PsExec lets you run processes remotely on other systems without the need
of a client and with full access to console applications. Using PsExec,
you can launch and execute CMD commands remotely. PsExec is part of the
PsTools toolkit developed by Sysinternals.

1. Download PSTools.zip from the following link:

   https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/share/PSTools.zip

2. Extract the zip file to a folder.

3. Download the agent.msi file from the following link:

   https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/agent.msi

4. Put agent.msi in the PSTools folder.

5. Add IP list in ip.txt file for installing agent in those computers.

6. Now run setup.bat.

7. Enter the Url of the main server.

8. Enter Domain Username and password then hit enter.

9. It will take time for installing agent in all Computers.

Uninstalling (Windows) the Discovery Agent Application
------------------------------------------------------

1. Go to the directory where agent.msi file is situated.

2. Run the agent.msi file.

3. Given that you have already installed the Agent Application, the
     Agent Setup Wizard leads you to the Modify, Repair, and Remove
     installation dialog box.

.. _amf-193:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-193.png
    :align: center
    :alt: figure 193

4. Select Remove and follow the instructions to remove the Agent
   Application.