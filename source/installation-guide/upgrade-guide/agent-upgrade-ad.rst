*****************************************
Agent\Monitor Bulk Installation Using GPO
*****************************************

One advantage of having an Active Directory Domain is the possibility to
deploy software packages via a Group Policy Object. Using GPO is crucial
to save time and money.

Microsoft gives us a simple way to deploy software and also provides a
quick solution to uninstall it when needed.

1. Open the Group Policy Management panel and create a new GPO.

.. _aup-9:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-9.png
    :align: center
    :alt: figure 9

.. _aup-10:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-10.png
    :align: center
    :alt: figure 10

.. _aup-11:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-11.png
    :align: center
    :alt: figure 11

.. _aup-12:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-12.png
    :align: center
    :alt: figure 12

.. _aup-13:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-13.png
    :align: center
    :alt: figure 13

.. _aup-14:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-14.png
    :align: center
    :alt: figure 14

.. _aup-15:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-15.png
    :align: center
    :alt: figure 15

.. _aup-16:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-16.png
    :align: center
    :alt: figure 16

.. _aup-17:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-17.png
    :align: center
    :alt: figure 17

.. _aup-18:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-18.png
    :align: center
    :alt: figure 18

.. _aup-19:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-19.png
    :align: center
    :alt: figure 19

.. _aup-20:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/agent-installation-guide/AUP-20.png
    :align: center
    :alt: figure 20

2. Once GPO is Created then Software Installation Starts when a System
   is Restarted or it can be started by typing the following command in the CMD of a node.

**“gpupdate /force”**
