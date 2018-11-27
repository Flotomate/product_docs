**********************************************
Understanding Agent-Based vs. Agentless Method
**********************************************

These two methods of discovering Asset can be compared with Push vs.
Pull. In Agentless Discovery, the Discovery engine scans a given network
for pingable Assets and populate the same in the CMDB. In Agent-Based,
every node of the network must run an Agent Application which
continuously streams the relevant data back to the server. As a best
practice, Assets which are frequently moved in the context of a
corporate network there Agent-based discovery and polling make more
sense. Whereas, Agent-less is the only way for scanning SNMP assets like
a printer, router, switches, etc.

Below are six dimensions that highlight the fundamental differences
between Agent-Based and Agentless scanning:

+-----------------------+-----------------------+-----------------------+
|                       | Agent-Based           | Agentless             |
+=======================+=======================+=======================+
| Discovery Method      | Agent-Based Discovery | Agentless Discovery   |
|                       | is a push-based       | is a pull-based       |
|                       | strategy, where every | approach, which is    |
|                       | node in a network     | designed to leverage  |
|                       | runs an Agent         | a network either      |
|                       | Application. The      | defined by a domain   |
|                       | Application pushes    | or an IP range.       |
|                       | the data into the     |                       |
|                       | main server.          | It uses network and   |
|                       |                       | management protocols  |
|                       | It does not have any  | like SNMP, WMI, etc.  |
|                       | network or domain     |                       |
|                       | barriers.             |                       |
+-----------------------+-----------------------+-----------------------+
| Deployment            | Running Agent-Based   | Agentless Discovery   |
|                       | Discoveries in        | requires one-time     |
|                       | multiple workstations | configuration of a    |
|                       | require the           | network in the main   |
|                       | individual            | server. Once a user   |
|                       | installation of the   | configures a network, |
|                       | Application. In case  | the user can create a |
|                       | the workstations are  | Discovery Probes.     |
|                       | part of a network, an |                       |
|                       | administrator can     |                       |
|                       | remotely install the  |                       |
|                       | application on all    |                       |
|                       | the workstations.     |                       |
+-----------------------+-----------------------+-----------------------+
| Device Coverage       | Currently,            | In an Agentless       |
|                       | Agent-Based scanning  | setup, the product    |
|                       | supports the          | scans Assets that     |
|                       | Discovery of Windows  |                       |
|                       | and Ubuntu machines.  | following credential  |
|                       |                       | types:                |
|                       |                       |                       |
|                       |                       | -  WMI (Windows       |
|                       |                       |    Management         |
|                       |                       |    Instrumentation)   |
|                       |                       |                       |
|                       |                       | -  SSH                |
|                       |                       |                       |
|                       |                       | -  SNMP               |
|                       |                       |                       |
|                       |                       | -  SNMP V3            |
+-----------------------+-----------------------+-----------------------+
| Maintenance           | The Agent Application | No maintenance needed |
|                       | requires maintenance  | at the level of a     |
|                       | in the form of        | node.                 |
|                       | patches and updates   |                       |
|                       | at the node level.    |                       |
+-----------------------+-----------------------+-----------------------+

**Which one is better, Agentless or Agent-Based?**

It depends upon your requirement. Both Agent-Based and Agentless
Discovery are similar in their capabilities and scale. The differences
are in the way they function and their scope.