******************************************
ITSM Plugin - Active Directory Integration
******************************************

This is a standard plugin offered by Flotomate to all our users.

**Purpose**: The plugin provides integration with an Active Directory. When the plugin is executed it can 
create new users, update existing user, reset user password and delete a user using the LDAP protocol.

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

5. You can trigger the plugin as an action item to a :ref:`workflow <ad-workflow>` and :ref:`Scenario <Create a Scenario>`. Following are some of the action items (as part of workflows):

   Before triggering any action, one has to understand the parameters that goes into making an input to the active directory. 
   
   a. **optype (operation type)**: Refers to the kind of operations you want with the plugin. You can select any one from the below types:

     i. create: Create a new user. 

     ii. delete: Delete a user only. 

     iii. update: Update object properties. 

     iv. addtogroup: Adds an existing user to a group. 

   b. **base-dn**: A base dn is the point from where a server will search for users. It is the main directory. An example base-dn would
      be: cn=admin,dc=example,dc=com.

   c. **CN (Common Name)**: Refers to the name of the object with attributes. 

   Following are examples of the actions (operations) mentioned above. 

   a. **Create a new user**: A workflow creates a new user in the Active Directory using the plugin when a request is created. Here the 
      following parameters have been set:

      i. **optype**: create (mandatory to create a new user).
      ii. **base-dn**: CN=User,DC=flotomate,DC=com (refers to the top level directory called **User**)
      iii. **CN**: Name of the object here it is Bhavin_test_User. 
      iv.  **Properties of object Bhavin_test_User**: st and mail (AD properties).  

      .. _plgm-4:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-4.png
          :align: center
          :alt: figure 4

   b. **Add user to a group**: A workflow adds a user to a group in the Active Directory using the plugin when a request is created.Here the 
      following parameters have been set:

      i. **optype**: addtogroup (mandatory to add an existing user to a group).
      ii. **base-dn**: CN=User,DC=flotomate,DC=com (refers to the top level directory called **User**)
      iii. **CN**: Name of the object here it is Bhavin_test_User. 
      iv.  **group**: It is the name of the group here it is DnsAdmins mentioned as **CN-DnsAdmins, CN=Users, DC=flotomate, DC=com**.   

      .. _plgm-5:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-5.png
          :align: center
          :alt: figure 5

   c. **Delete a user**: A workflow that deletes a user in the Active Directory using the plugin when a request, with a specific tag, is created. Here the 
      following parameters have been set:

      i. **optype**: delete (mandatory to delete a user).
      ii. **base-dn**: CN=User,DC=flotomate,DC=com (refers to the top level directory called **User**)
      iii. **CN**: Name of the object. Here a placeholder has been selected instead of the username. 
      
      .. _plgm-6:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-6.png
          :align: center
          :alt: figure 6

   d. **Update a user info**: A workflow updates a user in the Active Directory using the plugin when a request, with a specific tag, is created. Here the 
      following parameters have been set:

      .. note:: If given properties don't exist then they will be created.

      i. **optype**: Update (mandatory to update an existing user).
      ii. **base-dn**: CN=User,DC=flotomate,DC=com (refers to the top level directory called **User**)
      iii. **CN**: Name of the object. Here a placeholder has been selected instead of the username.
      iv. **mail**: Email of the user. Here a placeholder has been used. 
   
      .. _plgm-7:

      .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-7.png
          :align: center
          :alt: figure 7