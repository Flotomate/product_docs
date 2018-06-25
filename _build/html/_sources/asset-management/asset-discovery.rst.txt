***************
Asset Discovery
***************

Discovery of Workstations and Other Network Devices
===================================================

Flotomate aims to give maximum flexibility in ways to Discovery Assets
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

The first part of discovering Assets in Flotomate (without using an
Agent) is to set up the infrastructure and then to create a Discovery
Probe. Once you create a Discovery Probe, you can Schedule Discoveries
and even discover changes in existing recognized Assets.

.. note:: You need Administrative rights to set up the infrastructure for Asset Discovery and 
          Domain rights to discover the target Domain.

.. note:: Present supported credentials are WMI, SSH, SNMP, and SNMP V3.

Understanding Agent-Based vs. Agentless Method
----------------------------------------------

These two methods of discovering Asset can be compared with Push vs.
Pull. In Agentless Discovery, the Discovery engine scans a given network
for pingable Assets and populate the same in the CMDB. In Agent-Based,
every node of the network must run an Agent Application which
continuously streams the relevant data back to the server. As a best
practice, Assets which are frequently moved in the context of a
corporate network there Agent-based discovery and polling make more
sense. Whereas, Agent-less is the only way for scanning SNMP assets like
a printer, router, switches, etc.

Below are six dimensions that highlight the fundamental differences
between Agent-Based and Agentless scanning:

+-----------------------+-----------------------+-----------------------+
|                       | Agent-Based           | Agentless             |
+=======================+=======================+=======================+
| Discovery Method      | Agent-Based Discovery | Agentless Discovery   |
|                       | is a push-based       | is a pull-based       |
|                       | strategy, where every | approach, which is    |
|                       | node in a network     | designed to leverage  |
|                       | runs an Agent         | a network either      |
|                       | Application. The      | defined by a domain   |
|                       | Application pushes    | or an IP range.       |
|                       | the data into the     |                       |
|                       | main server.          | It uses network and   |
|                       |                       | management protocols  |
|                       | It does not have any  | like SNMP, WMI, etc.  |
|                       | network or domain     |                       |
|                       | barriers.             |                       |
+-----------------------+-----------------------+-----------------------+
| Deployment            | Running Agent-Based   | Agentless Discovery   |
|                       | Discoveries in        | requires one-time     |
|                       | multiple workstations | configuration of a    |
|                       | require the           | network in the main   |
|                       | individual            | server. Once a user   |
|                       | installation of the   | configures a network, |
|                       | Application. In case  | the user can create a |
|                       | the workstations are  | Discovery Probes.     |
|                       | part of a network, an |                       |
|                       | administrator can     |                       |
|                       | remotely install the  |                       |
|                       | application on all    |                       |
|                       | the workstations.     |                       |
+-----------------------+-----------------------+-----------------------+
| Device Coverage       | Currently,            | In an Agentless       |
|                       | Agent-Based scanning  | setup, the product    |
|                       | supports the          | scans Assets that     |
|                       | Discovery of Windows  |                       |
|                       | and Linux machines.   | following credential  |
|                       |                       | types:                |
|                       |                       |                       |
|                       |                       | -  WMI (Windows       |
|                       |                       |    Management         |
|                       |                       |    Instrumentation)   |
|                       |                       |                       |
|                       |                       | -  SSH                |
|                       |                       |                       |
|                       |                       | -  SNMP               |
|                       |                       |                       |
|                       |                       | -  SNMP V3            |
+-----------------------+-----------------------+-----------------------+
| Maintenance           | The Agent Application | No maintenance needed |
|                       | requires maintenance  | at the level of a     |
|                       | in the form of        | node.                 |
|                       | patches and updates   |                       |
|                       | at the node level.    |                       |
+-----------------------+-----------------------+-----------------------+

**Which one is better, Agentless or Agent-Based?**

It depends upon your requirement. Both Agent-Based and Agentless
Discovery are similar in their capabilities and scale. The differences
are in the way they function and their scope.

Infrastructure Setup
--------------------

Setting up the Infrastructure is the first step before Asset Discovery.
This step is prerequisite for Agentless Discovery of Assets, but not for
the Agent Application.

.. note:: Setting up the Infrastructure requires Administrative rights.

The Infrastructure Setup consists of three broad sections:

-  DNS Configuration:

-  Credential Library:

-  Networks:

DNS Configuration:
^^^^^^^^^^^^^^^^^^

The DNS configuration helps the product in resolving hostnames of Assets
against their IPs from the DNS. A DNS is useful especially when the
network protocol is DHCP.

In DHCP protocol, the IPs of Assets keep on changing, so the hostname of
a machine is taken as the unique identifier. The DNS maps all the
hostnames of the Assets with their IP addresses. Flotomate connects with
the DNS using the information provided by an administrator in the DNS
Configuration page.

.. note:: DNS configuration requires you to have administrative rights.

**Configuring DNS**

1. Log in to your Dashboard and head to **Admin** from the Navigation
   Tabs. Use search, or you can find the **DNS Configuration** in IT
   Infrastructure.

.. _amf-156:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-156.png
    :align: center
    :alt: figure 156

2. The DNS Configuration page opens. Click on **Edit** to make the
   fields editable.

3. Enter your primary DNS address in the primary field and your backup
   DNS address in the secondary field.

4. The Base URL field is the domain name of Flotomate hosted on your
   server. Enter the name and hit Update to save your changes.

You can later edit your DNS configuration in the DNS Configuration page.

Credential Library
^^^^^^^^^^^^^^^^^^

Flotomate provides an interface to upload all your credentials, so our
product can authenticate for an authorized access to a network.

A repository stores all Credentials, which we call a library where you
can manage (add, edit and delete) them.

We provide four easy Discovery Types to choose from:

-  WMI

-  SSH

-  SNMP

-  SNMP V3

.. note:: Managing credentials requires administrative rights.

**Adding Credential**

1. Go to **Admin** (One of the Navigation Tabs)>> **Credential Library**
   (under IT Infrastructure). The Credentials page opens where you can
   view all existing credentials.

2. Click the **Add Credential** situated in the top right corner of the
   page. The Add Credential dialog box opens.

.. _amf-157:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-157.png
    :align: center
    :alt: figure 157

3. Add a **Name** to the credential and select a Discovery Type which
   determines the authentication parameters. Now let’s understand the
   available Discovery Types:

    **WMI (Windows Management Instrumentation):**

    .. note:: Please refer to :numref:`amf-157`.

    This protocol is used to scan for data in Windows-based systems
    within a Domain or Workgroup.

        a. **Domain Username & Password**: These are credentials of the
           Administrator Account that has access to all the nodes in the
           domain.

        b. **Domain Name**: The part of a network address which identifies
           it as belonging to a particular domain.

        c. **Domain Discovery**: Enabling this marks the credential as
           discoverable. It means that the credential is for Discovery.
 
    **SSH (Secure Shell):**

    The SSH protocol is used to discover UNIX based machines.

        .. _amf-158:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-158.png
            :align: center
            :alt: figure 158

        a. **Domain Username & Password**: These are the credentials for the
           user account specific to the Asset that we are going to discover. In
           case there are multiple machines, a common user can be created (with
           root access) in all the machines to make discovery easy; else, each
           different account would require a separate SSH credential.

    **SNMP (Simple Network Management Protocol)**

    Flotomate uses this application-layer protocol to scan devices with
    the SNMP agent in a managed network.

        .. _amf-159:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-159.png
            :align: center
            :alt: figure 159

        a. **Community String**: The Community String acts as a password in a
           managed network. It is sent along with each SNMP Get-Request to gain
           access to an SNMP enabled device’s data. If the community string is
           correct, the get request fetches the data.

    **SNMP V3 (Simple Network Management Protocol Version 3):**

    It is a secure version of SNMP with user-based authentication.

        .. _amf-160:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-160.png
            :align: center
            :alt: figure 160

        a. **Community String**: It is like a password which is used for
           authentication.

        b. **Authentication Protoco**\ l: Use the protocol that you want to use
           (we support both MD5 and SHA) in field-A (:numref:`amf-160`).

        c. **Username**: Enter your username.

        d. **Auth Passphrase**: This is the Auth password

        e. **Privacy Passphrase**: This is the Privacy password.

        f. **Security Level**: Choose an appropriate security level from the
           following options:

            i. **Private Authentication**: Uses protocols like SHA for
               authentication and protocols like AES for privacy.

            ii. **No Private Authentication**: only use authentication
                protocol.

            iii. **No Private No Authentication**: Data transfer with
                 authentication and privacy.

**Testing Connection**

.. role:: red
You can test the credential by connecting with a computer (:red:`works for WMI and SSH credentials`). Click on
**Test Connection** next to **Save**. A dialog box opens asking for the
IP of the machine. Submitting an IP starts a process that tells whether
a successful connection was established or not.

.. _amf-161:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-161.png
    :align: center
    :alt: figure 161

**Editing/Deleting Credentials**

1. Go to **Admin** >> **Credential Library** (under IT Infrastructure).

.. _amf-162:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-162.png
    :align: center
    :alt: figure 162

2. Click the edit icon adjacent to the credential you want to edit. You
   see the Edit Credential dialog box. Make your changes and hit
   **Update**.

3. You can delete any credential by clicking the Delete icon adjacent
   to a credential.

Network
^^^^^^^

Adding a network to Flotomate is an essential task for you to perform
asset Discovery and monitoring. We support Domain networks and IP Range
Networks.

.. note:: Managing Networks requires administrative rights.

**Adding a Network**

1. Log in to your Dashboard and head to **Admin** >> **Networks** (under
   IT Infrastructure).

2. Click the **Create a Network** button situated in the top right corner
   of the page. A dialog box opens.

.. _amf-163:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-163.png
    :align: center
    :alt: figure 163

.. _amf-164:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-164.png
    :align: center
    :alt: figure 164

3. Give a name to the network.

4. Add a Domain Network Type:

   We have two Domain Network Types to select from:

    a. Domain Network:

        +-----------------------------------+-----------------------------------+
        | Windows Domain Controller         | Windows Workgroup                 |
        +===================================+===================================+
        | It is a form of a computer        | It is a peer-to-peer network of   |
        | network in which all user         | computers running Windows OS.     |
        | accounts, computers, printers and |                                   |
        | other security principals, are    | Type in the common name of the    |
        | registered with a Domain          | Workgroup.                        |
        | Controller                        |                                   |
        |                                   | Select the credential of a remote |
        | Type the Domain Controller Name,  | computer in the network from the  |
        | something like company.com.       | Credential list.                  |
        |                                   |                                   |
        | Select the appropriate credential |                                   |
        | from the Credential list.         |                                   |
        +-----------------------------------+-----------------------------------+

    
    b. IP Range Network:

        +-----------------------------------+-----------------------------------+
        | Entire Network                    | This option uniquely identifies   |
        |                                   | an entire network with IP Range   |
        |                                   | Start (example: 192.168.27.0) and |
        |                                   | Subnet Mask (example:             |
        |                                   | 255.255.255.0).                   |
        +-----------------------------------+-----------------------------------+
        | Specific Range                    | You can specify an IP Range with  |
        |                                   | a start and end IP, and a Subnet  |
        |                                   | Mask.                             |
        +-----------------------------------+-----------------------------------+
        | Comma Separate IP List            | As the name suggests, you can add |
        |                                   | a comma-separated list of all the |
        |                                   | IPs.                              |
        +-----------------------------------+-----------------------------------+

5. Type in a description and protocol type (if IP Range is selected).
   We have two protocols to select from:

    +-----------------------------------+-----------------------------------+
    | DHCP                              | STATIC                            |
    +===================================+===================================+
    | In this protocol, IP is centrally | It uses static IP addresses to    |
    | allocated and resolved in your    | identify devices in the network.  |
    | network.                          |                                   |
    |                                   |                                   |
    | You have to configure your DNS    |                                   |
    | for asset Discovery to work.      |                                   |
    +-----------------------------------+-----------------------------------+

6. Add the necessary credentials from the credential list, or you can create new credentials using the
   **Add New Credential** option in :numref:`amf-163`. When you are done hit **Create**.

**Editing/Deleting Network**

Log in to your Dashboard and head to **Admin** >> **Networks**
(under IT Infrastructure).

.. _amf-165:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-165.png
    :align: center
    :alt: figure 165

This section lists all existing networks. Click the Edit Icon
adjacent to the network that you want to edit.

Edit the network in the Edit Network dialog box and save your
changes before exiting.

You can delete any network by clicking the Delete icon adjacent to the
network that you want to delete.

Discovery Probe
---------------

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
^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Log into the Flotomate Dashboard.

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
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The Probe fetches the following data points from a workstation (subject to change in subsequent product updates):

-  General Details:

   a. Name and ID

   b. Asset Type

   c. Status

   d. Used By

   e. Department

   f. IP

   g. Host Name

-  OS Name and Version

-  Service Pack Name

-  Memory Size

-  Disk Size

-  CPU Speed

-  CPU Core Count

-  MAC Address

-  Domain Name

-  Serial Number

-  Processor Information

-  Network Adapter Information

-  Logical Disk Information

-  Last Audit Date

Managing a Discovery Probe
--------------------------

The Agentless method uses a Discovery Probe for discovery. Once you
create a Probe, you can start Discovering Assets and can generate
reports based on the output of a Discovery operation.

New Assets can be added automatically to the CMDB during a Discovery
operation and kept up to date by scheduling a process called
`Polling <#run-on-demand-polling>`__ that retrieves any changes at the
source.

Using Scheduling, you can even automate the Discovery process. You can
review the discovered Assets before committing them to the CMDB.

Run on Demand Discovery
^^^^^^^^^^^^^^^^^^^^^^^

The fastest way to initiate a Discovery is to use the **Scan New Assets** option
in a Probe:

1. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

2. Select a Probe. The **Scan New Assets** option appears.

3. Click on **Scan New Assets** and it asks whether you want to add the Assets
   automatically or not. In response, the discovery process begins. The
   Status changes to FINISHED when done. Along with that it also shows
   the date and time of completion of the discovery.

    .. _amf-168:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-168.png
        :align: center
        :alt: figure 168

   During discovery, you can view the `progress <#statusprogress-of-a-probe>`__ under the Discovery tab.

4. All discovered Assets are added to the Asset List View; there you
   can view them and can perform other operations. If you did not
   select automatic addition to the CMDB, then discovered Assets are
   staged for `review <#reviewing-discovered-assets>`__; from there you
   have to commit them to the CMDB. You can view the Assets that are currently staged
   by clicking on the **View Assets in Stage** button under the Status tab.

.. _amf-169:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-169.png
    :align: center
    :alt: figure 169

Run on Demand Polling
^^^^^^^^^^^^^^^^^^^^^

Polling detects any changes made to a discovered Asset at the source and
pushes the changes (if any) to the CMDB. This process helps you to keep
your CMDB up to date. The fastest way to initiate Polling is to use the
**Scan Existing Assets** option.

1. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

2. Select a Probe. The **Scan Existing Assets** option appears.

3. Click on **Scan Existing Assets** and it asks for confirmation. On a
   positive response, the polling process begins. The Status changes to
   FINISHED when done. Along with that it also shows the date and time
   of completion of the polling.

.. _amf-170:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-170.png
    :align: center
    :alt: figure 170

Scheduling
^^^^^^^^^^

The Probe allows you to perform periodic scans using the Schedule
function. It is a powerful feature to automate your Discovery process.
You can Schedule both Discovery and Polling.

**Scheduling a Discovery:**

.. note:: You need to first create a Probe before you can use scheduling.

1. Log into the Flotomate Dashboard.

2. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

.. _amf-171:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-171.png
    :align: center
    :alt: figure 171

3.  Click on a probe. The color changes to dark blue. The Details Pane
    is visible on the right side of the probe list.

4. Click on the **Discovery tab**. You see “No-schedule-created”
   message if you are scheduling for the first time. Click on
   **Schedule** to create one.

.. _amf-172:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-172.png
    :align: center
    :alt: figure 172

5. Refer :numref:`amf-171`. There are three fields in Schedule that you need
   to fill:

    a. Field-A talks about the frequency of scheduled Discovery that
       you want. You get the following options:

        i. **Once**: Discovery happens only once at a specific
           date and time.

        ii. **Daily**: The Discovery Schedule activates on a start
            date & time. After that, the Discovery happens every
            day at a specified time mentioned in the Hour and
            Minute field.

        iii.  **Weekly**: Discovery happens on a specific day/days of
              a week.

        iv.  **Monthly**: Discovery happens in selected month/months
             of a year on a particular day.

    b. In Field-B, if you want the discovered Assets directly to be
       added to the CMDB then select **Yes,** else **No** if you want
       to review the Assets and add them yourself.

    c. Field-C is where you can enter one or more email addresses to
       send them discovery reports. After every successful Discovery,
       the system generates a report detailing about the discovered
       Assets. You can add as many email addresses you want. The report
       looks something like this:

.. _amf-173:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-173.png
    :align: center
    :alt: figure 173

6. Select the options and complete the fields, and hit **Save
   Schedule** to start the Schedule.

**Scheduling a Polling**

The process of scheduling a Polling operation is similar to Discovery
except the **Automatically Add Asset in Store** option is not present in
Polling.

The **Schedule** option can be found in the **Polling** tab.

Editing a Schedule for Discovery and Polling
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

You can easily edit the parameters of a set Schedule: you can change the
frequency, review settings and add/subtract emails.

.. _amf-174:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-174.png
    :align: center
    :alt: figure 174

1. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

2. Select a Probe and from the Glance pane and go to
   **Discovery**/**Polling** >> **Edit Schedule**.

3. You can turn on/off a Schedule using the **Scheduled** toggle.

4. Make the changes and hit **Save Schedule**.

Editing a Probe
^^^^^^^^^^^^^^^

You can edit all the parameters of an existing Probe:

1. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

2. Select the Probe that you want to edit. **Action Menu** appears
   next to the option **Scan New Assets**.

.. _amf-175:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-175.png
    :align: center
    :alt: figure 175

3. Select **Edit** from the **Action Menu**. The Update Discovery
   Probe dialog box appears. The dialog box has the same fields as the
   `Create Discovery Probe <#creating-a-discovery-probe>`__ dialog
   box.

4. Change the parameters that you want and hit **Update**.

Deleting a Probe
^^^^^^^^^^^^^^^^

1. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

2. Select the Probe that you want to delete. **Action Menu** appears
   next to the option **Scan New Assets**.

3. Click on **Archive** from the Action Menu. A confirmation box
   appears and clicking on **Yes** deletes the Probe.

.. _status-of-a-probe:
Status/Progress of a Probe
^^^^^^^^^^^^^^^^^^^^^^^^^^

When you do a Discovery or a Polling operation, the Status tab is
updated with the operation’s progress and the date and time of
completion.

.. _amf-176:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-176.png
    :align: center
    :alt: figure 176

During a discovery the following things are shown as part of the
progress status in the **Discovery** tab:

-  **Total Nodes**: Total number of node in the network.

-  **Up Node**\ s: Total number of nodes responding to a ping.

-  **Windows Nodes**: Out of total Up Nodes how many are Windows nodes.

-  **Linux Nodes**: Out of total Up Nodes how many are Linux nodes.

-  **SNMP Nodes**: Out of total Up Nodes how many are SNMP nodes.

.. _amf-177:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-177.png
    :align: center
    :alt: figure 177

Reviewing Discovered Assets
^^^^^^^^^^^^^^^^^^^^^^^^^^^

The :ref:`Status <status-of-a-probe>`  tab houses a button called **View Assets in Stage**. If
you have scheduled a Discovery with the option, **Automatically Add
Asset in Store** as Yes, then all discoveries are staged in the Asset in
Review page which is only accessible by the **View Assets in Stage**
button.

.. _amf-178:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-178.png
    :align: center
    :alt: figure 178

Once Assets are staged, you can manually add every Asset to the List
View using the **Add** button adjacent to every Asset, or you can select
them all and add them at once using the bulk add feature (:numref:`amf-177`).
You can also delete the items in bulk.

Use Case
--------

Now we discuss a scenario where we discover Assets in a network using
three types of Discovery. We create two Probes in the process; one uses
an IP Range Network and other, Domain Network. The Probe using the IP
Range Network can discover all types of Assets, but the other Probe can
discover only Windows machines. The use case gives you an overview of
the entire process involved in setting up Discovery in Flotomate.

We have the following Assets in the network that we want to discover:

- Three Windows workstations in a domain.

- One Linux workstation.

- An SNMP enabled router.

IP Range Network Discovery Probe
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

We now create a Discovery Probe that uses WMI, SSH, and SNMP protocols
to discover Assets in a network. We start by configuring the
Infrastructure.

**Adding Credentials:**

Credentials help us to get access to nodes so that we can fetch the
necessary data. We have the following credentials to add:

-  **Windows Machines**:

   Username = Administrator

   Domain Name = mindarray.com

   Password: Mind@launch

-  **Linux Machine**:

   Domain Username = discovery

   Password = admin

-  **SNMP Enabled Router**:

   Community String = public

   System OID = .1.3.6.1.4.1.16972

   **SNMP Device Properties:**

   Mac Address: .1.3.6.1.2.1.17.2.5.0

   Description: .1.3.6.1.2.1.1.1.0

   Uptime: .1.3.6.1.2.1.1.3

   Support: .1.3.6.1.2.1.10.23.2.3.1.5.210000.1

   ContactNo: .1.3.6.1.2.1.10.23.2.3.1.6.210000.1

We have to create the following Discovery types to incorporate the above
credentials:

-  WMI for Windows machines

-  SSH for the Linux machine

-  SNMP for the router.

Now we add the credentials:

-  Go to **Admin** (one of the Navigation Tabs) >> **Credential
   Library** (Under IT Infrastructure).

-  We add the credentials using the Add Credential dialog box. Learn how
   to add credentials: Credential Library.

.. _amf-179.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-179.1.png
    :align: center
    :alt: figure 179.1
    
.. _amf-179.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-179.2.png
    :align: center
    :alt: figure 179.2

.. _amf-179.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-179.3.png
    :align: center
    :alt: figure 179.3

.. _amf-179.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-179.4.png
    :align: center
    :alt: figure 179.4

**Adding Custom SNMP Properties**

SNMP Custom Properties allow us to fetch specific property values of the
SNMP router. The values are located using OIDs (Object IDs). An OID is
an address to identify a device and its statuses. For example, we can
know the temperature reading coming from a sensor at a remote facility.

Before fetching any properties of an SNMP device, the product has to
identify the device (Asset type) and this happens using the sysOID. A
sysOID is a series of numbers that uniquely identifies an SNMP device.
It is included when adding an SNMP device in the SNMP Custom Properties
section. Once an SNMP device is added then the OIDs for the custom
properties are added.

The sysOID also helps in fetching manufacturer details of a device. If
manufacturer records have sysOIDs then this is possible. You can also
add a manufacturer when adding an SNMP device in SNMP Custom Properties.

.. _amf-180.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-180.1.png
    :align: center
    :alt: figure 180.1

.. _amf-180.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-180.2.png
    :align: center
    :alt: figure 180.2

.. _amf-180.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-180.3.png
    :align: center
    :alt: figure 180.3

.. _amf-180.4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-180.4.png
    :align: center
    :alt: figure 180.4

Related Topic:

-  `SNMP Properties <#snmp-custom-properties>`__

-  `Adding Manufacturer <#adding-a-manufacturer>`__.

**Adding a Network:**

Now that we have added the credentials, It is time to add a Network that
would utilize the credentials to communicate with the nodes.

-  Go to **Admin** >> **Networks** (under IT Infrastructure).

-  We use the `Add Network <#network>`__ dialog box to add a Network
   called IP_Range.

.. _amf-181:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-181.png
    :align: center
    :alt: figure 181

Now we are going to see what Network information we have entered and
what options we have selected.

.. _amf-182:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-182.png
    :align: center
    :alt: figure 182

.. _amf-183:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-183.png
    :align: center
    :alt: figure 183

We have entered the IP addresses of every machine/device as a
comma-separated list. We do not know whether their IP addresses are
static or not, so we have gone with the DHCP. Finally, we have added the
credentials that we created earlier.

**Configuring DNS:**

Since we have selected the Protocol Type as DHCP, we need to configure
the DNS settings. Learn more about DNS Configuration:

-  We go to **Admin** >> **DNS Configuration** (Under IT
   Infrastructure).

-  The DNS Configurations page opens. We add the Primary DNS and
   **Update** the settings.

.. _amf-184:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-184.png
    :align: center
    :alt: figure 184

**Creating a Discovery Probe:**

Now we create the Discovery Probe that performs the discovery in the
network.

-  We go to **Asset** (one of the Navigation Tabs) >> **Discovery
   Probe**.

-  We create a Probe called IP_Range_Probe using the Network that we
   have created. Learn `how to create a
   Probe <#creating-a-discovery-probe>`__.

.. _amf-185:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-185.png
    :align: center
    :alt: figure 185

**Our first Discovery Operation:**

Running our first discovery operation:

-  We go to **Assets** >> **Discovery Probe**.

-  We select IP_Range_Probe and click on **Scan New Assets**. We select
   automatic addition of Assets. The Discovery operation starts and
   populates the CMDB. We can view the Assets in the Asset List View.

.. _amf-186:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-186.png
    :align: center
    :alt: figure 186

Domain Network Discovery Probe
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

We create another Probe which uses a Domain Network. We already have the
necessary credential in the Library. We just need to add a new Network.

**Adding a Network:**

We add a new Network called Domain_Net almost following the same steps
as we did while adding the IP_Range. The difference is that here the
Network Type is a Domain Network and Domain Network Type is Windows
Domain Controller.

Domain Controller Name can be an IP Address or a domain name. If IP
Address is there, then you must configure DNS.

.. _amf-187:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-187.png
    :align: center
    :alt: figure 187

**Creating a Discovery Probe:**

We create another Probe that uses a Domain Network to discovery Windows
machines. As we did with IP_Range_Probe, we use the **Create Discovery
Probe** dialog box.to create Domain_Net_Probe.

.. _amf-188.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-188.1.png
    :align: center
    :alt: figure 188.1

.. _amf-188.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-188.2.png
    :align: center
    :alt: figure 188.2


**Discovery of Assets:**

We have cleared the Asset List View so we can perform another Discovery
using the new Probe. We are going to run the Domain_Net_Probe by
clicking on **Scan New Assets** from the Discovery Probe page. We select the
auto-addition option and the discovered Assets are automatically added
to the CMDB.

Flotomate Discovery Agent 
=========================

Not all workstations in an organization are part of a network, but
still, they need discovery. By using our Agent Application, Flotomate
can fetch data from such workstations remotely.

Flotomate’s Agent Application is a lightweight application that runs in
the background of a workstation, acquires data, and pushes it directly
to the main server.

Minimum System Requirements
---------------------------

The following table highlights the hardware and software requirements
for a system to run the Agent Application.

+----------------------+----------------------+
| **Processor Type**   | Intel Dual Core      |
+======================+======================+
| **Processor Speed**  | 2.6 GHz              |
+----------------------+----------------------+
| **RAM**              | 1 GB                 |
+----------------------+----------------------+
| **Free Hard Disk**   | 100 MB               |
+----------------------+----------------------+
| **Operating System** | Windows 7 and higher/|
|                      | Ubuntu 16 and higher |
+----------------------+----------------------+

Installing the Discovery Agent Application
------------------------------------------

Installing in Windows:
^^^^^^^^^^^^^^^^^^^^^^

Installing the Agent on a Windows machine can be done in three ways:

**Using the Application Installer:**

1. Download the Agent Application installer on the workstation.

2. Go to the directory where the Agent.exe file is situated.

3. Run Agent.exe as Administrator.

.. _amf-189:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-189.png
    :align: center
    :alt: figure 189

4. The installation wizard opens. Click Next and set destination path.

.. _amf-190:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-190.png
    :align: center
    :alt: figure 190

5. In the URL field, enter the URL of Service Desk’s main server and
   click **Next**.

   .. note:: http or https in URL is a must.

.. _amf-191:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-191.png
    :align: center
    :alt: figure 191

6. In the next dialog box, click Install to complete your
   installation.

**Using the Application Installer (Non-Interactive):**

1. You can also install the Agent Application from the Command Prompt
   without the hassle of seeing multiple dialog boxes.

2. Open CMD and change the target path to Agent.exe.

3. Type Agent.exe and the URL of the main server, and hit enter. Your
   installation is done.

.. _amf-192:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-192.png
    :align: center
    :alt: figure 192

**Using PsExec for installation:**

PsExec lets you run processes remotely on other systems without the need
of a client and with full access to console applications. Using PsExec,
you can launch and execute CMD commands remotely. PsExec is part of the
PsTools toolkit developed by Sysinternals.

1. Download PSTools.zip from the following link:

   https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/share/PSTools.zip

2. Extract the zip file to a folder.

3. Download the Agent.exe file from the following link:

   https://s3.ap-south-1.amazonaws.com/flotomate-customer-releases/latest/agent/Agent.exe

4. Put Agent.exe in the PSTools folder.

5. Add IP list in ip.txt file for installing agent in those computers.

6. Now run setup.bat.

7. Enter the Url of the main server.

8. Enter Domain Username and password then hit enter.

9. It will take time for installing agent in all Computers.

Uninstalling (Windows) the Discovery Agent Application
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Go to the directory where Agent.exe file is situated.

2. Run the Agent.exe file.

3. Given that you have already installed the Agent Application, the
     Agent Setup Wizard leads you to the Modify, Repair, and Remove
     installation dialog box.

.. _amf-193:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-193.png
    :align: center
    :alt: figure 193

4. Select Remove and follow the instructions to remove the Agent
   Application.