*********************************************
Managing Software Packages/Registry Templates
*********************************************

The first step towards Deployment is to add Software Packages/Registry Templates in
the system. A Package/Registry Template has to be manually added to the Deployment module before
it can be attached to a Deployment Request.

Whatever Packages/Templates you add, they all appear on the :doc:`Package List
View <package-registry-list-view>` (either under Windows Packages, Linux Packages or Windows Registry).
There you can modify a Package/Template details and also delete them.

Adding a Software Package
=========================

1. Go to the :doc:`Package List
   View <package-registry-list-view>` (either Windows or Linux).

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

        iii. **Operating System**: OS like Windows.

        iv.   **OS Component Patch**: Update patch of an OS.

        v.    **Unknown**

   e. **Version**: Type in the version of the Software.

   f. **Vendor**: Name of the entity who created the Software Package. The
      list is populated from the :ref:`Vendor Catalog <am-vendor>` List.

   g. **Package Architecture (Compulsory Field)**: Architecture of the
      package either 64bit or 32bit.

   h. **Description**: Add a Brief explanation of the Software Package.

   .. _spf-26:
   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.png
        :align: center
        :alt: figure 26

   i. **Package Location Type (Compulsory Field)**: Here you state whether
      the location is for a Shared Drive or a Remote URL. A Share drive is
      a locally hosted storage location whereas a Remote URL points to a
      location on the Internet. A package can have only one location type.

   j. **Package Locations (Compulsory Field)**: Here you type and add the
      location URL. You can add multiple URLs of the same package.

   k. **Locations**: Here you can view all the location URLs added to the
      Package. You can add multiple location URLs because a Software
      Package can be made up of multiple components each having a separate
      location.

      .. _spf-26.1:
      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.1.png
            :align: center
            :alt: figure 26.1

   l. Some software don't support **Silent Installation Argument**; for them, you can supply an explicit argument. 
      Select **Yes** which enables you to supply an explicit argument. Learn more about :ref:`Explicit Arguments` 
        
   Fill in the fields and click **Add**. Now you have successfully added a
   Package, and it now appears on the :doc:`Package List View <package-registry-list-view>`.


Silent Installation of a Software
---------------------------------

The default behavior of our Agent Application is to install Software silently; for this /S is added to the exe file by default. 
Some software have a different argument value; for example, Skype (version 8.25 and above) has /Silent as the argument. 

If you want silent installation of a Software ,with a different argument, then type the argument in the *Silent Installation Argument*
field while :ref:`adding the Software package <Adding a Software Package>`.

Explicit Arguments
^^^^^^^^^^^^^^^^^^
You can supply explicit arguments for software that doesn't support **Silent Installation Argument** while
:ref:`adding a Software package <Adding a Software Package>`. Such arguments will take care of onscreen options and perform a 
silent installation.

You can upload a file (extension depends on the Software) containing the arguments along with the file name. This will guide the silent installation of the software. 

.. _spf-26.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.2.png
    :align: center
    :alt: figure 26.2    


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


Creating a Registry Template
============================

A Registry Template created as part of Deployment has Keys and Values, when
deployed can manipulate the behavior of Windows components, Hardware and Software of a computer. The system has
24 pre-defined templates out of the box; they are as follows:

.. note:: Related Topic: :ref:`Registry Deployment Use Case <A Registry Deployment Use Case>`.

.. _spf-27.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.png
    :align: center
    :alt: figure 27.1

**To create a New Template:**

- Go to the :ref:`Registry Template List View <Viewing Package/Registry List View>`.

- Click on **Create Windows Registry Template** situated in the top right corner of the page.

- A dialog box opens where you have to enter a name and description. 

.. _spf-27.1.0:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.0.png
    :align: center
    :alt: figure 27.1.0

- When done, click on **Create** and your templates will be created. 

- You will be redirected to the **Update** page of the Template where you can modify the registry details.

Editing a Registry Template
---------------------------

A user (See :ref:`Technician Roles`) can go to the Update page of a Registry Template from the :ref:`Registry List View <sp-list-view>` and modify its details.
Clicking on a Template name opens the Update page.

.. _spf-27.1.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.1.png
    :align: center
    :alt: figure 27.1.1

In the Update page a user can perform the following actions:

- Update Name and Description of the Template.

- Delete the Template (A pre-defined Template cannot be deleted).

- Add and modify Registry Items.

A Registry Item is a set of instruction to locate and modify a particular value name/key. A Registry Item has the following fields:

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

You can add n number of Registry Items in a Registry Template, and you can modify (or delete) them later. You cannot
modify a predefined Registry Item in a predefined Registry Template. 

Creating a new Registry Item
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Go to the :ref:`Registry Template List View <Viewing Package/Registry List View>`.

- Click on a Template to open its Update page. 

- In the new page, you can view all existing Registry Items. There is a Search Bar for searching Items.
  Learn how to use the :ref:`sp-search-bar`. Click on **Create Registry Item**.  

- A dialog box opens. Fill in the fields (:ref:`Learn about the fields <Editing a Registry Template>`) and add a description.

- When done, click on **Create**.