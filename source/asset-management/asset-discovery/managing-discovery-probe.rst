**************************
Managing a Discovery Probe
**************************

The Agentless method uses a Discovery Probe for discovery. Once you
create a Probe, you can start Discovering Assets and can generate
reports based on the output of a Discovery operation.

New Assets can be added automatically to the CMDB during a Discovery
operation and kept up to date by scheduling a process called
:ref:`Polling<run-on-demand-polling>` that retrieves any changes at the
source.

Using Scheduling, you can even automate the Discovery process. You can
review the discovered Assets before committing them to the CMDB.

Run on Demand Discovery
=======================

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

   During discovery, you can view the :ref:`progress<status-of-a-probe>` under the Discovery tab.

4. All discovered Assets are added to the Asset List View; there you
   can view them and can perform other operations. If you did not
   select automatic addition to the CMDB, then discovered Assets are
   staged for :ref:`review<reviewing-discovered-assets>`; from there you
   have to commit them to the CMDB. You can view the Assets that are currently staged
   by clicking on the **View Assets in Stage** button under the Status tab.

.. _amf-169:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-169.png
    :align: center
    :alt: figure 169

Run on Demand Polling
=====================

.. note:: If the Network is set to use DHCP protocol then one has to :ref:`configure DNS <DNS Configuration>`. 

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
==========

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
              a week at a specified time.

        iv.  **Monthly**: Discovery happens in selected month/months
             of a year on a particular day at a specified time.

        The Time Zone is automatically set based on the Time-Zone in the :ref:`Account Profile <ad-account>`. but
        you can change it.     

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
============================================

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
===============

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
   :ref:`Create Discovery Probe<creating-a-discovery-probe>` dialog
   box.

4. Change the parameters that you want and hit **Update**.

Deleting a Probe
================

1. Go to **Asset** (A Navigation Tab) >> **Discovery Probe**.

2. Select the Probe that you want to delete. **Action Menu** appears
   next to the option **Scan New Assets**.

3. Click on **Archive** from the Action Menu. A confirmation box
   appears and clicking on **Yes** deletes the Probe.

.. _status-of-a-probe:

Status/Progress of a Probe
==========================

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

-  **Ubuntu Linux Nodes**: Out of total Up Nodes how many are Ubuntu Linux nodes.

-  **SNMP Nodes**: Out of total Up Nodes how many are SNMP nodes.

.. _amf-177:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-177.png
    :align: center
    :alt: figure 177

Reviewing Discovered Assets
===========================

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