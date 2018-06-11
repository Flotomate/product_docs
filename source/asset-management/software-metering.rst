.. _software-metering-1:
*****************
Software Metering
*****************

Metering is a convenient tool to track the utilization of a Software
application across machines in an organization. Using Metering,
{Product} can track three usage statistics of a Software Asset using an
Agent. You have to enable Metering individually for Software Assets that
you want to track. Currently, Metering tracks the following information
of a Software Asset:

-  The number of times the Software application was open. Also referred
   to as Usage Count

-  Total time the Software Application was used. Also referred to as
   Usage Duration.

-  Time elapsed since the application was last open. Also referred to as
   Last Used.

Adding a Meter
==============

1. Go to **Asset** (A Navigation Tab) >> **Software Meter**.

2. The Software Meter page opens. Here you can view all the Meters that
   you have created. Click on **Create a Meter** situated in the top
   right corner of the page.

.. _amf-148:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-148.png
    :align: center
    :alt: figure 148

3. The Create a Meter dialog box opens. Then you have to provide the
   following information:

    a. **Meter information**: In this section, you have to provide a
       **Name** and **Description** of the Meter.

        .. _amf-149:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-149.png
            :align: center
            :alt: figure 149

    b. **Select Software Asset**: Select the Software that you want to
       meter. You can search the Software using the search bar. The search
       bar supports Advanced Search. Learn `how to use Advanced
       Search <#_Understanding_the_Asset>`__.

        .. _amf-150:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-150.png
            :align: center
            :alt: figure 150

    c. **Configure Executable File Name**: As the name suggests, you have to
       provide the name of the executable file of the Software application
       if the file is not configured automatically.

        .. _amf-151:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-151.png
            :align: center
            :alt: figure 151

    d. **Select Computer**: You have two ways to add computers:

        i. **Computers**: You have to select computers with the {Product}
           Agent manually from a list. You can search for computers in the
           search bar. The search bar supports Advanced Search.

        .. _amf-152:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-152.png
            :align: center
            :alt: figure 152

        ii. **Network**: You can select all the computers with the Agent in
            an IP Range defined Network. Here you have to select the Network.

        .. _amf-153:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-153.png
            :align: center
            :alt: figure 153

4. After providing the information, click on **Create** to add the
   meter in the Software Meter page.

Viewing Meter Statistics
========================

There are two ways to view the data collected by a Meter:

-  Go to the Software Meter page and click on a Meter to view the data
   in the right-hand side information pane.

.. _amf-154:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-154.png
    :align: center
    :alt: figure 154

-  You can also view the Metering data in the `Details
   View <#searching-assets>`__ of the Software Asset under the Meter
   tab.

.. _amf-155:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-155.png
    :align: center
    :alt: figure 155

Viewing Meter Statistics for Consolidated Software Assets
=========================================================

In a Consolidation of Software Assets, one Asset is the Primary Asset,
and the rest are Secondary Assets. If any or all the Assets have a
Meter, then the following scenarios prevail.

-  If all Assets in a Consolidation have a Meter, then the Primary Asset
   shows the cumulative data of all the Assets in its Meter tab, and the
   Secondary Assets shows their individual meter data.

-  If the Primary Asset does not have a Meter but Secondary Assets have
   then the Primary Asset shows the cumulative meter data of Secondary
   Assets, and the Secondary Assets show their data. In vice-versa, the
   Primary Asset shows its data, and the Secondary Assets show no data.

Whatever Meter data is present in a Consolidation it gets added to the
Primary Asset.