********************
Infrastructure Setup
********************

Setting up the Infrastructure is the first step before Asset Discovery.
This step is prerequisite for Agentless Discovery of Assets, but not for
the Agent Application.

.. note:: Setting up the Infrastructure requires Administrative rights.

The Infrastructure Setup consists of three broad sections:

-  DNS Configuration:

-  Credential Library:

-  Networks:

DNS Configuration:
==================

The DNS configuration helps the product in resolving hostnames of Assets
against their IPs from the DNS. A DNS is useful especially when the
network protocol is DHCP.

In DHCP protocol, the IPs of Assets keep on changing, so the hostname of
a machine is taken as the unique identifier. The DNS maps all the
hostnames of the Assets with their IP addresses. Flotomate connects with
the DNS using the information provided by an administrator in the DNS
Configuration page.

.. note:: DNS configuration requires you to have administrative rights.

**Configuring DNS**

1. Log in to your Dashboard and head to **Admin** from the Navigation
   Tabs. Use search, or you can find the **DNS Configuration** in IT
   Infrastructure.

.. _amf-156:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-156.png
    :align: center
    :alt: figure 156

2. The DNS Configuration page opens. Click on **Edit** to make the
   fields editable.

3. Enter your primary DNS address in the primary field and your backup
   DNS address in the secondary field.

4. The Base URL field is the domain name of Flotomate hosted on your
   server. Enter the name and hit Update to save your changes.

You can later edit your DNS configuration in the DNS Configuration page.

Credential Library
==================

Flotomate provides an interface to upload all your credentials, so our
product can authenticate for an authorized access to a network.

A repository stores all Credentials, which we call a library where you
can manage (add, edit and delete) them.

We provide four easy Discovery Types to choose from:

-  WMI

-  SSH

-  SNMP

-  SNMP V3

.. note:: Managing credentials requires administrative rights.

**Adding Credential**

1. Go to **Admin** (One of the Navigation Tabs)>> **Credential Library**
   (under IT Infrastructure). The Credentials page opens where you can
   view all existing credentials.

2. Click the **Add Credential** situated in the top right corner of the
   page. The Add Credential dialog box opens.

.. _amf-157:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-157.png
    :align: center
    :alt: figure 157

3. Add a **Name** to the credential and select a Discovery Type which
   determines the authentication parameters. Now let’s understand the
   available Discovery Types:

    **WMI (Windows Management Instrumentation):**

    .. note:: Please refer to :numref:`amf-157`.

    This protocol is used to scan for data in Windows-based systems
    within a Domain or Workgroup.

        a. **Domain Username & Password**: These are credentials of the
           Administrator Account that has access to all the nodes in the
           domain.

        b. **Domain Name**: The part of a network address which identifies
           it as belonging to a particular domain.

        c. **Domain Discovery**: Enabling this marks the credential as
           discoverable. It means that the credential is for Discovery.
 
    **SSH (Secure Shell):**

    The SSH protocol is used to discover UNIX based machines.

        .. _amf-158:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-158.png
            :align: center
            :alt: figure 158

        a. **Domain Username & Password**: These are the credentials for the
           user account specific to the Asset that we are going to discover. In
           case there are multiple machines, a common user can be created (with
           root access) in all the machines to make discovery easy; else, each
           different account would require a separate SSH credential.

    **SNMP (Simple Network Management Protocol)**

    Flotomate uses this application-layer protocol to scan devices with
    the SNMP agent in a managed network.

        .. _amf-159:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-159.png
            :align: center
            :alt: figure 159

        a. **Community String**: The Community String acts as a password in a
           managed network. It is sent along with each SNMP Get-Request to gain
           access to an SNMP enabled device’s data. If the community string is
           correct, the get request fetches the data.

    **SNMP V3 (Simple Network Management Protocol Version 3):**

    It is a secure version of SNMP with user-based authentication.

        .. _amf-160:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-160.png
            :align: center
            :alt: figure 160

        a. **Community String**: It is like a password which is used for
           authentication.

        b. **Authentication Protoco**\ l: Use the protocol that you want to use
           (we support both MD5 and SHA) in field-A (:numref:`amf-160`).

        c. **Username**: Enter your username.

        d. **Auth Passphrase**: This is the Auth password

        e. **Privacy Passphrase**: This is the Privacy password.

        f. **Security Level**: Choose an appropriate security level from the
           following options:

            i. **Private Authentication**: Uses protocols like SHA for
               authentication and protocols like AES for privacy.

            ii. **No Private Authentication**: only use authentication
                protocol.

            iii. **No Private No Authentication**: Data transfer with
                 authentication and privacy.

**Testing Connection**

.. role:: red
You can test the credential by connecting with a computer (:red:`works for WMI and SSH credentials`). Click on
**Test Connection** next to **Save**. A dialog box opens asking for the
IP of the machine. Submitting an IP starts a process that tells whether
a successful connection was established or not.

.. _amf-161:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-161.png
    :align: center
    :alt: figure 161

**Editing/Deleting Credentials**

1. Go to **Admin** >> **Credential Library** (under IT Infrastructure).

.. _amf-162:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-162.png
    :align: center
    :alt: figure 162

2. Click the edit icon adjacent to the credential you want to edit. You
   see the Edit Credential dialog box. Make your changes and hit
   **Update**.

3. You can delete any credential by clicking the Delete icon adjacent
   to a credential.

.. _adding-a-network:

Network
=======

Adding a network to Flotomate is an essential task for you to perform
asset Discovery and monitoring. We support Domain networks and IP Range
Networks.

.. note:: Managing Networks requires administrative rights.

**Adding a Network**

1. Log in to your Dashboard and head to **Admin** >> **Networks** (under
   IT Infrastructure).

2. Click the **Create a Network** button situated in the top right corner
   of the page. A dialog box opens.

.. _amf-163:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-163.png
    :align: center
    :alt: figure 163

.. _amf-164:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-164.png
    :align: center
    :alt: figure 164

3. Give a name to the network.

4. Add a Domain Network Type:

   We have two Domain Network Types to select from:

    a. Domain Network:

        +-----------------------------------+-----------------------------------+
        | Windows Domain Controller         | Windows Workgroup                 |
        +===================================+===================================+
        | It is a form of a computer        | It is a peer-to-peer network of   |
        | network in which all user         | computers running Windows OS.     |
        | accounts, computers, printers and |                                   |
        | other security principals, are    | Type in the common name of the    |
        | registered with a Domain          | Workgroup.                        |
        | Controller                        |                                   |
        |                                   | Select the credential of a remote |
        | Type the Domain Controller Name,  | computer in the network from the  |
        | something like company.com.       | Credential list.                  |
        |                                   |                                   |
        | Select the appropriate credential |                                   |
        | from the Credential list.         |                                   |
        +-----------------------------------+-----------------------------------+

    
    b. IP Range Network:

        +-----------------------------------+-----------------------------------+
        | Entire Network                    | This option uniquely identifies   |
        |                                   | an entire network with IP Range   |
        |                                   | Start (example: 192.168.27.0) and |
        |                                   | Subnet Mask (example:             |
        |                                   | 255.255.255.0).                   |
        +-----------------------------------+-----------------------------------+
        | Specific Range                    | You can specify an IP Range with  |
        |                                   | a start and end IP, and a Subnet  |
        |                                   | Mask.                             |
        +-----------------------------------+-----------------------------------+
        | Comma Separate IP List            | As the name suggests, you can add |
        |                                   | a comma-separated list of all the |
        |                                   | IPs.                              |
        +-----------------------------------+-----------------------------------+

5. Type in a description and protocol type (if IP Range is selected).
   We have two protocols to select from:

    +-----------------------------------+-----------------------------------+
    | DHCP                              | STATIC                            |
    +===================================+===================================+
    | In this protocol, IP is centrally | It uses static IP addresses to    |
    | allocated and resolved in your    | identify devices in the network.  |
    | network.                          |                                   |
    |                                   |                                   |
    | You have to configure your DNS    |                                   |
    | for asset Discovery to work.      |                                   |
    +-----------------------------------+-----------------------------------+

6. Add the necessary credentials from the credential list, or you can create new credentials using the
   **Add New Credential** option in :numref:`amf-163`. When you are done hit **Create**.

**Editing/Deleting Network**

Log in to your Dashboard and head to **Admin** >> **Networks**
(under IT Infrastructure).

.. _amf-165:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-165.png
    :align: center
    :alt: figure 165

This section lists all existing networks. Click the Edit Icon
adjacent to the network that you want to edit.

Edit the network in the Edit Network dialog box and save your
changes before exiting.

You can delete any network by clicking the Delete icon adjacent to the
network that you want to delete.