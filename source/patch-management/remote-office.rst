*************
Remote Office
*************

Modern organizations are geographically dispersed. They have offices at different locations all controlled from a main office. Offices that are
away from the main office are termed as Remote Offices. It may happen that all the offices of an organization form part of a single 
network. Individual offices can have a relay server: A relay server is used to allow communications from outside a company's firewall 
to internal Servers.  

In order to accommodate such situations, we have the following Patch Management features:

- A user can create a group of computers for a location and save it as a Remote Office. 

- A user can add a Remote Office in a scope instead of individual computers for Patch Management.

- Users can point a Remote Office to a relay Server. This is useful when there are multiple offices, and the admin doesn't want them
  to hog the central server for Patch download. This is why we have the feature that allows a Remote Office to download Patches from a 
  local shared drive (routed via relay server). 


**To Add and Configure a Remote Office:**

Go to **Admin** (a Navigation Tab) >> **Remote Office**
(Patch/Package Management).

.. _P-remote-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-REMOTE-1.png
   :align: center
   :alt: figure 1

The Remote Office page opens. Here you can search and view your existing Remote Offices. Click on **Add Remote Office** in the top right corner

You are redirected to a new page. Here you enter the following information:

.. _P-remote-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-REMOTE-2.png
   :align: center
   :alt: figure 2

- Section A is where you enter the Name, Description and Location of the Remote Office.

.. note:: Related Topic: :ref:`ad-location`

- Section B is where you configure for a relay server. Select **Direct Communication** when you don't want to use a relay server.
  
  If you want the Remote office to download Patches from a local source (via shared drive) then select **Distribution Server**. 
  Enter a IP and a Port number so the product server can route the Patches to the Remote Office's shared drive. 

- Section C is where you add computers to the Remote Office. Learn how to :ref:`add computers <add-computer-scope>`.

- When done, click on **Create** to save your remote office.

.. _P-remote-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-REMOTE-3.png
   :align: center
   :alt: figure 3