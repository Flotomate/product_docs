*****************
DNS Configuration
*****************

Some email notifications have links to the product. The URL of the
product is appended to such links from the DNS Configuration.

The DNS configuration is also used in resolving hostnames of Assets
against their IPs from the DNS when the network protocol is DHCP.

In the DHCP protocol, the IPs of Assets keep on changing, so the
hostname of a machine is taken as the unique identifier. The DNS maps
all the hostnames of the Assets with their IP addresses. Motadata
connects with the DNS using the information provided by the
administrator in the DNS Configuration page (Primary DNS and Secondary
DNS) during polling (scanning of existing Assets).

.. note:: Setting DNS configuration requires you to have administrative rights.

Configuring DNS
===============

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

-  The Base URL field is the domain name of Motadata hosted on your
   servers. Enter the name and hit **Update** to save your changes.

You can later edit your DNS configuration in the DNS Configuration page.