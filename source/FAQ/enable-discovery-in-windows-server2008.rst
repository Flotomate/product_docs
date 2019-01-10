********************************************************************
How to Enable Agent-less Network Discovery on Windows Server 2008 R2
********************************************************************

The network discovery is disable by default. When enabled it again switches back to off, because Network Discovery is dependent
on Windows services that can't be started. To resolve this issue follow the following steps:

1. Start services.msc
2. Make sure that the services below are set to startup type manual:
    a. Function Discovery Resource Publication
    b. SSDP Discovery
    c. UPnP Device Host
3. Go to Network and Sharing Center
4. Click Change advanced sharing settings
5. Select Turn on network discovery
6. Click Save changes