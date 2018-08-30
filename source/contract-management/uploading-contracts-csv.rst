*************************************
Creating/Updating Contracts Using CSV
*************************************

The Contract module supports bulk creation/update of Contracts using a CSV file. A Technician has to create a CSV file with the details of 
all the Contracts to use this feature. 

**Some of the Benefits of using a CSV file:**

- A large number of Contracts can be created easily.

- A large number of existing Contracts can be modified easily.

- Saves time when working with large number of Contracts. 

- The CSV file acts as a local copy in which a Technician can work and periodically upload the file in the system. 

Using the CSV Import feature
============================

Creating a CSV file
-------------------

You can download a blank CSV file with all the column headers from the :doc:`contract-list-view`. A Technician can populate the downloaded
file with Contract details without changing the headers values.

**To Download Blank CSV:**

- Go to the :doc:`contract-list-view` and click on **Import Contracts**.

.. _con-46.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-46.1.png
    :align: center
    :alt: figure 46.1

- The Import page opens. Click on **Download Demo CSV** to download the blank file.

.. _con-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-47.png
    :align: center
    :alt: figure 47

Now open the file and input details according to the column values.

.. _con-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-48.png
    :align: center
    :alt: figure 48

Things to Remember when using the file:

- The first row is the header which should not be changed.

- Each subsequent rows will represent a single Contract. 

- When entering date and time check all available date formats. 

**Uploading a CSV File:**

- Go to the :doc:`contract-list-view` and click on **Import Contract** (ref: :numref:`con-47`) option.

- The Import page opens. Here you go through four stages before Contracts are created/updated. 

- The first stage is the Select File stage: Here you do the following things:
  
  a. **Select a Date format**: Select the date format that you have used in the CSV file. Following the available date&time formats:
    
     .. _con-49:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-49.png
        :align: center
        :alt: figure 49
     
     Few examples of date&time formats.
     
     .. _con-50:
     .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-50.png
        :align: center
        :alt: figure 50    
     
  b. **Upload the CSV file**: Select the CSV file for upload.

  When done click on **Next**.


.. _con-51:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-51.png
    :align: center
    :alt: figure 51 

- The next stage is called **Column Mapping** (refer: :numref:`con-51`). Every item in the first
  row (heading) is a name of a property. The system automatically
  matches the names in the file heading with the property names in the
  system.

  In :numref:`con-51`, the left side column has the system Contract property names and
  right side column has the property names in the CSV file.

  In case a property name does not have a match, the right-hand side
  field of the name remains empty. Here you have to manually select the
  matching name from a drop-down list by clicking on the field.

    .. _con-52:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-52.png
        :align: center
        :alt: figure 52

  It is not necessary that all the property names have to have a match;
  you can still upload your Requestors as long as required fields are
  taken care off. Click **Next** to continue to the next stage.

  You can create custom property names using Custom Fields. You can create n number of such fields, and they appear
  along side the default ones. :doc:`Learn more (head to Custom Fields) <admin-customization>`.

- The next stage is called **Unmatched Value Mapping**. The given
  property names in the header have values (rows). The system checks
  for property values that aren’t in the system.

    .. _con-53:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-53.png
        :align: center
        :alt: figure 53

  You can manually assign a value from the Possible Values (system values)
  to an Unmatched Value (value in the file). Click **Next** to continue to
  the next step.

- Now you are in the **Review** stage. Here you see the number of
  Contracts being imported (Contracts are updated in case existing Contracts are imported). Click **Import** to finish the import
  process. 

.. _con-54:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/contract-management/con-54.png
     :align: center
     :alt: figure 54

- On clicking **Import**, new Contracts are created or existing Contracts are updated, or it could be both.     
