****************************************
Flotomate High Availability Server Setup
****************************************

What is High Availability Setup?
================================

High availability refers to the period of time when the (Service Desk)
service is available. The concept focuses on the maximum uptime of the
service by ensuring service and data recovery during an unplanned
disruption.

In a High Availability setup, there are three servers, the main server
is called the Master, the secondary server is called the Slave and
there’s an HA-proxy server.

Master is the main (Service Desk) server which is accessed by the users,
and the Slave remains idle. The database of the Master is
instantaneously replicated in the Slave. During a downtime, the Slave
becomes the Master with the same Database as the Master (Main Server).

Both Master and Slave are connected to the HA-proxy server. The proxy
server acts as a load balancer that redirects traffic to the Slave when
the Master is down.

Possible Use Cases of a High Availability Setup:

-  Maintaining availability of service during an unplanned shutdown of
   the Master (Main Server).

   For example, An organization maintaining an HA has to have two
   separate Servers, one for Master and other for Slave, this is to
   ensure that in an unforeseen event like a fire, natural calamity,
   etc. when the Master is down, the Slave can be kept alive from the
   last point of recovery.

   .. _ha-1:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-1.png
        :align: center
        :alt: figure 1

   **Note: A (Haproxy) load balancer redirects traffic to the Slave when
   the Master is down.**

-  High availability setup can be used for a planned outage of the
   Service Desk for the purpose of maintenance.

-  High Availability can be used in the event of a disaster recovery of
   data.

Setting up High Availability Servers
====================================

You have to install the product build in two separate servers (with
different environments), one as the Master and other as the Slave. Both
the servers have to have separate IP addresses.

The HA-proxy have to be installed in a separate server as well.

**Minimum System Requirements for Master and Slave Servers:**

-  4GB of System RAM.

-  Minimum Two Core Processor.

-  Minimum 100 GB of Hard disk space.

**Download of Base OS:**

You need Ubuntu-16.04.1 Server OS for this setup. Follow the link to
download the OS: `Download Link<https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/share/ubuntu_server_os.iso>`_

**Things to Know/Have before Installation:**
--------------------------------------------

-  Installation of the Master and Slave has to happen from the same
   build.

-  You will be asked for the IP of both Master and Slave during
   installation, so keep them handy.

-  Two Static IPs of Master and Slave server. Make sure both IPs are
   pingable when setting up HA.

Installation of Master and Slave
---------------------------------

1. Copy release build installer (service_desk_master_CI) to target
   machine.

2. Open terminal and navigate to the directory where the build is.

3. Make Sure you have the permission to execute the file. If there’s no
   permission then you can change it using the following command:

   **sudo chmod 777 service_desk_master_CI**

4. Run Installer by using the following command:

   **sudo ./service_desk_master_CI**

   .. _ha-2:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-2.png
        :align: center
        :alt: figure 2

   During Installation, Installer will prompt for Password. Please
   provide following password : mypassword.

   .. _ha-3:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-3.png
        :align: center
        :alt: figure 3

5. Since this is a High Availability setup for Master, we are going to
   choose option number of 2.

   .. _ha-4:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-4.png
        :align: center
        :alt: figure 4

6. The setup will ask for confirmation whether you want HA or not. Type
   y and enter.

7. The installation process will start. The setup will ask for the IP of
   the Master server. Provide the IP address and hit enter.

   .. _ha-5:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-5.png
        :align: center
        :alt: figure 5

   Then the setup will ask for the IP of the Slave server. Provide IP
   and hit enter.

   .. _ha-6:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-6.png
        :align: center
        :alt: figure 6

8. Wait for the installation process to finish. After the installation,
   wait for a couple of minutes for the Service Desk to go online.

9. Before beginning the installation of the Slave server, open the
   (Master) Service Desk using its IP address and Register the product.

   .. _ha-7:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-7.png
        :align: center
        :alt: figure 7

   .. note:: Before beginning the installation process of Slave, complete registration of Master and wait for five minutes.

10. Log into the Slave server (which is different from Master).The steps
    to install a Slave is same as :ref:`Master <Installation of Master and Slave>` up to step 4.

11. During installation, you will be asked whether you want HA or
    Standalone. Since this is an HA installation of Slave, select option
    3 and hit enter.

12. The setup will ask for confirmation; select y and hit enter.

13. Provide the IP addresses of Slave and Master during the
    setup.

    .. _ha-8:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-8.png
         :align: center
         :alt: figure 8

14. Now you will be prompted for the main-backup password which is:
    **aqwe123@** .

15. The database replication from the Master will begin. The
    installation will finish after DB replication. **This completes the
    setup of HA servers.**

    .. _ha-9:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-9.png
         :align: center
         :alt: figure 9

    .. _ha-10:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-10.png
         :align: center
         :alt: figure 10

Slave server will stay idle as long as the master is running. You can’t
access the slave using its IP address.

How to Maintain Database Replication When Master is Down
========================================================

In an event when Master shuts down, the Slave becomes active and becomes
the Master with all data from the last point of recovery at Master.

.. important:: It may happen that elastic search might not work in Slave server. 
               :ref:`Learn how to resolve this problem <Elastic Search not Working After Slave Becomes Master in a HA Setup.>`. 

.. important:: In case you want to restart a running master server, you have to make sure the associated slave server is shutdown
               in order to prevent an unwanted transition of a master to slave.            

The Slave becomes the new Master and the old Master stays idle. In order
to maintain HA of service and DB replication (for data recovery) an
Admin as to convert the old Master into the new Slave. Now the admin
will perform the following processes.

**Note: New Master IP: 192.168.0.118 and old Master IP: 192.168.0.137
(based on above HA Setup)**

.. note:: You have to work on both the servers as root users.

1. *Admin opens new Master(\ *\ **IP: 192.168.0.118**\ *) begins the
   process of converting old Master in New Slave. Admin changes the
   config_change.py file:*

   **cd /opt/flotomate/Restore/New\\ Master/**

   **python3 config_changes.py 192.168.0.118(new-master) 192.168.0.137(old-master)**

   .. _ha-11:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-11.png
        :align: center
        :alt: figure 11

2. Admin restarts PostgreSQL at New Master:

   **sudo systemctl restart postgresql**

4. Admin starts the restore_master.sh script file in old Master (**IP:
   192.168.0.137**):

   **cd /opt/flotomate/Restore/Prev\\ Master**

   **sudo sh restore_master.sh**

5. The old Master will ask for the new Master IP.

6. Now you will be prompted for the password which is: **aqwe123@.**

Now the old Master is the New Slave and the DB of new Master (old Slave)
will be replicated here.

.. _section-1:

Setting Up HA-Proxy Server (Optional)
=====================================

**Note: HAproxy is a popular open source load balancer. You can use any
other load balancer.**

A HAproxy (also known as a Load Balancer) is a solution to distribute a
web application across multiple servers. In the HA setup, a HAproxy
routes the traffic to the Slave server (after becoming a Master) when
the Master is down.

**Note: HA-proxy requires a separate IP . HAproxy is a separate server
from the Master and Slave**\ *.*

Installation of HA-proxy
------------------------

We will be using HAProxy 1.6 stable version for HA setup. Your server
needs to have an internet connection. Run the below commands from the
terminal.

| apt-get update
| apt-get install haproxy=1.6.\\*

.. _ha-12:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-12.png
    :align: center
    :alt: figure 12

HAproxy Setup
--------------

.. note:: First you need to install the HAproxy.

1. Log into the HAproxy server and open a terminal as root.

2. Now you have to configure the Configuration file of HAproxy using the
   following command.

   **sudo nano /etc/haproxy/haproxy.cfg**

   .. note:: you can use a different text editor to open the config file.

3. Copy paste the following at the end of the file and save it.

   .. _ha-13:

   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-13.png
        :align: center
        :alt: figure 13

4. Now you have to restart the HAproxy using the following command.

   .. _ha-14:
   
   .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/ha-setup/HA-14.png
        :align: center
        :alt: figure 14

