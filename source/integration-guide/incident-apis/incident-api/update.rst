.. _update-api:

***************************
**POST** Update an Incident
***************************

::

 {{server-url}}/api/v1/incident/{{Incident-Id}}

You can update the details of an existing incident/request ticket by calling the above endpoint with the incident ID. 
You have to pass the following key-values:

**Header**

+---------------+----------------------------------------------------+
| **Key**       | **Description**                                    |
+---------------+----------------------------------------------------+
| Authorization | Bearer {access token obtained after authorization} |
+---------------+----------------------------------------------------+
| Content-Type  | application/json                                   |
+---------------+----------------------------------------------------+
 
**Body**

+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| Key                     | Value Type   | Description                                                                                              |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| subject                 | STRING       | Subject or Title of an Incident                                                                          |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| description             | STRING       | Description of an Incident                                                                               |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| categoryName            | STRING       | Category Name of an Incident. Set to 'Incident' as It is default to 'Service Request                     |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| impact                  | ENUM         | Describes the effect of the incident/request. Possible values: LOW, ONUSER , ONDEPARTMENT, Or ONBUSINESS |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| priority                | ENUM         | Shows the importance of the request/incident. Possible values: LOW,MEDIUM,HIGH,URGENT                    |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| urgency                 | ENUM         | Marks the request as urgent. Possible values: LOW,MEDIUM,HIGH, or URGENT                                 |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| locationName            | STRING       | Location Name where Incident happened. Note that Location Must Exist with same name                      |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| tags                    | String Array | Tags on an Incident                                                                                      |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| spam                    | Boolean      | true or false                                                                                            |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| status                  | STRING       | Exact status of the incident                                                                             |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| attachmentsRefNames     | String Array | array of file reference name, view upload api doc.                                                       |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+
| customFieldValueDetails |              | View create incident API body details.                                                                   |
+-------------------------+--------------+----------------------------------------------------------------------------------------------------------+

Example (Request & Response)
----------------------------

**Request**

::
  
  curl --request POST \
  --url 'http://{{server-url}}/api/incident/{{Incident-Id}}' \
  --header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJncmFudF90eXBlIjoicGFzc3dvcmQiLCJ1c2VyX25hbWUiOiJqb2huQGZsb3RvbWF0ZS5jb20iLCJzY29wZSI6WyJvdGhlci1hcGktc2NvcGUiXSwiZXhwIjoxNTM2MjM4NjYwLCJhdXRob3JpdGllcyI6WyJVU0VSIl0sImp0aSI6IjAzZGI3ZmI0LTVmNjUtNGM2Ny1hZTJkLTk4ODkyYzRiNzI3NyIsImNsaWVudF9pZCI6IlRyaXBBcHAtY2xpZW50In0.frXc5yUhA2QDRmTEQW9_kqQV0y7zjqImYMLMqzf2pZ8' \
  --header 'Content-Type: application/json' \
  --data '{
	"status":"Resolved"
    }'
    
**Response**

::

 {
  "returnCode": "SUCCESS",
  "status": 0,
  "userMessage": null,
  "id": 501
  }

