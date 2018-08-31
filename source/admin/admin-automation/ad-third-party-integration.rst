*************************************
Integration with Third Party Services
*************************************

Flotomate supports Jira integration out of the box and any other third
party client supporting rest API.

.. note:: Integration requires Administrative rights

Jira Integration
================

-  Go to **Admin** >> **Integrations** (Automation)

-  You see an empty list if you are integrating an app for the first
   time, else you can see all the existing third-party integrations.

-  Click **Create an Integration** situated in the top right corner of
   the page.

-  Give a Name to the service and a suitable description.

-  Select Jira API Integration from the below option.

-  Type in the username, password, and the domain name.

-  Save your settings before exiting.

.. _adf-55:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-55.png
    :align: center
    :alt: figure 55

Rest API Client
===============

A REST API defines a set of functions which developers can perform
requests and receive responses via HTTP protocol such as GET and POST.
Flotomate allows third party clients to create Requests using REST API.

Before using REST API, you have to create an API Client.

**Creating an API Client:**

-  Go to **Admin** >> **Integrations** (Automation).

.. _adf-55.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-55.1.png
    :align: center
    :alt: figure 55.1

-  Click on **Create an Integration** situated in the top right corner of the page.

-  Give the settings a name and description.

-  Select the **Rest API Client** option from below, and you have two options with respect to user selection.

   a. **Allow any User**: You can use the credentials of any user (registered with the product) to make API calls.

   b. **Allow specific User**: You can only use the credentials of the mentioned user for making API calls.

.. _adf-55.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-55.2.png
    :align: center
    :alt: figure 55.2  

-  Click on **Create** to save your API Client.

.. note:: The user acts as an identifier for all interactions made using
          the API. It is preferable to create a dummy user specifically for the
          Client.

- Open the API client again from the Integrations page to view the Client **ID** and **Secrete**.

.. _adf-56:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-56.png
    :align: center
    :alt: figure 56

Learn how to make :ref:`API Calls <How to Create Incident Using REST API>`.

Edit Integration
================

-  Go to **Admin** >> **Integrations** (Automation).

-  Click the edit icon adjacent to the API name that you want to edit.

-  Make your changes and hit **Update**.

You can delete any API integration by clicking the Delete icon, or go to
edit page and click **Delete**.

Disable a API Integration
=========================

-  Go to **Admin** >> **Integrations**.

-  You can disable any API with the adjacent toggle.

.. _adf-57:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-57.png
    :align: center
    :alt: figure 57