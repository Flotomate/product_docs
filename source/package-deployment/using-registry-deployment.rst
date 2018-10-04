******************************
A Registry Deployment Use Case
******************************

In a Windows machine, the Registry is a hierarchical database of lower level settings. 
The purpose of it is to serve as an archive that collects and stores configuration settings 
of Windows components, Hardware and Software. These configuration setting entires are retrieved 
by their respective Windows components, Hardware and Software at startup.

Windows Registry contains keys and values and by manipulating them we can change the behavior of the OS. Now we are going to create a 
Registry Configuration (also create Registry Items) that *disables the automatic update button in Windows 10*. Then we are going to deploy the Configuration by creating a 
Deployment Request.

**Creating a Registry Configuration:**

- We are going to create a Configuration called **Disable Windows Auto-Update ** (:ref:`Creating a Registry Configuration`).

- We require a single Registry Item that would disable the automatic update button in Windows 10 (:ref:`Creating a new Registry Item`). 
  
  We locate the following location key: **HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\WindowsUpdate\AU**.
  We then add the value data 1 having the data type: **Reg_DWORD** to the value Name: **NoAutoUpdate**. It translates into the following
  arguments for the Registry Item:

.. _sp-u-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-U-1.png
    :align: center
    :alt: figure 1

- Now we have created the Registry Item, and then we update the Configuration.

.. _sp-u-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-U-2.png
    :align: center
    :alt: figure 2

- We create a Deployment Request for the Configuration (:ref:`adding-a-package-deployment-request`).

.. _sp-u-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-U-3.png
    :align: center
    :alt: figure 3

- We check the :ref:`Deploy Status <sp-deployment-status>` to know whether the deployment was successful. 

