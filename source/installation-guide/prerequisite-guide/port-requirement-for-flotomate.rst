******************************
Port Requirement for Flotomate
******************************

Port serves as an interface between one computer and other computers. When setting up our product, opening the right ports is
vital for the proper functioning of our ITSM solution. Following are ports for all the services in Flotomate ITSM.

- Main Server
    1. Http/Https     80/443
    2. DNS            53
    3. SSH            22
    4. SNMP           161
    5. WMI            135 & 445, 5000 - 6000 (TCP), 49152 – 65535 
    6. LDAP           389
    7. Discovery      8081
    8. Main-server    8080
    9. RDP-Client     7070
    10. RDP-Server    5900
    11. SMTP          25/465/587 (could be any one)
    12. POP3          995/110 (based on default setup)
    13. IMAP          993/143 (based on default setup)
    14. ARP           219
    15. TCP           Random ports once when ready for connection. These are dynamic port range.
    16. LDAPS         636
- Plugin server
    1. Plugin server  5050
    2. Http/Https     80/443
- Relay/File Server
    1. File/Relay Server  6060
    2. Http/Https         80/443
- Agent
    1. Http/Https         80/443