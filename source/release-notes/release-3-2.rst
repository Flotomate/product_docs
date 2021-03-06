****************************
Release Notes - Pigeon 3.2.0
****************************

Extended Support for Agent Less Discovery
=========================================

In this release we have extended the capabilities of the agent less discovery. Now we support the
following OSs:

- Solaris* 11.3 and 10 (It might happen that too many software might be discovered.)
- OpenSuse Tumbleweed
- Fedora 29
- CentOS* 6 and CentOS 7.6 (Some network adapter fields might not be discovered.)
- REd Hat 7.6 * (In some Redhat hardware the serial number might be missing.)
- Debian 9

Task Schedule
=============

Motadata users can create and manage task schedules. The scheduling feature allows a user to create recurring Tasks
with a defined time interval. The interval can be set as:

- Daily
- Monthly
- Weekly
- Custom interval in either minutes, hours, days or months.  

:ref:`Learn more <Scheduling Tasks>`. 

Different License Combination
=============================

Now we have different kinds of licenses to better suit the needs of our customers. The licenses are:

- All Module trial
- Asset + Patch
- Asset management license Only
- Patch Management license Only
- Service Desk + Asset 
- Service Desk +  Patch
- Service Desk Only

RDP Support
===========

Now we support RDP for Windows server 2012 and 2016. 

Better Security
===============

- Now all connections between servers and agents are now secured using HTTPS. 
- Option to disallow concurrent logging of users. The option is under **Admin** >> **Preference**. 