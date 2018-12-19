****************************
Reactivate License using API
****************************

The license of Flotomate ITSM is binding with the MAC address of the server. In an event where an admin decides to migrate our product to 
a different server, he will get an error of license not being enough. This error is due to the change in MAC address. 

In order to resolve the issue, the admin has to make an api call to **http://{product_ip}/api/ususer/activationcode** 
which will yield an activation key. He will give the activation key to us,
and we will use it to generate a new license. 

.. _keyapi-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/server-installation/KEYAPI-1.png
       :align: center
       :alt: figure 1 