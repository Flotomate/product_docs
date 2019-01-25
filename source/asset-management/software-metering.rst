.. _software-metering-1:

*****************
Software Metering
*****************

Metering is a convenient tool to track the utilization of a Software
application across machines in an organization. Using Metering,
CMDB can track two usage statistics of a Software Asset using an
Agent. A user has to enable Metering individually for Software Assets that
he/she wants to track. Currently, Metering tracks the following information
of a Software Asset:

- Total time the Software Application was used. Also referred to as
  Usage Duration.

- Time elapsed since the application was last open. Also referred to as
  Last Used.

The above two statistics are shown in two different ways: cumulative counts from all the agents and individual counts of each agent.

The metering feature is available for all OS platforms supported by the :ref:`Flotomate Agent Application <Flotomate Discovery Agent>`.

Adding a Meter
==============

Each Software has its own Meter, and Meter statistics are recorded individually. In order to track multiple Software, and a user has to
create multiple Meters. 

**Follow the Below Steps to Set Up a Meter:**

- Go to **Asset** (A Navigation Tab) >> **All Software IT Assets**, and then open the :ref:`Details View <Manage Asset Details>`
  of the Software that you want to meter.

.. _amf-147.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-147.1.png
    :align: center
    :alt: figure 147.1   

Configure Executable Filename
-----------------------------

Before you can set-up a Meter, you have to add the executable filename of the Software:

- In the Details View, Under the Details tab, click the edit icon. A new dialog box opens.

.. _amf-147.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-147.2.png
    :align: center
    :alt: figure 147.2

- Add the name; the name and extension has to match the actual filename of the Application/Software that you want to track.

.. _amf-147.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-147.3.png
    :align: center
    :alt: figure 147.3

Adding Computers
----------------

Now that the filename is added, you can now configure a Meter. Here you will be asked for a target/targets; A target is a group of
computers from where usage statistics about the Software will be collected. 

- Things to remember before adding targets:

   a. If you want to track the usage in computers belonging to a remote office, you have to first create the :ref:`Remote Office <Remote Office>`
      and then add it to the :ref:`Endpoint Scope <ad-endpoint-scope>`.

   b. If you want to add individual Computers, then you have to bring them first within the :ref:`Endpoint Scope <ad-endpoint-scope>`. 

- In the Details View, under the **Meter** Tab, click on **Configure Meter**.

.. _amf-148:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-148.png
    :align: center
    :alt: figure 148 

- The Configure Meter dialog box opens. Here you have to define a target/targets. A target can include:

    .. _amf-149:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-149.png
        :align: center
        :alt: figure 149 

   a. **A Remote Office**: You can add a Remote office to a target; to added multiple Remote Offices, you have to add multiple targets.
      You can filter the Computers within a Remote Office using include and exclude conditions. The process is similar to adding
      a Remote Office in :ref:`Endpoint Scope <add-remote-office>`.

   b. **Individual Computers**: You can search and select computers currently having the Agent application. :ref:`Learn more <Adding of Computers from List>`.       
    
- When done, click on **Update**. A meter will be added to the Software Asset.

Meter Statistics
================

There are two ways to view the data collected by a Meter:

- You can view the Metering data in the :doc:`Details View <manage-asset-details>` of the Software Asset under the Meter
  tab.

  **Things to Remember:**

   a. You have to start the Meter using the **Start** button.

   b. In order to add more targets, you have to first stop the Meter and click on Re Configure Meter.

   c. The **Reset** button restarts the Meter Counter.  

.. _amf-154:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-154.png
    :align: center
    :alt: figure 154

- Go to **Asset** >> **Software Meter**. Here you get a central repo of all created Meters; apart from that you can:

   a. Turn a Meter on and off. 

   b. View Meter statistics of individual Meter.

   c. Delete a Meter.

.. _amf-155:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-155.png
    :align: center
    :alt: figure 155

Viewing Meter Statistics for Consolidated Software Assets
=========================================================

In a :ref:`Consolidation of Software Assets <Consolidating Software>`, one Asset is the Primary Asset,
and the rest are Secondary Assets. If any or all the Assets have a
Meter, then the following scenarios prevail.

- If all Assets in a Consolidation have a Meter, then the Primary Asset
  shows the cumulative data of all the Assets in its Meter tab, and the
  Secondary Assets shows their individual meter data.

- If the Primary Asset does not have a Meter but Secondary Assets have
  then the Primary Asset shows the cumulative meter data of Secondary
  Assets, and the Secondary Assets show their data. In vice-versa, the
  Primary Asset shows its data, and the Secondary Assets show no data.

Whatever Meter data is present in a Consolidation it gets added to the
Primary Asset.