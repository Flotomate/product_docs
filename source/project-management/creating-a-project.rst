********************
Create a New Project
********************

.. note:: Technicians with necessary permissions can create a project. :ref:`Learn more <Technician Roles>`.

A technician can create a new project in the following way:

- He goes to the :ref:`project list page <Project Management List View>`. 

- He clicks on the **Create a Project** button situated in the top right corner of the page.

.. _proj-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/project-management/PROJ-10.png
    :align: center
    :alt: figure 10

- A dialog box opens where the technician can enter the following inputs:

    .. _proj-11:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/project-management/PROJ-11.png
        :align: center
        :alt: figure 11

  a. Name of the project in the name field.

  b. **Project Key**: The project key will be used to generate unique ids for tasks created in the project.

  c. Set the project owner. He/she will be the assigned technician.

  d. Set the priority of the project.

  e. Set the Start and end date of the project.

  f. Set the location of the project; this applies location scope to the project. To be member/owner of the project, a technician has to have the
     location permission (or All Location permission) as set in the project. Learn more about :ref:`location scoping <Data Segregation with Location Scope>`.

  g. Set a Department. :ref:`Learn how to add more departments <ad-departments>` 

  h. Set a Category. :ref:`Learn how to add more Category <ad-category>`

  i. Write a description of the project.

- When done, the technician will click on **Create**.

Project Visibility
==================

- A new project is visible to the creator only by default. 

- Projects follow :ref:`location scoping <Data Segregation with Location Scope>` when it comes to visibility, which means a technician has to have the permission of the location of a project.
  A project inherits the location of the creator.

- A project creator can assign an owner and members, which allows others to view the project. 
  During assignment, the technician list is filtered based on the location permission of the creator. 