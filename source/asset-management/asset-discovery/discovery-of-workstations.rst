***************************************************
Discovery of Workstations and Other Network Devices
***************************************************

Motadata aims to give maximum flexibility in ways to Discovery Assets
in a network. Our product can discover all pingable IT Assets in or
outside a network. We support Assets Discovery in Windows Domain and IP
Range Networks, and we also have an Agent Application for Assets that
are not part of any network/domain.

**Discovery Mechanism Overview?**

-  Domain Network Discovery detects all Windows workstations and servers
   that are:

   a. Part of a Windows Domain and uses Active Directory.

   b. Part of a Windows Workgroup.

-  IP Range Network Discovery detects all workstations and servers
   within a range and supports:

   a. UNIX (Using SSH) and Windows-based systems (Using WMI).

   b. Workstations (Windows) that are part of a Windows workgroup.

   c. Pingable devices like network routers, printers, access points,
      etc. Using the SNMP protocol.

-  Our Agent Application can fetch data from workstations, which aren’t
   part of any network/domain, remotely. It is a lightweight application
   that runs in the background of a workstation as a service, acquires
   the data and pushes directly to the main server.

The first part of discovering Assets in Motadata (without using an
Agent) is to set up the infrastructure and then to create a Discovery
Probe. Once you create a Discovery Probe, you can Schedule Discoveries
and even discover changes in existing recognized Assets.

.. note:: You need Administrative rights to set up the infrastructure for Asset Discovery and 
          Domain rights to discover the target Domain.

.. note:: Present supported credentials are WMI, SSH, SNMP, and SNMP V3.