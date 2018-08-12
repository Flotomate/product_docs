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

.. _spf-27.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.png
    :align: center
    :alt: figure 27.1

**To create a New Template:**

- Go to the :ref:`Registry Template List View <Viewing Package/Registry List View>`.

- Click on **Create Windows Registry Template** situated in the top right corner of the page.

- A dialog box opens where you have to enter a name and description. 

.. _spf-27.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.1.png
    :align: center
    :alt: figure 27.1

- When done, click on **Create** and your templates will be created. 

Editing a Registry Template
---------------------------

A Registry Template houses Registry Items. Each Registry Item has the following:

- **Action**: Following operations are permissable:

  a. Write Value

  b. Delete Value

  c. Add Key

  d. Delete Key

- **Header Key**: Following Header Keys are supported:

  a. HKEY_LOCAL_MACHINE

  b. HKEY_USERS\.Default

- **Sub Key**: User defined

- **Data Type**: Following data types are supported:

  .. _spf-27.2:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-27.2.png
      :align: center
      :alt: figure 27.2

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

You can add n number of Registry Items in a Registry Template, and you can modify them later. You cannot
modify a predefined Registry Item in a predefined Registry Template. 

**To Create a new Registry Item:**

- Go to the :ref:`Registry Template List View <Viewing Package/Registry List View>`.

- Click on a Template to open its details view. 

- In the new page, you can view all existing Registry Items. There is a Search Bar for searching Items.
  Learn how to use the :ref:`sp-search-bar`. Click on **Create Registry Item**.  

- A dialog box opens. Fill in the fields (:ref:`Learn about the fields <Editing a Registry Template>`) and add a description.

- When done, click on **Create**.