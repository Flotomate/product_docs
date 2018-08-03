***********************************
Configuring Patch Download Location
***********************************

Currently, all Patches are downloaded by the Product Server from the
Update Server in a Shared Drive by default. A Patch is downloaded in the Shared
Drive when there’s a request for the Patch.

Computers during a deployment fetch the Patches from a Shared Drive;
the mechanism has been designed to save bandwidth during a deployment.
You cannot expect hundreds of Computers downloading the same Patch
separately. Instead, a Patch is first downloaded on the Shared Drive,
and then it is fetched by the Computers.

To facilitate the download process, you need to configure two things:
Proxy Server and Shared Drive configuration.

.. _proxy-settings:

Configuring Proxy Settings 
==========================

Before you can download anything, you have to make sure the Product
Server can access the internet. For this, you have to configure the
Proxy Settings in the product.

Accessing Proxy Settings
------------------------

Log in to your Dashboard.

Go to **Admin** (A Navigation Tab) >> **Proxy Server Configurations** (IT Infrastructure).

.. _pf-32:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-32.png
   :align: center
   :alt: figure 32

Configure Proxy Settings
------------------------

On clicking the :ref:`Proxy Server Configurations <proxy-settings>`, the Proxy Server
Configuration page opens. Click on **Edit** to make things editable. You
get three options to select from, and they are as follows:

-  **No Internet Access**: Select this option when you do not want the
   Product Server to access the Internet.

.. _pf-33:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-33.png
   :align: center
   :alt: figure 33

-  **Direct Internet Access**: Select this option when there are no
   Proxy settings between the Internet and the Product Server.

-  **Configure Manually**: If you have a Proxy, then you can configure
   it under this option. Your inputs go in the following fields:

   a. **Host**: Provide the address of the Computer running the Proxy
      server.

   b. **Port**: Refers to the port number of the Proxy server.

   c. **Username**: Username of the Proxy server

   d. **Password**: Password of the Proxy server.

Select an option and provide the required inputs. Hit **Update** to save
your changes. Now you have successfully configured your Proxy settings.

.. _share-drive:

Configuring Shared Drive
========================

A Shared Drive is a shared resource on a Computer network. It is a
device or piece of information on a Computer that can be remotely
accessed from another Computer, typically via a local area network or an
enterprise intranet, transparently as if it were a resource in the local
machine.

The Shared Drive is the default location where the Product Server stores
all the Patches before deployment. The product asks for a Shared Drive
when Patches don’t have a locally stored Package file.

**To Setup a Shared Drive:**

1. Log in to your Dashboard.

2. Go to **Admin** (A Navigation Tab) >> **Shared Drive Configurations**
   (Patch/Package Deployment).

.. _pf-34:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-34.png
   :align: center
   :alt: figure 34

3. The Shared Drive Configuration page opens. Here you get the following
   fields and options:

.. _pf-35:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-35.png
   :align: center
   :alt: figure 35
::
    a. In section-A (:numref:`pf-35`), you type in a URL that tells the Product Server the location of the Shared Drive.

    b. If you want the Patches to be automatically downloaded when there’s a request, then turn on the toggle button in section-B.

   Click the **Edit** button to make the fields editable. Once you enter
   the URL, you can test the connection; the product tells you whether a
   successful connection was established with the Share Drive. Once you
   are done with everything, click on **Update** to save your changes.

.. _configuring-package-location-single-patch:

Configuring Package Location for a single Patch
===============================================

It may happen that a Patch already exists in an accessible location as a
package file, and to prevent the Product Server from downloading it
again, we can add an URL in the Patch so that Computers know they can
fetch the Patch directly from the mentioned location.

**To Configure Package Location:**

1. Go to the :ref:`Details View <patch-details-view>` of a Patch.

2. Click on **Configure Packages** from the **Action Menu** situated in
   the top right corner of the page.

.. _pf-36:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-36.png
   :align: center
   :alt: figure 36

3. The Configure Package dialog box opens. Paste the URL into the empty
   field and click on **Add Location**. You can add multiple locations
   in the dialog box.

.. _pf-37:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-37.png
   :align: center
   :alt: figure 37

4. In the Configure Package dialog box, you can view the URLs that have
   been added. You can delete an URL by clicking the adjacent delete
   icon.