***************
Discovery Probe
***************

After setting up the Infrastructure, now it is the time for you to
create a Discovery Probe. A Discovery Probe is used in an Agentless
setup to discover Assets in a network. It runs processes to discover all
pingable workstations and devices in the network using the network
credentials and can generate reports based on the output. Other
capabilities that a Probe provides are: scheduling, Polling (detecting
changes in existing Assets), and Asset Review; these features help you
to make your Discovery operations smooth and manageable.

A Discovery Probe supports a wide range of network protocols to cover
maximum types of devices in a network.

.. note:: Creating Discovery Probe requires Administrative rights.

Creating a Discovery Probe
==========================

1. Log into the Motadata Dashboard.

2. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

.. _amf-166:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-166.png
    :align: center
    :alt: figure 166

3. The Discovery Probe page opens. Here you get to see all the existing
   probes. Click on **Create Discovery Probe** situated in the top
   right corner of the page. Create Discovery Probe dialog box opens.

.. _amf-167:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-167.png
    :align: center
    :alt: figure 167

4. The Create Discovery Probe dialog box has four fields (refer :numref:`amf-166`):

    a. Section-A: You enter a Name for the Probe here. By default, you
       see the keyword Prob followed by the Date and Time. You can
       change the default name to anything.

    b. Section-B: Enter a description of the Probe here.

    c. Section C: Depending on what you want to discover or scan, you
       have to select a Network Type: Domain Network or IP Range
       Network.

       i.  Domain Network: This type is used to discover or scan
           Windows workstations either under a Domain Controller or
           in a Windows Workgroup.

       ii. IP Range Network: This type is used to discover or scan
           all workstations (UNIX & Windows-based machines), network
           devices and other pingable Assets.

    d. Section-D: While setting up the Infrastructure you must have
       added your network/networks. Those networks appear as a drop-down
       list filtered by the Network Type you have selected. The Probe
       acquires the network properties from the selected network.

5. Once you are done, click on **Create**. You have successfully
   created a Discovery Probe. There is no limit to the number of Probes
   that you can create.

Information Fetched by a Probe
==============================

The Probe fetches the following data points from a workstation (subject to change in subsequent product updates):

.. note:: Assets having UUID as 00000000000 can also get discovered.

-  General Details:

   a. Name and ID

   b. Asset Type

   c. Status

   d. Used By

   e. Department

   f. IP

   g. Host Name

- OS Name and Version

- Service Pack Name

- Memory Size

- Disk Size/Information

- CPU Speed

- CPU Core Count

- MAC Address

- Domain Name

- Serial Number

- Processor Information

- Network Adapter Information

- Monitor Information

- Mouse and Keyboard

- Logical Disk Information

- Physical Disk Information

- Last Audit Date