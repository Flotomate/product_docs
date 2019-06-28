********************************
Introduction to Motadata Plugin
********************************

What is a Plugin?
=================

A plug-in is a piece of code that integrates with our main server to perform a specific function. 
In the context of our product, a plugin is nothing but a .fp bundle (i.e. Kind of app, zip). 

What is a Plugin Server?
========================

Plugin server is a server which hosts/runs plugins. It is like our main server with a specialized purpose of running plugins. 
The main server will call a plugin server to execute specific plugin and get the desired output.

Plugin Architecture
===================

.. _plgm-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/plugin-server/PLGM-1.png
    :align: center
    :alt: figure 1

Why use a Plugin Architecture?
==============================

Different users have different needs as customization is the reality of our market. It not possible to accommodate all different needs 
in the form of a product feature, which is why we have introduced the concept of plugin architecture.

Benefits of a Plugin Architecture
---------------------------------

- Gives the ability to add business specific functions to the ITSM tool; for example, a user might want to send a notification to his CRM when a ticket is 
  created.

- Provides a great deal of flexibility when it comes to customization without burdening the tool.

- New functions can be added without changing the code base of the main product.

Some of the Types of Plugin We Support
======================================

1. **Notification Plugin**

    a. Web Call to 3rd Party System (i.e. SMS Server, ERP System, NMS System etc.) 
    b. Mobile Push Notification
    c. NMS 

2. **Discovery Plugin**

    a. Proprietary Device (i.e. For Testing, We'll use SNMP with more custom Prop)

3. **Report Plugin (Stretch Goal)**

    a. Complex Request Report Export
    b. Complex Asset Report Export
    c. Complex Widget

4. **Pull Plugin (i.e. Pull Data from Other System and Push to Motadata.)**

    a. Pull Asset Data and Merge those data in our inventory.

5. Any Other Plugin. 

Plugin Deployment Workflow
==========================

When deploying a plugin the following steps need to be executed in the given below sequence:

- Develop a {your-plugin-name} Plugin.
- Build {your-plugin-name} Plugin (.fp file).
- :ref:`Deploy in Plugin Server. <Plugin Server Setup Guide>`
- Restart Plugin Server.
- In Main-Server : :ref:`Register Test Plugin. <Register a Plugin>`
- In Main-Server : Configure Test Plugin.
- In Main-Server: Define Mapping.
- Execute Plugin by Test Execute Call or Workflow Action.