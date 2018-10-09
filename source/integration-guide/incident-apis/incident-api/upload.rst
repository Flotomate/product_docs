.. _upload-api:

*****************************
**POST** Upload an Attachment
*****************************

::

 {{server-url}}/api/oprfile

You can call the above endpoint to upload a file in the ITSM system. When you upload a file, you get a reference filename, 
which you can pass in the body while creating or updating an incident/request ticket; this associates the file with the ticket.

You need the following key-values:

**Header**

+---------------+----------------------------------------------------+
| Key           | Description                                        |
+---------------+----------------------------------------------------+
| Authorization | Bearer {access token obtained after authorization} |
+---------------+----------------------------------------------------+

**Body**

+------+-------------+
| Key  | Description |
+------+-------------+
| file | Filename    |
+------+-------------+

Example (Request & Response)
----------------------------


**Request**

::

 Upload an Attachment

**Response**

::

 {
  "refFileName": "k9YqG9KTAB",
  "realName": "simple_add_your_logo_rubber_stamp-r4b9fb34b28254f4ebf7f8bc25bff8fb4_6ogxj_307.jpg",
  "link": null
 }