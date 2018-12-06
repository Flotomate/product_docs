.. _create-api:

***************************
**POST** Create an Incident
***************************

::

 {{server-url}}/api/v1/incident

In order to create a new incident/request, you have to call the above endpoint with the following key-values:

**Header**

+---------------+----------------------------------------------------+
| **Key**       | **Description**                                    |
+---------------+----------------------------------------------------+
| Authorization | Bearer {access token obtained after authorization} |
+---------------+----------------------------------------------------+
| Content-Type  | application/json                                   |
+---------------+----------------------------------------------------+

**Body**

You would be sending a JSON request that will create a ticket and populate its details. Some of the key-value pairs are compulsory, notice the description of each.

.. note:: Keys with asterisk are compulsory.

+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
|        Keys               |   Value Type   |                                                 Description                                                             |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| subject*                  | STRING         | Subject of the ticket.                                                                                                  |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| categoryName*             | STRING         | Category Name of an Incident. Set to 'Incident' as It is default to 'Service Request                                    |
|                           |                |                                                                                                                         |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| requesterEmail*           | STRING         | Email address of the user registered for the client.                                                                    |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| ccEmailSet                | String Array   | Email Address of People to whom notification to be sent for certain events on Incident                                  |
|                           |                |                                                                                                                         |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| tags                      | String Array   | These are additional identifiers attached to a ticket. Its a list                                                       |
|                           |                | that can contain n number of STRINGS.                                                                                   |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| impact                    | ENUM           | Describes the effect of the incident/request. Possible values: LOW, ONUSER , ONDEPARTMENT, Or ONBUSINESS                |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| priority                  | ENUM           | Shows the importance of the request/incident. Possible values: LOW,MEDIUM,HIGH,URGENT                                   |        
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| urgency                   | ENUM           | Marks the request as urgent. Possible values: LOW,MEDIUM,HIGH, or URGENT                                                |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| description               | STRING         | Additional explanation about the ticket.                                                                                |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| requesterName             | STRING         | Name of the user registered for the client.                                                                             |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
| locationName              | STRING         | Location Name where Incident happened. Note that Location Must Exist with same name                                     |
|                           |                |                                                                                                                         |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
|attachmentsRefNames        | String Array   | File Reference Name of attachments for an Incident                                                                      |
|                           |                |                                                                                                                         |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+
|customFieldValueDetails    | MAP:           | This key is related to custom fields.                                                                                   |
|                           | {key:STRING,   |                                                                                                                         |
|                           |  value:OBJECT} |                                                                                                                         |
|                           |                |                                                                                                                         |
|                           |                | You have to make a GET request to the endpoint: http://{Server-url}/api/ususer/form/{module-name}                       |
|                           |                | to know what are the available custom fields and their ID.                                                              |
|                           |                | Header:Authorization: Bearer {access token after authorization}, Content-Type: application/json.                        |
|                           |                |                                                                                                                         |
|                           |                | Example customFieldValueDetails value: {"1":{"type":1,"stringValue":"Open"},"35":{"type":1,"stringValue":null}}.        |
|                           |                | Supported Type:                                                                                                         |
|                           |                | STRING = 1;                                                                                                             |
|                           |                | INTEGER = 2;                                                                                                            |
|                           |                | DOUBLE = 3;                                                                                                             |
|                           |                | BOOLEAN = 4;                                                                                                            |
|                           |                | LONG = 5;                                                                                                               |
|                           |                | INTEGER LIST = 7;                                                                                                       |
|                           |                | STRING LIST = 8;                                                                                                        |
|                           |                | BIG STRING = 10;                                                                                                        |
+---------------------------+----------------+-------------------------------------------------------------------------------------------------------------------------+

Example (Request & Response)
----------------------------

**Request**

::

 curl --request POST \
  --url 'http://{{server-url}}/api/v1/incident' \
  --header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJncmFudF90eXBlIjoicGFzc3dvcmQiLCJ1c2VyX25hbWUiOiJ0aW1AYWNtZS5jb20iLCJzY29wZSI6WyJvdGhlci1hcGktc2NvcGUiXSwiZXhwIjoxNTM4NzMxNDUxLCJhdXRob3JpdGllcyI6WyJVU0VSIl0sImp0aSI6IjI4ZjJkYmFmLWYyMTQtNDI3NS1hM2EyLTdmMjU0ZDQ0M2IyMSIsImNsaWVudF9pZCI6IkFQSS1jbGllbnQifQ.bogFU_77vgNnwgO0vcobGyjSJfPgV2JmJ6FvzyrxoO8' \
  --header 'Content-Type: application/json' \
  --data '{
	"tags":["mouse"],
	"subject":"Need a new keyboard",
	"description":"Need a wireless keyboard",
	"requesterEmail":"tim@acme.com",
	"requesterName":"Tim",
	"locationName":"Ahmedabad"
    }'

**Response**

::

 {
  "returnCode": "SUCCESS",
  "status": 0,
  "userMessage": null,
  "id": 2
 }
