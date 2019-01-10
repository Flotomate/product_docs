*****************************
Release Notes - Sparrow 3.1.0
*****************************

**Introduction of New Features**
================================

1. Agent-less Discovery of Solaris System
-----------------------------------------

2. Disaster Recovery
--------------------

Disaster recovery is an automated process to replicate the database of the main server in a remote server. 

3. Activation Key Using API
---------------------------

The license of Flotomate ITSM is binding with the MAC address of the server. In an event where an admin decides to migrate our product to 
a different server, he will get an error of license not being enough. This error is due to the change in MAC address. 

We have added a feature where the admin makes an api call which yields an activation key. He will give the activation key to us,
and we will use it to generate a new license. :ref:`Learn more <Reactivate License using API>`.

5. ITSM Plugin - SMS Plugin
---------------------------

We now have a plugin that can send an SMS using a third party API. :ref:`Learn More <ITSM Plugin - Text SMS Integration>`.

**Feature Improvements**
========================

1. ITSM Plugin - Active Directory Integration
---------------------------------------------

With the existing plugin, users can now create new users in a AD with a password and reset the password of an existing user. :ref:`Lear more <ITSM Plugin - Active Directory Integration>`.  
