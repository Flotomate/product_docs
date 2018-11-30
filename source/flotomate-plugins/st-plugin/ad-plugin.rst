******************************************
ITSM Plugin - Active Directory Integration
******************************************

This is a standard plugin offered by Flotomate to all our users.

**Purpose**: The plugin provides integration with an Active Directory. When the plugin is executed it can 
create new users, update existing users, read user data and delete a user using the LDAP protocol.

**Perquisite**: Plugin server needs to be setup with the main server (:ref:`Learn More <Plugin Server Setup Guide>`). 

**Plugin Setup**

1. Download the plugin .fp file and transfer it to the plugin server (:ref:`Learn More <plugin-transfer>`).

2. Restart the plugin server.

3. Register the plugin in the ITSM tool (:ref:`Learn more <Register a Plugin>`).

.. _plgm-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-2.png
    :align: center
    :alt: figure 2

4. Update the plugin with the following information:

   a. **AD Server URL**: Type in the AD server URL using the LDAP protocol.

   b. **Domain Admin User**: Active Directory username.

   c. **Domain Admin Password**: Active Directory password. 

.. _plgm-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-3.png
    :align: center
    :alt: figure 3

5. You can trigger the plugin as an action item to a :ref:`workflow <ad-workflow>`. Following are some of the action items:

   a. **Create a new user**: A workflow creates a new user in the Active Directory using the plugin when a request is created.

      .. _plgm-4:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-4.png
          :align: center
          :alt: figure 4

   b. **Create a new user group**: A workflow creates a new user group in the Active Directory using the plugin when a request is created.

      .. _plgm-5:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-5.png
          :align: center
          :alt: figure 5

   c. **Delete a user**: A workflow delete a user in the Active Directory using the plugin when a request, with a specific tag, is created.
      
      .. _plgm-6:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-6.png
          :align: center
          :alt: figure 6

   d. **Update a user info**: A workflow updates a user in the Active Directory using the plugin when a request, with a specific tag, is created.
   
      .. _plgm-7:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-7.png
          :align: center
          :alt: figure 7