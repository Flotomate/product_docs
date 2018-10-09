****************
Ignoring a Patch
****************

The idea of Patch Management revolves around security, enhancement, and
compliance. Sometimes it may happen that specific Patches don’t comply
with the idea of Patch Management. It becomes necessary to keep these
Patches out from the IT infrastructure which might cause more trouble
than any good.

Our product allows users to ignore certain Patches for deployment.
Ignoring a Patch has the following effects:

-  An ignored Patch is segregated to a separate section called **Ignored
   Patches**.

-  A Patch is overlooked by all automatic processes (Automatic Patch
   Deployment and Automatic Patch Test).

-  An ignored Patch is overlooked even when it’s part of one or more
   Deployment Requests.

There are two ways to ignore Patches: manual and automatic (**Decline
Patch Configuration**)

.. _manual-ignore-patch:

Manually Ignore Patches
=======================

- Go to the :ref:`Patch List View <patch list view>`.

- Select the Patch/Patches that you want to ignore. The Ignore button appears above the list area.

.. _pf-54:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-54.png
   :align: center
   :alt: figure 54

- Clicking the Ignore button opens a confirmation dialog box. On
  confirming, the selected Patches are sent to the ignored list.

.. _pf-55:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-55.png
   :align: center
   :alt: figure 55

- You can also ignore a Patch from its :ref:`Details View <patch details view>`.

.. _pf-56:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-56.png
   :align: center
   :alt: figure 56

.. _decline-patch-configuration:

Decline Patch Configuration
===========================

Ignoring Patches is a vital security feature (:ref:`Learn
More <manual-ignore-patch>`), and Decline Patch Configuration allows you
to automate this process. The automatic feature works to ignore Patches
for a specific set of Computers which is different from manual ignoring
(where a Patch is ignored for all Computers).

A decline configuration jumps into action whenever a Computer demands a
Patch. It checks whether the Patch is part of any DC and updates the
Patch database accordingly. Patches ignored automatically are also added
to the global ignored list, but you can drill down to the specific
Computers where they have been ignored using the UI features.

We now create a Decline Patch Configuration that ignores Windows
Defender patches for the Computer Group Alpha.

.. note:: The maximum number of decline configurations you can create is ten.

-  We go to **Patch** from the **Launcher**.

-  We select **Decline Patch Configuration** from the Patch menu.

.. _pf-57:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-57.png
   :align: center
   :alt: figure 57

-  The Decline Patch Configuration page opens. Here we can view all
   existing decline configurations. We click on **Create Configuration**
   situated in the top right corner of the page.

-  The Create page opens. We provide a name and description.

.. _pf-58:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-58.png
   :align: center
   :alt: figure 58

-  We see the Patches and application for selection. Selected Applications and Patches are considered as a whole.  

.. _pf-59:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-59.png
   :align: center
   :alt: figure 59

-  We select the application Windows Defender (:numref:`pf-59`). All existing
   and future Patches of Windows Defender for the target computers will be
   ignored. We can also select individual Patches for ignoring or mix
   things up by using both application and Patches.

   When selecting an application, we can specify which severities to
   consider.

.. _pf-60.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-60.1.png
   :align: center
   :alt: figure 60.1
.. _pf-60.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-60.2.png
   :align: center
   :alt: figure 60.2

.. _pf-60.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-60.3.png
   :align: center
   :alt: figure 60.3

-  We set a Remote Office and a include condition that will select computers belonging to the Alpha group. 
   Here you can set the following things:

   a. Set a :ref:`Remote Office <add-remote-office>`. This will allow auto selection of multiple computers from a Remote Office's 
      network may or may not be based on include and exclude conditions. 

   b. Set :ref:`individual <Adding of Computers from List>` computer 

   
   c. Set a different :ref:`Scope<Adding Multiple Scopes>` (Target) if there are multiple Remote Offices.    

-  We click on **Create** to save our decline configuration.

-  Later we can edit the decline configuration from the Decline Patch
   Configuration page.

.. _pf-61:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-61.png
   :align: center
   :alt: figure 61

.. _un-ignore-patches:

Un-Ignoring Patches
===================

You can un-ignore Patches that have been ignored; it doesn’t matter
whether they have been manually ignored or by a decline configuration.

The process of un-ignoring is same as :ref:`manually ignoring a
Patch <manual-ignore-patch>` where instead Ignore button you get
Un-Ignore button. When you un-ignore a Patch, it happens globally.