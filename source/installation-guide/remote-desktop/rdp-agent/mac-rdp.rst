********************************
MAC RDP Agent Installation Guide
********************************

Mac RDP agent can be downloaded from the system terminal.

Minimum Requirement
===================

- High Sierra OS

Installation Steps
==================

- Download the RDP installation file: `Click Here <https://flotomate-customer-releases.s3.ap-south-1.amazonaws.com/latest/rdp+server/mac/mac_rdp>`_

- Go to the directory where you have installed the RDP file. 

- Install RDP using the command: **sudo ./mac_rdp**

- Enable RDP services using the following command:

  .. code-block:: sudo launchctl list | grep com.flotomate.rdp
  .. code-block:: sudo launchctl load service  /Library/Launchdaemon/com.flotomate.rdp