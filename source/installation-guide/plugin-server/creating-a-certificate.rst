******************************************
Setting SSL Connection to Active Directory
******************************************

In order to create a user, with password, in the Active Directory from Motadata using a plugin, an admin has to
configure SSL connection between the plugin server and AD. 

An admin has to generate a SSL certificate from the AD and configure the same in the plugin server. You need the following 
things installed on the Windows Domain Controller.

**Prequisite**

- Internet Information Services

- Windows Certificate Services

- Windows 2000 Pack 2 (If you are using Windows 2000)

- Windows 2000 High Encryption Pack (128-bit) (If you are using Windows 2000)

Step 1: Install AD Certificate Services
=======================================

An admin has to install Certificate Services, if installed he can skip to step 2. The below screenshots are from Windows Server 2008.

1. Logs into AD as administrator. 

2. Goes to Start >> Administrative Tools >> Server Manager.

3. Clicks on **Add Roles** from the **Roles Summary** section.

.. _plg-11:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-11.png
    :align: center
    :alt: figure 1

4. On **Server Roles** page, selects **Active Directory Certificate Services** and then checks **Next**.

.. _plg-12:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-12.png
    :align: center
    :alt: figure 2

5. Selects **Certification Authority** from **Role Services** and clicks on **Next**. 

.. _plg-13:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-13.png
    :align: center
    :alt: figure 3

6. Selects **Enterprise** from **Setup Type** and clicks on **Next**.

.. _plg-14:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-14.png
    :align: center
    :alt: figure 4

7. Clicks on **Root CA** from **CA Type** and then clicks on **Next**. 

.. _plg-15:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-15.png
    :align: center
    :alt: figure 5

8. Admin can configure cryptography services from **Private Key** >> **Cryptography**. Keeping the default config is fine.
   He then clicks on **Next**.

.. _plg-15:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-15.png
    :align: center
    :alt: figure 5

9. Inputs the common name of the CA and clicks on **Next**. 

.. _plg-16:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-16.png
    :align: center
    :alt: figure 6

10. Accepts default values in the **Validity Period** and sets storage location for certificate in **Certificate Database** page, 
    and clicks on **Next**. 

.. _plg-17:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-17.png
    :align: center
    :alt: figure 7

.. _plg-18:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-18.png
    :align: center
    :alt: figure 8

11. Clicks on **Install** after verifying information.

12. Admin verifies the installation from the results screen.

.. _plg-20:
    
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/plugin-server/PLG-20.png
    :align: center
    :alt: figure 10

Step 2: Obtain Server Certificate
=================================

Admin will now add the SSL certificate to the list of accepted certificates. 

1. Opens Run and enters **certsrv.msc**.

2. Admin right clicks on the name of the certificate (right hand side) and selects **Properties**. 

3. Under General tab, admin selects **View Certificate**.

4. In new dialog box, selects **Details** tab >> **Copy to File**.

5. Export wizard starts. Admin selects **Base-64 encoded binary X.509(.CER)** option.

6. Enters location and name, and confirms export. 

Step 3: Add Server Certificate as Trusted
=========================================

Admin has to import the certificate created in the above steps to the AD server. This step ensures that a plugin can have
a secure connection with the AD server. 

1. Opens Microsoft Management Console (Start >> Run >> mmc.exe);

2. Chooses File >> Add/Remove Snap-in;

3. Chooses Add in the Standalone tab;

4. Chooses the Certificates snap-in, and click Add;

5. Chooses the Computer Account in the wizard, and then selects Local Computer. Ends wizard by clicking on **Finish**;

6. Closes the Add/Remove Snap-in dialog;

7. Navigate to Certificates in Local Computer.

8. Selects store to import:
   a. Chooses Trusted Root Certification Authorities in case of Root CA certificate from issuing company. 
   b. Chooses Other People if certificate is from the server itself.

9. Choses All Tasks >> Import by right clicking the store. 

10. Follow wizard and provide the certificate file. 

Now we will import the certificate in the plugin server. :ref:`Learn more <plug-certificate>`.