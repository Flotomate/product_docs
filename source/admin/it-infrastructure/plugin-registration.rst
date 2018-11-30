*****************
Register a Plugin
*****************

A plugin is a piece of code that integrates with our main server to perform a specific function. 
In the context of our product, a plugin is nothing but a .fp bundle (i.e. Kind of app, zip). 

A plugin is first installed in a plugin server. A plugin server is a server which hosts/runs plugins. It is like our main server with a specialized purpose of running plugins. 
The main server will call a plugin server to execute specific plugin and get the desired output.

Once the plugin is installed. A user has to register the plugin in the ITSM tool. Registering a plugin establishes all the 
dependencies and makes it available for execution.

**Registering a Plugin:**

1. A plugin is registered from the admin section. Go to **Admin** >> **Plugins** (IT Infrastructure). 

2. Click on **Register New Plugin** situated in the top right corner.

.. _ad-plg-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-PLG-1.png
    :align: center
    :alt: figure 1

3. Select a plugin and click on **Register**.

4. The update page of the plugin opens. Here you have to configure the plugin.

.. seealso:: Learn :ref:`how plugin server is setup <Plugin Server Setup Guide>`.

