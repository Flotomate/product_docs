*********************
Release Notes - 3.3.0
*********************

Better SLA 
===========

We have enhanced the capabilities of SLA by introducing the following features:

- SLA will now consider break time (defined in business hours) in its time calculation. 
- SLA's default due-time can be configurable. 

Improved IT Asset Management and Discovery
==========================================

We have introduced important changes in Asset Management and how it discovers assets:

- Support for Keyboard components for Windows and Ubuntu in AgentLess Discovery.
- Support for Pointing device in Windows and Ubuntu in AgentLess Discovery.
- Added support of Keyboard and Mouse in Report. 
- During Discovery Progress, users can watch the history and current progress. 
- Discovered Asset's name shown during discovery progress.
- Pagination support for asset discovery progress list.
- Users can print the discovery history.
- RDP Agent for MAC.
- Now assets having UUID as 00000000000 can also get discovered.
- Support for pointing device in Windows and Ubuntu in Agent Base Discovery.
- Provide custom field support for Product and Vendor.
- Discovery Logs can be downloaded.
- Pagination support in asset component view.
- Agent for Windows server 64 bit and 32 bit.

Motadata Reporting
==================

In this release, we have introduced new reporting capabilities and trash features:

- Trash folder functionality (Repots will not be directly deleted, they will be moved to trash first).
- Reports can be restored from trash to any other folder.
- Pre-defined Task related reports have been added. 
- Task Qualification support in Request,Problem and Change reports.
- Task Details in Request Summary report.

Changes in Task Management
==========================

Minor, but important, changes have been made which are:

- "Send notification" option in task has been added. 
- Task audit trail has been improved (date-time stamp added). 

Other Changes
=============

- User can create request without email id . (Email id is optional)
- New Email notifications: When folder is deleted, renamed and schedulers are turned off by an authorized user the owner will receive an email notification.
- RDP port changed from 5900 to 5901 in both RDP agent and main server.
- User can Login with 'Logon Name'.
- Ticket audit trail has been improved.
- Pending Approvals are ignored after closure of a ticket.
