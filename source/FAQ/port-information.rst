********************************************
What Ports are Required for Asset Discovery?
********************************************

The process of asset discovery involves a series of data exchanges between the main server and nodes in a network. 
It requires a certain set of ports to be open for discovery to work. Here are the ports which you need to allow for asset
discovery.

- ITSM Main Server: 

    a. DNS: 53
    b. SSH: 22
    c. SNMP: 161
    d. WMI: 135 & 445,  5000 - 6000(TCP), 49152 – 65535 (TCP) -Random ports once when ready for connection.
    e. LDAP: 389
    f. Discovery Server: 8081
    g. HTTP/HTTPS: 80/443
    h. Main-server: 8080
    i. RDP-Client: 7070
    j. RDP-Server: 5900
    k. SMPTP 25/465/587
    l. POP3: 995/110
    m. IMAP 993/143

- Plugin server ports for: 

    a. Plugin Server: 5050
    b. HTTP/HTTPS: 80/443

- Relay/File server ports for:

    a. File/Relay Server: 6060
    b. HTTP/HTTPS: 80/443

- Agent ports for: 

    a. HTTP/HTTPS: 80/443
