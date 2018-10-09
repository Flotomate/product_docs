***************************
Managing Incident Using API
***************************

Welcome to ITSM Incident Management API. Our APIs allow third party systems to create, update and read an Incident from our ITSM System.

All CRUD operations using APIs are done with the following methods: **GET**, **POST** and **DELETE**.

First you need to Setup your Client with our system and authenticate to acquire a Token ID. Using the Token ID you have to make all requests to our system.

Setting Up API Client
=====================

Before making any API requests, you have to register your Client with our ITSM system and acquire the following things:

- Client ID
- Client Secret
- Username
- Password

Log into the ITSM system and go to **Admin** >> **Integration** (Under Automation), and register your product for REST API.

Authorization
=============

Authentication with our ITSM system allows you to acquire an access token, using which you have to make incident requests.

**POST** Acquire Token
----------------------

::

  {{server-url}}/api/oauth/token

You have to make a POST request to the above endpoint using the following key-values:

**Header**

+---------------+--------------------------------------------------+
| **Key**       | **Description**                                  |
+---------------+--------------------------------------------------+
| Authorization | Basic Client-ID:Client-Secret encoded in Base64. |
+---------------+--------------------------------------------------+

**Body**

+------------+--------------------------------------------------------------------------------+
| **Key**    | **Description**                                                                |
+------------+--------------------------------------------------------------------------------+
| username   | UserName of user (registered with our ITSM system) for whom API to be Executed |
+------------+--------------------------------------------------------------------------------+
| password   | Password of User (registered with out ITSM system) for whom API to be Executed |
+------------+--------------------------------------------------------------------------------+
| grant_type | OAuth2 Grant Type. (i.e. password)                                             |
+------------+--------------------------------------------------------------------------------+

Example (Request & Response)
----------------------------

**Request**

::

  curl --request POST \
  --url 'http://{{server-url}}/api/oauth/token' \
  --header 'Authorization: Basic bWFpbi13ZWItYXBwLWNsaWVudDptYWluLXdlYi1hcHAtc2VjcmV0' \
  --header 'content-type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW' \
  --form username=tim@acme.com \
  --form password=123 \
  --form grant_type=password

**Response**

::

 {
  "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJncmFudF90eXBlIjoicGFzc3dvcmQiLCJ1c2VyX25hbWUiOiJ0aW1AYWNtZS5jb20iLCJzY29wZSI6WyJtYWluLXdlYi1hcHAtc2NvcGUiXSwiZXhwIjoxNTM4Njg0NTkzLCJhdXRob3JpdGllcyI6WyJVU0VSIl0sImp0aSI6IjZkM2JkMWU5LTdhOTYtNDFmZS1hZmY5LTgyYmQ1ZDVmNWNiZiIsImNsaWVudF9pZCI6Im1haW4td2ViLWFwcC1jbGllbnQifQ.1pHYIEKAsBcjNf0xiwot5fcu0KOH2E4COqiusDuVh6I",
  "token_type": "bearer",
  "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJncmFudF90eXBlIjoicGFzc3dvcmQiLCJ1c2VyX25hbWUiOiJ0aW1AYWNtZS5jb20iLCJzY29wZSI6WyJtYWluLXdlYi1hcHAtc2NvcGUiXSwiYXRpIjoiNmQzYmQxZTktN2E5Ni00MWZlLWFmZjktODJiZDVkNWY1Y2JmIiwiZXhwIjoxNTQxMjY5MzkzLCJhdXRob3JpdGllcyI6WyJVU0VSIl0sImp0aSI6ImU2YWUxZTMxLWQzZWQtNGJkYi05NTY4LWRhNmQ3NmUwZWE4YiIsImNsaWVudF9pZCI6Im1haW4td2ViLWFwcC1jbGllbnQifQ.aFV-DBgNrSS2hF91qv_zmtBsiRS2z3VsgnyoXVcAxeA",
  "expires_in": 7199,
  "scope": "main-web-app-scope",
  "jti": "6d3bd1e9-7a96-41fe-aff9-82bd5d5f5cbf"
 }


Incident APIs
=============

- :ref:`create-api`

- :ref:`get-api`

- :ref:`update-api`

- :ref:`upload-api`
 