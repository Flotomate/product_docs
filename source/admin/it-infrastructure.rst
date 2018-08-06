*****************
IT Infrastructure
*****************

Getting Started with Email Setup
================================

Setting up an email server and linking that with the product allows the
product to send and receive emails.

Some of the capabilities that the product get after email setup are:

-  Requestors can log tickets using email.

-  The product can send :ref:`Email
   Notifications <setting email notifications>` and Announcements.

-  Technicians can change Request details using :ref:`Email
   Commands <email command settings>`.

Whether self-hosted or cloud-hosted, you can add any vanity email
address to Flotomate using any one of the two email protocols: POP3 and
IMAP.

.. note:: Before configuring email, you have to create an email with your
          email host and make sure to enable the protocol you want to use (POP3 or
          IMAP).

.. note:: You need administrative rights to set the email configuration.

Email Server Configuration
--------------------------

-  Log in to your Dashboard and head to **Admin** from the Navigation
   Tabs. Use the search field, or you can find the Email Server
   Configuration under IT Infrastructure.

.. _adf-61.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-61.1.png
    :align: center
    :alt: figure 61.1

.. _adf-61.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-61.2.png
    :align: center
    :alt: figure 61.2

-  On clicking, you see the **Email Server Configuration** page. Your
   email host provides you with all the information needed to complete
   the process.

-  A summary of the required information:

    +-----------------------------------+-----------------------------------+
    | Outgoing Server                   | This is the hostname of your      |
    |                                   | outgoing SMTP server. For         |
    |                                   | example, the hostname of Google’s |
    |                                   | outgoing SMTP is smtp.gmail.com   |
    +===================================+===================================+
    | Outgoing Port                     | It refers to the outgoing port    |
    |                                   | number of the SMTP server.        |
    +-----------------------------------+-----------------------------------+
    | Outgoing Email                    | The outgoing email address.       |
    +-----------------------------------+-----------------------------------+
    | Outgoing Username                 | Username of the outgoing email    |
    |                                   | address.                          |
    +-----------------------------------+-----------------------------------+
    | Outgoing Password                 | Password of the outgoing email    |
    |                                   | address.                          |
    +-----------------------------------+-----------------------------------+
    | Outgoing Security Type            | Please refer to your email server |
    |                                   | specification to know what        |
    |                                   | security standards it supports.   |
    |                                   | Currently, we support TLS and     |
    |                                   | SSL.                              |
    +-----------------------------------+-----------------------------------+
    | Incoming Server                   | This is the hostname of your      |
    |                                   | incoming mail server. For         |
    |                                   | example, the hostname of Google’s |
    |                                   | incoming POP3 server is           |
    |                                   | pop.gmail.com and for IMAP        |
    |                                   | server, imap.gmail.com            |
    +-----------------------------------+-----------------------------------+
    | Incoming Port                     | It refers to the incoming port    |
    |                                   | number of the mail server.        |
    +-----------------------------------+-----------------------------------+
    | Incoming Email                    | The incoming email address.       |
    +-----------------------------------+-----------------------------------+
    | Incoming Password                 | Password of the incoming email    |
    |                                   | address.                          |
    +-----------------------------------+-----------------------------------+
    | Incoming Security Type            | Please refer to your email server |
    |                                   | specification to know what        |
    |                                   | security standards it supports.   |
    |                                   | Currently, we support TLS and     |
    |                                   | SSL.                              |
    +-----------------------------------+-----------------------------------+
    | Incoming Protocol                 | POP3 or IMAP                      |
    +-----------------------------------+-----------------------------------+
    | Incoming Supportidle              | Disable/Enable IMAP IDLE support  |
    +-----------------------------------+-----------------------------------+

-  After filling the fields, you can test the connection between the
   server and Flotomate using **Test Connection**. Flotomate warns you
   in case of a connection error.

-  Add any email addresses that you want to ignore (don’t want to
   receive emails from) in the **Ignore Email Addresses** field. Use
   **Update** to save your changes.

Flotomate gives you two email fields one for outgoing and the other for
incoming. If you want, you can use two different addresses for outgoing
and incoming. You can use the **Email Server Configuration** page to
edit your settings later.

Enabling Email to Ticket
------------------------

The Email to Ticket feature allows users to create a Request by sending
an email to the incoming email ID of the product.

The subject of the email becomes the subject of the Request and the body
becomes the Description. Whether only registered users can send or
everyone depends on the **Allow to report Request without login** option
in **Admin** >> **Helpdesk Security**.

To enable this feature:

-  Go to **Admin** >> **Email Server Configuration** (IT
   Infrastructure).

-  There turn on the toggle **Enable Email to Ticket**.

-  The Category field specifies the default category applied to Requests
   created via email.

.. _adf-62:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-62.png
    :align: center
    :alt: figure 62

DNS Configuration:
==================

Some email notifications have links to the product. The URL of the
product is appended to such links from the DNS Configuration.

The DNS configuration is also used in resolving hostnames of Assets
against their IPs from the DNS when the network protocol is DHCP.

In the DHCP protocol, the IPs of Assets keep on changing, so the
hostname of a machine is taken as the unique identifier. The DNS maps
all the hostnames of the Assets with their IP addresses. Flotomate
connects with the DNS using the information provided by the
administrator in the DNS Configuration page (Primary DNS and Secondary
DNS) during polling (scanning of existing Assets).

.. note:: Setting DNS configuration requires you to have administrative rights.

Configuring DNS
---------------

-  Log in to your Dashboard and head to **Admin** from the Navigation
   Tabs. Use the search, or you can find the **DNS Configuration** in IT
   Infrastructure.

.. _adf-63:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-63.png
    :align: center
    :alt: figure 63

-  On clicking **DNS Configuration**, you see the DNS Configuration
   page.

-  Enter your primary DNS address in the primary field and your backup
   DNS address in the secondary field.

-  The Base URL field is the domain name of Flotomate hosted on your
   servers. Enter the name and hit **Update** to save your changes.

You can later edit your DNS configuration in the DNS Configuration page.

Credential Library
==================

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
--------------

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

Network
=======

Adding a Network allows the product to perform the following things:

-  Asset discovery and monitoring.

-  Remote deployment of Patches and Packages.

.. note:: Managing Networks requires administrative rights.

Add a Network
-------------

1. Log in to your Dashboard and head to **Admin** >> **Networks** (IT
   Infrastructure).

2. Click the **Create a Network** icon situated in the top right corner
   of the page. Create a Network dialog box opens.

.. _adf-69:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-69.png
    :align: center
    :alt: figure 69

.. _adf-70:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-70.png
    :align: center
    :alt: figure 70

3. Give a name to the network.

4. You can associate the Network to a department.

5. Add a Domain Network Type:
   We have two Domain Network Types to select from:

    a. Domain Network:

        +-----------------------------------+-----------------------------------+
        | Windows Domain Controller         | .Windows Workgroup                |
        +===================================+===================================+
        | -  Type the Domain Controller     | -  It is a peer-to-peer network   |
        |    Name, something like           |    of computers running Windows   |
        |    company.com.                   |    OS. Type in the common name of |
        |                                   |    the Workgroup.                 |
        | -  Select the appropriate         |                                   |
        |    credential from Credential     | -  Select the credential of a     |
        |    list.                          |    remote computer in the network |
        |                                   |    from Credential list.          |
        +-----------------------------------+-----------------------------------+

    p. IP Range Network:

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

6. Type in a description and protocol type (if IP Range is selected).

    a. We have two protocols to select from:

        +-----------------------------------+-----------------------------------+
        | DHCP                              | STATIC                            |
        +===================================+===================================+
        | -  In this protocol, IP is        | -  Using static IP addresses to   |
        |    centrally allocated and        |    identify devices in the        |
        |    resolved in your network.      |    network.                       |
        |                                   |                                   |
        | -  You have to configure your DNS |                                   |
        |    for asset Discovery to work.   |                                   |
        +-----------------------------------+-----------------------------------+

7. Add the necessary credentials from the credential list, or you can create new credentials using the
   **Add New Credential** option in :numref:`adf-69`. When you are done hit **Create**.

**Edit/Delete Network**

1. Log in to your Dashboard and head to **Admin** >> **Networks** (IT
   Infrastructure).

.. _adf-71:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-71.png
    :align: center
    :alt: figure 71

2. All your networks are listed on this page. Click the Edit Icon
   adjacent to the network that you want to edit.

3. Edit the network in the Edit Network dialog box and save your change
   before exiting.

You can delete any network by clicking the Delete Icon adjacent to the
network that you want to delete.

Proxy Server Configuration
==========================

If you want the product to have access to the internet, then you can
setup a proxy server or give the product direct access.

Some of the benefits of Proxy configured:

-  Control of patch downloading from update servers in Remote
   Deployment.

-  Protects the tool from direct access.

To configure Proxy Server:

-  Go to **Admin** >> **Proxy Server Configuration** (IT
   Infrastructure).

.. _adf-72:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-72.png
    :align: center
    :alt: figure 72

-  In the new page, you get three options:

   a. No Internet Access

   b. Direct Internet Access

   c. **Configure Manually** (Connection via proxy server): You require
      the following information to set up a proxy connection:

      i.   Proxy host

      ii.  Port number of the proxy server.

      iii. Credentials to access proxy server (Username and Password)

-  Save your changes using the **Update** button.

LDAP Configuration
==================

Flotomate allows batch upload of **Requestors** from an LDAP request.
LDAP is a protocol used by enterprises to access an Active Directory of
their employees. It is mainly used for email clients and other contact
search programs.

Flotomate establishes a connection with a distributed directory
information system using the user provided information, and it makes
queries using the LDAP protocol. It fetches the employee details from
the server into the product.

Configure LDAP:
---------------

1. Go to **Admin** >> **LDAP Configuration** (IT Infrastructure).

2. LDAP Configurations page opens. Here you can see all your existing
   LDAP servers if any. Click **Add LDAP Configuration** situated in the
   top right corner. You get the following dialog box:

..

.. _adf-73:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-73.png
    :align: center
    :alt: figure 73

.. _adf-74:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-74.png
    :align: center
    :alt: figure 74

3. Please refer :numref:`adf-73`. Give a name to the server. URL (field A) is
   the URL of the LDAP server which begins with ldap:// (ldaps:// if the
   connection is secured) followed by protocol components (IP address,
   and port number). A valid URL should look something like
   ldap://111.111.0.11:920. Base DN (field B) is an API reference for
   the LDAP object; basically, it tells us what to fetch from where to
   fetch from the LDAP server. Put you LDAP credentials in the User ID
   (field C) and Password (field D).

4. Please refer :numref:`adf-74`. Switch to the Mapping section of the dialog
   box. Here you have to enter the LDAP object attributes. There are
   two pre-defined fields (Name and Email). You can add more fields
   using the :doc:`Requestor Custom Field <admin-customization>` option. You can edit and delete a
   custom field in the :doc:`Custom Field <admin-customization>` section of Admin.

5. Hit **Add** to save your LDAP server.

The credentials required for LDAP configuration are of the LDAP Admin.
In case, credentials are not available then a new user can be created in
their Active Directory. Please refer the document LDAP Configuration by
Creating New User.

Edit LDAP Server
----------------

1. Open LDAP Configurations page and select the server that you want to
   edit.

.. _adf-75:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-75.png
    :align: center
    :alt: figure 75

2. Click **Edit** from the right-side details pane. The Edit LDAP
   Configuration dialog box opens. Make the changes and hit **Update**.

Please refer :numref:`adf-13`. Go to the LDAP Configurations page and select
the server name that you want to delete and click on Action Menu. Click
on **Delete** from the pop-up menu. On confirmation, the server gets
deleted.

LDAP Connection Test
--------------------

In the LDAP Configurations page, you can check an LDAP server’s
connection with the product by using the **Test Connection** option in
:numref:`adf-75`.

Setting LDAP Import Schedule
----------------------------

Scheduling allows you to periodically import employee details from the
server. This feature helps you to keep the Requestor list up to date.

.. _adf-76:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-76.png
    :align: center
    :alt: figure 76

1. Open **LDAP Configurations** page and select the server that you want
   to schedule an import. Under **Import Schedule**, set a schedule
   cycle for importing the Requestors. Flotomate offers three options:
   Daily, Weekly, and Monthly.

   a. Importing daily requires a start date and time; after that, the
      importing happens every day at the set time.

   b. Importing weekly requires you to set the days in a week on which
      the importing happens.

   c. Importing monthly requires you to set a day of the month and the
      months in which the importing happens.

2. After setting the schedule, hit **Save Schedule** to save your
   changes.

Edit/ Disable LDAP Schedule
---------------------------

You can later edit the schedule using the **Edit Schedule** option. The
Scheduled toggle turns on/off a schedule.

.. _adf-77:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-77.png
    :align: center
    :alt: figure 77
