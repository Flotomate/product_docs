.. _get-api:

**********************
**GET** Get an Inciden
**********************

::

 {{server-url}}/api/v1/incident/{{Incident-Id}}

You can fetch the details of a request/incident ticket by calling the above endpoint with the ticket ID.

You need the following key-values:

**Header**

+---------------+----------------------------------------------------+
| Key           | Description                                        |
+---------------+----------------------------------------------------+
| Authorization | Bearer {access token obtained after authorization} |
+---------------+----------------------------------------------------+

Example (Request & Response)
----------------------------

**Request**

::

 curl --request GET \
  --url 'http://192.168.0.107/api/incident/1'

**Response**

::

 {
    "requesterEmail": "tim@acme.com",
    "requesterName": "Tim",
    "ccEmailSet": [],
    "subject": "Need a new Mouse",
    "description": "Need a wireless mouse",
    "categoryName": "Service Request",
    "status": "Open",
    "impact": "LOW",
    "priority": "LOW",
    "urgency": "LOW",
    "locationName": null,
    "tags": [
        "mouse"
    ],
    "spam": false,
    "fileAttachments": null,
    "customFieldValueDetails": {}
 }