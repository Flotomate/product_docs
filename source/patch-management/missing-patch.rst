************************
What is a Missing Patch?
************************

A missing Patch is a Patch which is supposed to be there (installed), but still it is in demand for installation. 
There are several scenarios that can generate missing Patches but we are going to discuss few of them; 
before doing that you need to understand the role of a Computer, the Update Server, and Flotomate Server, 
and how they are related with one another.

-  **Computer**: A Computer resides in a Node. It is responsible for
   acquiring and installing the Patches. It communicates with both the
   Update Server and Flotomate Server.

-  **Update Server**: It gives information about new updates and
   provides the Patches when requested. Both the Computers and Flotomate
   Server communicates with the Update Server.

-  **Flotomate Server**: It gets the new update information from the
   Computers and gives instructions to them through a Deployment
   Request. It can also fetch new Patches from the Update server and
   store them in a Shared Drive.

-  **Relationship Matrix**: Computers, Update Server, and Flotomate
   Server they all exchange information with each other and work in
   collaboration. The below Relationship Matrix highlights the
   communication and relationships between them:

+-----------------+-----------------+-----------------+-----------------+
|                 | Computer        | Update Server   | Flotomate       |
|                 |                 |                 | Server          |
+=================+=================+=================+=================+
| Computer        |                 | It checks for   | It updates the  |
|                 |                 | all available   | server with     |
|                 |                 | updates and     | information     |
|                 |                 | fetches the     | about new       |
|                 |                 | information of  | Patches.        |
|                 |                 | new Patches.    |                 |
|                 |                 |                 | Searches        |
|                 |                 | On finding a    | through         |
|                 |                 | Deployment      | Deployment      |
|                 |                 | Request, it can | Requests, and   |
|                 |                 | acquire the     | initiates       |
|                 |                 | Patches from    | deployment if a |
|                 |                 | the Update      | Deployment      |
|                 |                 | Server and      | Request demands |
|                 |                 | install them    | so.             |
|                 |                 | following a     |                 |
|                 |                 | Deployment      | It performs     |
|                 |                 | Policy.         | deployment      |
|                 |                 |                 | based on a      |
|                 |                 |                 | Deployment      |
|                 |                 |                 | Policy given by |
|                 |                 |                 | the Flotomate   |
|                 |                 |                 | Server.         |
|                 |                 |                 |                 |
|                 |                 |                 | It acquires the |
|                 |                 |                 | Patches from    |
|                 |                 |                 | the download    |
|                 |                 |                 | location on the |
|                 |                 |                 | Shared Drive.   |
+-----------------+-----------------+-----------------+-----------------+
| Update Server   | Already defined |                 | The Flotomate   |
|                 | in the above    |                 | Server can      |
|                 | row             |                 | download the    |
|                 |                 |                 | Patches from    |
|                 |                 |                 | the Update      |
|                 |                 |                 | Server in its   |
|                 |                 |                 | Shared Drive.   |
+-----------------+-----------------+-----------------+-----------------+

Some of the scenarios where a Patch can go missing:

-  A user creates a Deployment Request for a Windows security Patch. He
   selects three Computers for deployment (A, B & C). He initiates the
   deployment process. The deployment process ends with A and B
   successfully installing the Patch, and C failing to install. The next
   time when Computer-C updates the Flotomate server about its
   requirement for the same Patch, the Patch reappears as **Missing** in
   the system; the user can check the Details View of the missing Patch
   to know that Computer-C is missing the Patch.

   The bottom line is that any requested Patch which is already in the
   system as Installed, appears under the Missing tab.

-  A Patch which is installed in Computer A & B, and later a new
   Computer C arrives and demands for same patch. The Patch is shown as
   missing for Computer C.

-  Computers keep on updating the Flotomate server about required new
   Patches; these all appear as **New** Patches in the system. When a
   Computer or Computers request for a Patch which is older than the
   oldest **Installed** Patch (system record), then the requested Patch
   is shown under the **Missing** tab.