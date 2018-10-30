*************************
Plugin Server Setup Guide
*************************

**What is a Plugin?**

A plug-in is a piece of code that integrates with our main server to perform a specific function. 
In the context of our product, a plugin is nothing but a .fp bundle (i.e. Kind of app, zip). 

**What is a Plugin Server?**

Plugin server is a server which hosts/runs plugins. It is like our main server with a specialized purpose of running plugins. 
The main server will call a plugin server to execute specific plugin and get the desired output.

Plugin Server Setup
===================

Enabling plugin capabilities in the main server is a three step process:

- Setting up a plugin server (Step 1).

- Copying .fb bundles in the plugin server (Step 2). 

- Configuring the main server with the plugin server (Step 3). 

.. note:: The plugin server can be setup in the main server or separately. 

.. _plugin-server-installation:

Plugin Server Configuration (Step 1)
------------------------------------

1. Open plugin server terminal and go to the directory of **plugin_server_CI**.  

.. _plg-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-1.png
    :align: center
    :alt: figure 1

2. Initiate installation of plugin server with the following command:

   **sudo ./plugin_server_CI**

.. _plg-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-2.png
    :align: center
    :alt: figure 2

3. Wait for the installation to finish. You will get the below screen.

.. _plg-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-3.png
    :align: center
    :alt: figure 3

.. _plugin-transfer:

Copying Plugin Bundle in the Plugin Server (Step 2)
---------------------------------------------------

1. Transfer plugin .fp file/files to the plugin server. 

.. _plg-4:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-4.png
    :align: center
    :alt: figure 4

2. Log in as root with **Sudo -i**. Go to the directory of  the .fp files. 

3. Now copy the .fp file/files to the plugin folder.

   **cp *.fp /opt/flotomate/plugin-server/plugins**

.. _plg-5:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-5.png
    :align: center
    :alt: figure 5

4. Now go to the plugins directory. 

5. Run **ls-la** and check user; if user is root then change that to fmtuser and fmtusergroup.

   **chown fmtuser:fmtusergroup *.fp**

.. _plg-6:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-6.png
    :align: center
    :alt: figure 6

6. Restart plugin service in the plugin server with the following command:

   **sudo systemctl restart ft-plugin-server.service**

.. _main-server-setup:

Main Server Configuration (Step 3)
----------------------------------

1. Open terminal of the main server. We will now input the IP address of the plugin server in the **services-config.yaml** file. 

2. Login as root: **sudo -i**. Go to the config folder using the command:

   **cd /opt/flotomate/main-server/config**

.. _plg-7:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-7.png
    :align: center
    :alt: figure 7

3. Open **services-config.yaml** using nano: 

   **nano services-config.yaml**

4. Go down to the **services** section and update the plugin server address.

.. _plg-8:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-8.png
    :align: center
    :alt: figure 8

5. Save your changes, and restart the main-server with the following command:

   **systemctl restart ft-main-server.service**

Now you are done with installing the server. 