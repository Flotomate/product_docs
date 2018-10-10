**********************************************
Create a New User in AD for LDAP Configuration
**********************************************

Creating a New User in Active Directory
=======================================

-  Go to Server Manager from your Windows Server.

-  Create a new user from the Active Directory Users and Computers.

Setting Permission for New User
===============================

-  Go to Active Directory Administrative Center from Server Manager.

-  Open the new user details page and go to **Member of the** section.

-  Add an Object name using the **Advanced** option.

.. _ldap-ad-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ldap-configuration/LDAP-AD-1.png
    :align: center
    :alt: figure 1

-  Once added, the Read Only Domain Controller should appear in the
   Member of the section.

-  Once you are done, click on OK.

Use the credential of the new user while setting up LDAP with the
Product.
