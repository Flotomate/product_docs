*****************************************************************************************************
Asset Discovery and Patch Management has Stopped Working after Migrating to HTTPS in the Main Server.
*****************************************************************************************************

The default port for the discovery service is http/80 which is different for the https/443. You have to redirect the service to
that port (https/443). 

Logging to the main server and apply the following commands to change the config file.

1. Command to open the config directory: ** cd /opt/flotomate/discovery-service/config**

2. Command to open the config file in the nano editor: **sudo nano service-conf.yaml** (You can use any other editor like Vim)

There, modify the highlighted link to https from http and port number to 443.  

.. _faq-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/faq/FAQ-4.png
    :align: center
    :alt: figure 4

Once the configuration is done, you have to restart the discovery process to put the changes in effect. Use the below command to
restart the discovery:

**sudo systemctl restart ft-discovery-service.service**