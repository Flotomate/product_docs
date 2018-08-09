How to Create Incident Using REST API
=====================================

A REST API defines a set of functions which developers can perform
requests and receive responses via HTTP protocol such as GET and POST.
{Product} allows third party clients to create Requests using REST API.

Perquisite
----------

Before using REST API, you have to create an API Client.

Learn how to create an :ref:`API Client <rest api client>`.

Creating an Incident?
---------------------

-  Go to **Admin** (A Navigation tab) >> **Integration** (under
   Automation).

-  Copy Client ID and Client Secret from the Integration page.

.. _rapi-3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/integration-guide/rest-3.png
    :align: center
    :alt: figure 3

-  Use the credentials (Client ID and Secrete) to acquire the access
   token. Here the user* credentials are required (Password and Username).

.. _rapi-4:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/integration-guide/rest-4.png
    :align: center
    :alt: figure 4

-  You will receive an access token from the server.

.. _rapi-5:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/integration-guide/rest-5.png
    :align: center
    :alt: figure 5

-  Now you can create an incident using the API path. Below is the API
   path for creating an Incident.

    **API**: *http://{server-url}/api/incident*

    **HTTP Method:** POST

    **Header**:

        **Key**: Authorization

        **Value**: Bearer {access_token}

    +-------------------+-------------------------------------------+
    | Parameters        | Value                                     |
    +-------------------+-------------------------------------------+
    | impact            | LOW, ONUSER , ONDEPARTMENT, Or ONBUSINESS |
    +-------------------+-------------------------------------------+
    | urgency           | LOW,MEDIUM,HIGH,URGENT                    |
    +-------------------+-------------------------------------------+
    | priority          | LOW,MEDIUM,HIGH,URGENT                    |
    +-------------------+-------------------------------------------+
    | tags              | Array. For ex: [ “rest” ]                 |
    +-------------------+-------------------------------------------+
    | subject           | Test Subject                              |
    +-------------------+-------------------------------------------+
    | description       | Test Decription                           |
    +-------------------+-------------------------------------------+
    | category          | 5                                         |
    +-------------------+-------------------------------------------+
    | fieldValueDetails | {                                         |
    |                   |                                           |
    |                   | "1":{                                     |
    |                   |                                           |
    |                   | "type":1,                                 |
    |                   |                                           |
    |                   | "stringValue":"Open"                      |
    |                   |                                           |
    |                   | }                                         |
    |                   |                                           |
    |                   | }                                         |
    +-------------------+-------------------------------------------+
    | requesterEmail    | User email address                        |
    +-------------------+-------------------------------------------+
    | requesterName     | User first name                           |
    +-------------------+-------------------------------------------+

    *Note*: Here User refers to the one registered with the Client. (See how
    to create API Client)*

    .. _rapi-7:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/integration-guide/rest-7.png
        :align: center
        :alt: figure 7

    **Response**:

    .. _rapi-6:
    
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/integration-guide/rest-6.png
        :align: center
        :alt: figure 6

-  Your Request is created on returning success.