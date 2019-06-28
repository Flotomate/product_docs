******************************
External Storage Configuration
******************************

Our current architecture only allows for a file server to act as a central storage for the following operations:

- Deployment of Patches.
- Deployment of Packages.
- Self-upgrade of Motadata Agent application.

.. note:: Learn about :ref:`File Server <File Server Installation Guide>`.

A file server is the backbone of our desktop automation features, which is why it becomes important for an admin to make sure there is 
sufficient space in their file server. We now have the External Storage Configuration which performs two functions:

- Clean the file server.

- Generate a notification when the file server reaches a certain storage limit.

**Steps to External Storage Configuration:**

1. Go to **Admin** >> **External Storage Configuration** (under Patch/Package Deployment).

2. The External Storage Configuration page will open. Click the edit button to make options editable.

.. _ad-sto-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/external-storage-config/AD-STO-1.png
    :align: center
    :alt: figure 1

3. Here you can toggle-on two functions:

   a. **Remove Old Patches**: Turning this option allows you to delete patches older than a specified number of months considering
      only the release date of a patch. Toggle the option on and set a number of months.

      .. _ad-sto-2:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/external-storage-config/AD-STO-2.png
          :align: center
          :alt: figure 2

   b. **Notify on size exceed**: You can set the system to generate a notification when the storage in the file server reaches a 
      certain limit. The recipient of the notification can be a Requester Group or All Requester Groups, and individual emails.
      You can specify the storage limit in terms of GB. 

      .. _ad-sto-3:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/external-storage-config/AD-STO-3.png
          :align: center
          :alt: figure 3

4. When done click on **Update** to save your changes. 

Test Connection with File Server
================================

You can check your connection with the file server from **Admin** >> **External Storage Configuration** (under Patch/Package Deployment).
On the External Storage Configuration page click on the **Test Connection** button.

.. _ad-sto-4:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/external-storage-config/AD-STO-4.png
    :align: center
    :alt: figure 4