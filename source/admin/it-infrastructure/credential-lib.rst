******************
Credential Library
******************

The product has a centralized credential library to store and manage
Network Credentials. When a Network is created, credentials are added
from the Credential Library.

A Network can have multiple devices, and you have to make sure
credentials of all those devices are in the Credential Library before
adding the Network to the product.

We provide four easy Discovery Types to choose.

-  WMI

-  SSH

-  SNMP

-  SNMP V3

.. note:: Managing credentials requires administrative rights.

Add Credential
==============

1. Go to **Admin** (One of the Navigation Tabs)>> **Credential Library**
   (IT Infrastructure). The Credentials page opens where you can view
   all the existing credentials if any.

2. Click the **Add Credential** situated in the top right corner of the
   page. The Add Credential dialog box opens.

.. _adf-64:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-64.png
    :align: center
    :alt: figure 64

3. Add a **Name** to the credential and select a Discovery Type which
   determines the authentication parameters. Now let’s understand the
   Discovery Types available with Flotomate:

    **WMI (Windows Management Instrumentation):**

    .. note:: Please refer to :numref:`adf-64`.

    This protocol is used to scan for data in Windows-based systems
    within a Domain or Workgroup.

    a. **Domain Username & Password**: These are the credentials for the
       Administrator Account that has access to all the nodes in the
       domain.

    b. **Domain Name**: The part of a network address which identifies
       it as belonging to a particular domain.

    c. **Domain Discovery**: If the credential belongs to an Asset which
       is part of a domain then you have to tick mark this field.

    **SSH (Secure Shell):**

    The SSH protocol is used to discover UNIX based machines.

    .. _adf-65:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-65.png
        :align: center
        :alt: figure 65

    a. **Domain Username & Password**: These are the credentials for the
       user account specific to the Asset that we are going to discover. In
       case there are multiple machines, a universal account can be created
       on all the machines to make Discovery easy; else, each different
       account requires a separate SSH credential.

    **SNMP (Simple Network Management Protocol)**

    Flotomate uses this application-layer protocol to scan devices with
    the SNMP agent in a managed network.

    .. _adf-66:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-66.png
        :align: center
        :alt: figure 66

    a. **Community String**: The Community String acts as a password in a
       managed network. It is sent along with each SNMP Get-Request to gain
       access to an SNMP enabled device’s data. If the community string is
       correct, the get request fetches the data.

    **SNMP V3 (Simple Network Management Protocol Version 3):**

    It is a secure version of SNMP with user-based authentication.

    .. _adf-67:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-67.png
        :align: center
        :alt: figure 67

    a. **Community String**: It is a password which is used for
       authentication.

    b. **Authentication Protoco**: Use the protocol that you want to use
       (we support both MD5 and SHA) in field-A.

    c. **Username**: Enter your username.

    d. **Auth Passphrase**: This is the Auth password

    e. **Privacy Passphrase**: This is the Privacy password.

    f. **Security Level**: Choose an appropriate security level from the
       following options:

        i. **Private Authentication**: Uses protocol like SHA for
           authentication and protocol like AES for privacy.

        ii. **No Private Authentication**: The only authentication protocol
            is used.

        iii. **No Private No Authentication**: Data transfer with
             authentication and privacy.

**Edit/Delete Credentials**

1. Go to **Admin** >> **Credential Library** (IT Infrastructure).

.. _adf-68:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-68.png
    :align: center
    :alt: figure 68

2. Click the Edit Icon adjacent to the credential you want to edit. In
   the Edit Credential dialog box, make your changes and hit
   **Update**.

You can delete any credential by clicking the Delete icon adjacent
to the credential.