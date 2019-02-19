*****************************************************************************************************
Asset Discovery and Patch Management has Stopped Working after Migrating to HTTPS in the Main Server.
*****************************************************************************************************

The default port for the discovery service is http/80 which is different for the https/443. You have to redirect the service to
that port (https/443). 

Logging to the main server and open the config file using the following command.

**/opt/flotomate/discovery-service/config/service-conf.yaml**

There, modify the port number to 443. 

.. _faq-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/faq/FAQ-4.png
    :align: center
    :alt: figure 4