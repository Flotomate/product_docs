*********************************
Request Management for Requesters
*********************************

The Customer Portal provides a simple interface for Requesters to create
and manage their Requests. The Customer Portal is the primary interface
between Requesters and the Helpdesk.

.. _creating-a-request-1:

Creating a Request 
==================

The Create a Request form on the Customer Portal is a toned down version
of the Technician Portal.

Requestors can also use the Create a Request dialog box without login as
guest users. An Admin has to enable the guest user feature.

-  Log in to the Customer Portal. You can log in with third-party
   credentials if SSO is already configured; please refer Administration
   Manual to know about SSO configuration.

-  Click on **Create Request**.

.. _rmf-78:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-78.png
    :align: center
    :alt: figure 78

.. _rmf-79:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-79.png
    :align: center
    :alt: figure 79

-  The **Create-a-Request** dialog box opens. You have to enter a
   Category, your email ID (your authenticated email if Request without
   login is disabled), and a Subject line. :doc:`Learn more about the
   fields<create-a-request>`.

-  Fill in the details and hit **Create**. If you are not logged in,
   then you may be asked to log in depending on the settings selected by
   the Admin. You have now created your Request.

Creating a Request with an Email 
--------------------------------

Flotomate gives the option to set up an email as the Helpdesk email
address. Requestors can send an email to create a Request.

The question, who can create a Request, depends on the **Helpdesk**
settings in the **Admin** section. If settings allow creating Requests
without login, then anyone with the Helpdesk email can create a Request.
Else, the system accepts email Requests from registered emails only.

When you create a Request using an email, the email subject becomes the
Request Subject, email body becomes the Request Description, and any
attachments become the Request attachment.

.. _request-list-view-1:

Request List View
=================

Requestors can manage their Requests on the Customer Portal in Request
List View, but a Requester has no rights to neither view nor manages
Requests created by other Requesters. He can only view and manage his
Requests.

To access Request List View

1. Log in to the Customer Portal.

2. On the homepage, you can find the button **My Requests**, click on
   it.

3. You are now on the Request List View.

    .. _rmf-80:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-80.png
        :align: center
        :alt: figure 80

    a. Section A&B are part of the :ref:`search features <searching-request-1>`.

    b. Section C is the list area for Requests. Here you can perform the
       following operations:

        i. :ref:`Classify <classify-requests-1>`

        ii.  :ref:`Resolve <resolving-a-request>`

        iii. :ref:`Edit <editing-subject-and-description>`

    c. Section-D is the details Pane of a Request.

    d. Clicking section-E gives you the option to set the number of Requests
       visible per page; the highest is 100 per page.

.. _searching-request-1:

Searching Request
=================

There are two broad ways to search requests:

-  **Search Bar**: This search bar is similar to the one in the
   :ref:`Technician List View <request-management-technician/using-a-search-bar>`.

-  **Filters**: Status-based filters that tell you about the
   distribution of Requests under various predefined and custom
   statuses:

.. _rmf-81:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-81.png
    :align: center
    :alt: figure 81

.. _request-details-view-1:

Request Details View
====================

The Details View is where a Requester communicates with the Technicians
and has access to the details of the Request.

1. Go to the :ref:`Request List View <request-list-view-1>`.

2. Click on the Subject line of a Request.

3. You are now in the Request Details View of that Request.

    .. _rmf-82:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-82.png
        :align: center
        :alt: figure 82

    a. Section –A are the :ref:`classifier <classify-requests-1>`\ \ s.

    b. Section-B is the :ref:`comment section <conversation-with-technician>`.
       The Requester can also view any linked Knowledge Base write-ups here.

    c. Section-C is the details about the assigned Technician.

    d. Section-D houses :ref:`Resolve <resolving-a-request>` and
       :ref:`Edit <editing-subject-and-description>`.

.. _classify-requests-1:

Classify Requests
=================

Flotomate allows requesters to classify Requests based on the following:

-  **Urgency**: Setting this label shows the Technicians which Requests
   to give priority. These are predefined labels that are immutable, and
   they are Low, Medium, High, and Urgent.

-  **Impact**: Setting this label shows where a Request has its effect
   which is either on User, Department or Business.

.. _rmf-83:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-83.png
    :align: center
    :alt: figure 83

Conversation with Technician
============================

Requesters can have a conversation thread with Technicians:

To write a comment:

-  Go to the :ref:`Details View <request-details-view-1>` of a Request.

-  Scroll down to the **Conversation** tab and click on **Reply to
   Technician**. The pane expands to show an editor.

.. _rmf-84:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-84.png
    :align: center
    :alt: figure 84

-  Write your comment. You can also attach files with your comments.

You can search and sort the comment thread.

Resolving a Request
===================

A Requester can resolve a Request in the following ways:

-  In the :ref:`List View <request-list-view-1>`, click on the **Resolve**
   button adjacent to a Request’s Subject line. The Status changes to
   Resolve.

-  In the :ref:`Details View <request-details-view-1>`, click on Resolve
   button situated in the top right corner of the page. The Status
   Changes to Resolve.

Reopening a Request
-------------------

You reopen a Request in the same ways you resolved it, instead of
**Resolve** you have **Reopen**.

Editing Subject and Description
===============================

Requesters can edit the Subject and Description of a Request in the
following ways:

-  In the :ref:`List View <request-list-view-1>`, click on the **Edit**
   button adjacent to a Request’s Subject line. A dialog box opens,
   perform the edits and hit Update.

-  In the :ref:`Details View <request-details-view-1>`, click on **Edit**
   button situated in the top right corner of the page. A dialog box
   opens, perform the edits and hit Update.