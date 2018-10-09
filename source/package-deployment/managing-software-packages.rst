*********************************************
Managing Software Packages/Registry Configurations
*********************************************

The first step towards Deployment is to add Software Packages/Registry Configuration in
the system. A Package/Registry Configuration has to be manually added to the Deployment module before
it can be attached to a Deployment Request.

Whatever Packages/Registry Configurations you add, they all appear on the :doc:`Deployment List View <package-registry-list-view>` 
(either in Windows Packages, Linux Packages or Windows Registry). 
After adding, you can modify a Package/Registry Configuration details and also delete them.

Adding a Software Package
=========================

1. Go to the :doc:`Package List View <package-registry-list-view>` (either Windows or Linux).

2. Click on the **Add Software Package** button situated in the top
   right corner.

3. The Add Software Package page opens. Here you get the following
   fields:

    .. _spf-25:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-25.png
        :align: center
        :alt: figure 25

   a. **Name (Compulsory Field)**: Here you type the name of the Package.
      The best practice is to type the name of the Software.

   b. **Platform (Compulsory Field)**: Select the OS on which the package
      runs. Here you get a predefined list containing Windows and Linux.

   c. **Silent Installation Argument**: :ref:`Learn More <Silent Installation of a Software>`. 

   d. **Package Type (Compulsory Field)**: You select any one of the
      options:

        i. **Application Patch**: Refers to a component of a computer program.

        ii. **Application**: Refers to an entire program designed to
            perform a set of coordinated functions.

        iii. **Unknown**

   d. **Version**: Type in the version of the Software.

   e. **Vendor**: Name of the entity who created the Software Package. The
      list is populated from the :ref:`Vendor Catalog <am-vendor>` List.

   g. **Package Architecture (Compulsory Field)**: Architecture of the
      package either 64bit or 32bit.

   h. **Description**: Add a Brief explanation of the Software Package.

   .. _spf-26:
   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.png
        :align: center
        :alt: figure 26

   h. **File Type**: Currently we support msi and exe file extensions in Windows.

   i. **Location Type**: Here you state whether the location is for a Shared Drive or from a Local Computer. 
      A Share drive is a locally hosted storage location whereas in Local Computer you have to upload the file. 
      A package can have only one location type.

   You can add additional arguments controlling install and uninstall behavior of the package; they are:

   a. :ref:`MSI File Parameter`
   b. :ref:`Parameters of Other Files (EXE/Linux)` 
        
   Fill in the fields and click **Add**. Now you have successfully added a
   Package, and it now appears on the :doc:`Package List View <package-registry-list-view>`.

MSI File Parameter
------------------

When uploading a MSI file you can attach/add additional files and arguments to control installation and uninstallation operations:

.. _spf-26.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.1.png
    :align: center
    :alt: figure 26.1

- **MSI Filename**: Type in the exact filename of the msi file. This allows the system to identify the installation file.

- **MST Filename**: A MST file allows you to collect installation options for 
  programs that use the Microsoft Windows Installer in a file. They can be used on the Installer (MSIEXEC.EXE) command line, 
  or used in a software installation Group Policy in a Microsoft Active Directory domain. Specific the exact name for the system to
  identify the file.

- **Arguments**: For example, if you want a reboot after installation then you can put an argument for that. You can access the the
  list of all the arguments from the CMD, by typing *filename.msi /?*.

.. _spf-26.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.2.png
    :align: center
    :alt: figure 26.2  

Parameters for Other Files (EXE/Linux)
--------------------------------------

.. _spf-26.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.3.png
    :align: center
    :alt: figure 26.3

The default behavior of our Agent Application is to install/uninstall Software silently; for this /S is added after the filename by default. 
Some software have a different argument value; for example, Skype (version 8.25 and above) has /Silent as the argument. 

If you want silent installation of a Software ,with a different argument, then type the exact filename followed by the argument.


Editing/Deleting a Software Package
-----------------------------------

**To Edit a Package:**

.. note:: Only Packages that are not associated with a deployment request
          can be edited.

1. Go to the :doc:`Package/Registry List
   View <package-registry-list-view>`.

2. In the list area, click on the **Edit Icon** adjacent to the package
   that you want to edit or click on the package name.

.. _spf-27:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.png
    :align: center
    :alt: figure 27

3. The Update package page opens. Make your changes and hit **Update**.

**To Delete a Package:**

.. note:: Only Packages that are not associated with a deployment request
          can be deleted.

In the List Page, click on the **Delete Icon** adjacent to the Package
that you want to delete. On confirmation, the package is deleted.


Creating a Registry Configuration
=================================

A Registry Configuration created as part of Deployment has Keys and Values, when
deployed can manipulate the behavior of Windows components, Hardware and Software of a computer. The system has
23 pre-defined Configurations out of the box; they are as follows:

.. note:: Related Topic: :ref:`Registry Deployment Use Case <A Registry Deployment Use Case>`.

.. _spf-27.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.png
    :align: center
    :alt: figure 27.1

**To create a New Registry Configuration:**

- Go to the :ref:`Registry List View <Viewing Package/Registry List View>`.

- Click on **Create Windows Registry Configuration** situated in the top right corner of the page.

- A dialog box opens where you have to enter a name and description. 

.. _spf-27.1.0:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.0.png
    :align: center
    :alt: figure 27.1.0

- When done, click on **Create** and your Configuration will be created. 

- You will be redirected to the **Update** page of the Configuration where you can modify the registry items.

Editing a Registry Configuration
--------------------------------

A user (See :ref:`Technician Roles`) can go to the Update page of a Registry Configuration from the :ref:`Registry List View <sp-list-view>` and modify its details.
Clicking on a Configuration name opens the Update page.

.. _spf-27.1.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.1.png
    :align: center
    :alt: figure 27.1.1

In the Update page a user can perform the following actions:

- Update Name and Description of the Registry Configuration (applicable in a custom Registry Configuration).

- Delete the Configuration (A pre-defined Configuration cannot be deleted).

- Add and modify custom Registry Items.

A Registry item is created using the **Create Registry Item** button. 

.. _spf-27.1.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.2.png
    :align: center
    :alt: figure 27.1.2

A Registry Item is a set of instructions to locate and modify a particular value name/key. A Registry Item has the following fields:

- **Action**: Following operations are permissable:

  a. Write Value

  b. Delete Value

  c. Add Key

  d. Delete Key

- **Header Key**: Following Header Keys are supported:

  a. **HKEY_LOCAL_MACHINE**: This branch contains computer specific information about the type of hardware, software, 
     and other preferences on a given PC. It is usually abbreviated as HKLM. You’ll mostly use the HKLM\Software key 
     to check machine-wide settings.

  b. **HKEY_USERS\.Default**: This branch contains individual preferences for each user of the computer, each user is represented 
     by a SID sub-key located under the main branch.

- **Sub Key**: Sub-keys are nested folders with in a hive. While creating a Registry Item, the Sub Key has to be manually filled in.

- **Data Type**: Following data types are supported:

    .. _spf-27.2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.2.png
        :align: center
        :alt: figure 27.2

  a. **REG_SZ**: This type is a standard string, used to represent human readable text values.

  b. **REG_BINARY**: This type stores the value as raw binary data. Most hardware component information is stored as binary data, 
     and can be displayed in an editor in hexadecimal format.

  c. **REG_DWORD**: This type represents the data by a four byte number and is commonly used for boolean values, 
     such as "0" is disabled and "1" is enabled. Additionally many parameters for device driver and services are this 
     type, and can be displayed in REGEDT32 in binary, hexadecimal and decimal format, or in REGEDIT in hexadecimal and decimal format.

  d. **REG_EXPAND_SZ**: This type is an expandable data string that is string containing a variable to be replaced when called by an application. 
     For example, for the following value, the string "%SystemRoot%" will replaced by the actual location of the directory 
     containing the Windows NT system files. (This type is only available using an advanced registry editor such as REGEDT32)

  e. **REG_MULTI_SZ**: This type is a multiple string used to represent values that contain lists or multiple values, 
     each entry is separated by a NULL character. (This type is only available using an advanced registry editor such as REGEDT32).

  f. **REG_QWORD**: A 64-bit number.

- **Value Name**: This field supports a user defined and dynamic variable. The dynamic variables are:

  .. _spf-27.3:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.3.png
      :align: center
      :alt: figure 27.3

- **Value Data**: This field supports a user defined and dynamic variable. The dynamic variables are:

  .. _spf-27.4:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.4.png
      :align: center
      :alt: figure 27.4

You can add n number of Registry Items in a Registry Configuration, and you can modify (or delete) them later. You cannot
modify a predefined Registry Item in a predefined Registry Configuration. 

Creating a new Registry Item
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Go to the :ref:`Registry Configuration List View <Viewing Package/Registry List View>`.

- Click on a Configuration to open its Update page. 

- In the new page, you can view all existing Registry Items. There is a Search Bar for searching Items.
  Learn how to use the :ref:`sp-search-bar`. Click on **Create Registry Item**.  

- A dialog box opens. Fill in the fields (:ref:`Learn about the fields <Editing a Registry Configuration>`) and add a description.

- When done, click on **Create**.