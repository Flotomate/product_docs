*****************************
How to Update Product License
*****************************

Describes Steps to Update Flotomate License

Prerequisite:
=============

Product instance in a server.

Installation Setup:
===================

After downloading the license.lic file, follow the below steps to set up
the license file in the Product Server:

1.  Login to Product Server and open terminal.

2.  Run the terminal as a root user.

.. _pl-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-1.png
    :align: center
    :alt: figure 1

3.  Change directory to the config folder.

    **cd /opt/flotomate/main-server/config**

.. _pl-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-2.png
    :align: center
    :alt: figure 2

4.  Stop system service for ft-main-server.

    **systemctl stop ft-main-server.service**

.. _pl-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-3.png
    :align: center
    :alt: figure 3

5.  Make folder content visible and their permissions using the command
    **ls-la**.

.. _pl-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-4.png
    :align: center
    :alt: figure 4

6.  Create back up of the existing license file with the extension .bkp

    **mv licence.lic licence.lic.bkp**

.. _pl-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-5.png
    :align: center
    :alt: figure 5

7.  Copy new license file into the config folder.

    **cp /{actual path of the file}/licence.lic /.**

.. _pl-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-6.png
    :align: center
    :alt: figure 6

8.  Change owner and group of the new license file to fmtuser and
    fmtusergroup.

    **chown fmtuser:fmtusergroup licence.lic**

9.  Change permission of license file if permission is not –rw -r --
    r--.

    **chmod 644 licence.lic**

.. _pl-7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-7.png
    :align: center
    :alt: figure 7

10. Start system service for ft-main-server.

    **systemctl ft-main-server.service**

.. _pl-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/installation-guide/product-license/PL-8.png
    :align: center
    :alt: figure 8
