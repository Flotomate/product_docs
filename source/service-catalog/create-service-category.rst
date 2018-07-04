*************************
Create a Service Category
*************************

Service Category allows you to group Templates into meaningful categories; 
this is the default classification in the product.

We are going to create a new category, called Human Resource, for our :ref:`On-Board <sc-use-case>` template.

Adding Service Catalog Categories 
=================================

-  We go to **Admin** (A Navigation tab) >> **Service Categories** (under Service Catalog).

.. _scf-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-2.png
    :align: center
    :alt: figure 2

- We click on **Add** to add a new category. The Add Category dialog box opens.

- In the new dialog box, we select the Request Category (Service Request) and give a Name (Human Resource).

.. _scf-3.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-3.1.png
    :align: center
    :alt: figure 3.1

.. _scf-3.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-3.2.png
    :align: center
    :alt: figure 3.2

- You can add sub-categories to a category, up to two levels. 

Adding Service Catalog Categories Using CSV
===========================================

You can add a new category using a CSV file. Now we are going to add the category, Human Resource:

- We go to the Categories (**Service Categories**) page and click on **Import Service Catalog Categories from CSV** 
  Action Menu.

  .. _scf-4:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-4.png
      :align: center
      :alt: figure 4

- The Import page opens. We upload our CSV file with the following headings and click on **Next**:

  a. **Category**: Name of the parent category

  b. **Sub Category**: Child category if any.

  c. **Item**: Name of the category at level 3.

  d. **Key**: Unique identifier of the category.

  .. _scf-5:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-5.png
      :align: center
      :alt: figure 5

  If we don't use the property names mentioned above, then we
  have to manually match the names with the mentioned system property names.

  .. _scf-6:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-6.png
      :align: center
      :alt: figure 6

- Now we are in the **Column Mapping** stage. Every item in the first
  row (heading of the file) is a name of a property. The system automatically
  matches the names in the file heading with the property names in the
  system.

  In :numref:`scf-6`, the left side column has the system property names and
  right side column has the property names in the CSV file.

  In case a property name does not have a match, the right-hand side
  field of the name remains empty. Here you have to manually select the
  matching name from a drop-down list by clicking on the field.

  .. _scf-7:
  .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-7.png
      :align: center
      :alt: figure 7

  .. note:: It is necessary that all property names have a match.

  We click on **Next** to continue to the next stage.


- Now we are in the **Unmatched Value Mapping** stage. Since none of the values are pre-defined, we click on **Next**
  to go to the next stage.

- Now we are in the **Review** stage. Here we see the number of
  Categories being imported. We click on **Import** to finish the import
  process. 

**Edit Categories**

All custom categories whether imported or added can be edited/deleted. In the Categories page, you will find the respective options.

.. _scf-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/service-catalog/SC-8.png
    :align: center
    :alt: figure 8




