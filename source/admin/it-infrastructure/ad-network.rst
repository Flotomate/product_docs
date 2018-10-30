*******
Network
*******

Adding a Network allows the product to perform the following things:

-  Asset discovery and monitoring.

-  Remote deployment of Patches and Packages.

.. note:: Managing Networks requires administrative rights.

Add a Network
=============

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