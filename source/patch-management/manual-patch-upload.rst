**************************
Manually Uploading a Patch
**************************

A user can upload a Patch manually and deploy the same across multiple computers. This feature is useful in the following scenarios:

- In an office where there's no internet connection, and the servers are hosted locally. 

- Installing linux Patches since there's no defined update server. 

Following are the steps to upload a Patch manually:

- Go to :ref:`Patch List View`.

- Click on **Add Patch** from the Action Menu.

.. _pf-ad-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-AD-1.png
    :align: center
    :alt: figure 1

- The Add patch page opens with the following fields:

    .. _pf-ad-2:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-AD-2.png
        :align: center
        :alt: figure 2

   a. Name of the Patch.

   b. Name of the Platform (Currently, either Windows or Linux).

   c. Severity as defined by the Patch vendor. 

   d. Supported architecture.

   e. Update category: mainly talks about the type of the Patch. Selection is done from a predefined list.

   f. Software Catalog: you have to relate the patch with a software in the catalog. Learn how to add software in :ref:`Software Catalog`.

   g. Reboot requirement.

   h. Description of the Patch.

   i. Windows specific details (KBID, Bulletin ID and Release Date). Refer Software vendor site for this info.

- When done, click on **Done**. The Patch will be added to the Patch List. 

- Now you have to configure the location of the file in the Patch that you have added. 

- Open the Patch from the :ref:`Patch List View`.

- Click on **Configure Patch**. 

.. _pf-ad-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-AD-3.png
    :align: center
    :alt: figure 3

- A dialog box opens where you can add multiple share drive file paths or upload files. 

.. _pf-ad-4:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-AD-4.png
    :align: center
    :alt: figure 4

-  Now you can initiate a :ref:`Deployment Request <Manually Creating a Request>` using the uploaded Patch.
