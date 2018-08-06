**************************
Managing Software Packages
**************************

The first step towards package deployment is to add Software Packages in
the system. A Package has to be manually added to the Package Management before
it can be attached to a Deployment Request.

Whatever Packages you add, they all appear on the :doc:`Package List
View <package-registry-list-view>` (either under Windows or Linux).
There you can modify the Package details and also delete them.

Adding a Software Package
=========================

1. Go to the :doc:`Package/Registry List
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

   c. **Package Type (Compulsory Field)**: You select any one of the
      options:

        i. **Application Patch**: Refers to a component of a computer program.

        ii. **Application**: Refers to an entire program designed to
            perform a set of coordinated functions.

        iii. **Operating System**: OS like Windows.

        iv.   **OS Component Patch**: Update patch of an OS.

        v.    **Unknown**

   d. **Version**: Type in the version of the Software.

   e. **Vendor**: Name of the entity who created the Software Package. The
      list is populated from the Vendor Catalog.

   f. **Package Architecture (Compulsory Field)**: Architecture of the
      package either 64bit or 32bit.

   g. **Description**: Add a Brief explanation of the Software Package.

   h. **Package Location Type (Compulsory Field)**: Here you state whether
      the location is for a Shared Drive or a Remote URL. A Share drive is
      a locally hosted storage location whereas a Remote URL points to a
      location on the Internet. A package can have only one location type.

   i. **Package Locations (Compulsory Field)**: Here you type and add the
      location URL. You can add multiple URLs of the same package.

   j. **Locations**: Here you can view all the location URLs added to the
      Package. You can add multiple location URLs because a Software
      Package can be made up of multiple components each having a separate
      location.

    .. _spf-26:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-26.png
        :align: center
        :alt: figure 26

   Fill in the fields and click **Add**. Now you have successfully added a
   Package, and it now appears on the :doc:`Package List View <package-registry-list-view>`.

Editing/Deleting a Software Package
===================================

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