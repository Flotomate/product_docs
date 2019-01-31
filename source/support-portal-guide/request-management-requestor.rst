*********************************
Request Management for Requesters
*********************************

The Customer Portal provides a simple interface for Requesters to perform the following operations:

- Create and manage tickets.
- Access service catalog.
- Open knowledge articles and FAQs.
- View announcements.

.. _creating-a-request-1:

Creating a Request 
==================

The Create a Request form on the Customer Portal is a toned down version
of the Technician Portal.

In order to create a new request ticket, a requester will go through the following steps:

-  He logs into the customer portal and clicks on **Create Request**.

.. note:: Requesters can create tickets without login, if the admin has set the :ref:`permissions in preference <helpdesk security>`. 

.. _rmf-78:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-78.png
    :align: center
    :alt: figure 78

.. _rmf-79:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-79.png
    :align: center
    :alt: figure 79

-  The **Create Request** dialog box opens. He fills the request form and submits. Some of the important fields are:

   a. Category

   b. Requester Email ID 

   c. Subject

-  The moment he clicks on **Create** a new ticket is create. 

Creating a Request with an Email 
--------------------------------

Flotomate gives the option to set up an email as the Helpdesk email
address. Requestors can send an email to create a request ticket.

The question, who can create a Request, depends on the :ref:`Preference <helpdesk security>`
settings in the **Admin**. If security settings allow creating Requests
without login, then anyone can create a Request.
Else, the system accepts email Requests from registered emails only.

When you create a Request using an email, the email subject becomes the
Request Subject, email body becomes the Request Description, and any
attachments become the Request ticket attachment.

.. _request-list-view-1:

My Request
==========

Requestors can manage their Requests from the Customer Portal's My Request section.

A requester can access the My Request section by: 

- Logging in to the Customer Portal.

- Clicking on **My Request**. 

In the **My Request** section a requester can view all this request tickets.

.. _rmf-80:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-80.png
    :align: center
    :alt: figure 80

.. _searching-request-1:

Searching Request
=================

There are two broad ways to search requests:

-  **Search Bar**: This search bar is similar to the one in the :ref:`Technician List View <Searching Requests>`.

-  **Filters**: Status-based filters that tell you about the distribution of Requests under various predefined and custom statuses:

.. _rmf-81:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-81.png
    :align: center
    :alt: figure 81

.. _request-details-view-1:

Request Details View
====================

A requester can open one of his requests from the :ref:`My Request <request-list-view-1>` section. The details view opens, where the requester can perform the
following actions:

- Update request details.

- Communicate with a technician. 

- Edit custom fields.

- Link assets. This feature has to be turned on by an admin from Admin >> :ref:`Preference <helpdesk security>`.

In the details view of a request, the requester will have the following sections:

    .. _rmf-82:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-82.png
        :align: center
        :alt: figure 82

    a. Section –A are the :ref:`classifier <classify-requests-1>`\ \ s.

    b. Section-B is the :ref:`comment section <conversation-with-technician>`.
       The Requester can also view any linked Knowledge Base write-ups here.

       Custom Fields tab allows the requester to modify custom field values. 

       Linked Assets tab lists all linked assets with the request. A requester can only link assets that are assigned to him/her. 

    c. Section-C shows the name and email of the assigned technician.

    d. Section-D houses :ref:`Resolve <resolving-a-request>` and :ref:`Edit <editing-subject-and-description>` options. Along with
       them, there's an action menu with the option to attach documents. 

.. _classify-requests-1:

Classify Requests
=================

Flotomate allows requesters to classify Requests, from the :ref:`details view <request-details-view-1>`, based on the following:

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

Requesters can start a conversation thread with a Technician:

To write a comment, a requester can:

-  Go to the :ref:`Details View <request-details-view-1>` of a Request.

-  Scroll down to the **Conversation** tab and click on **Reply to
   Technician**. The pane expands to show an editor.

.. _rmf-84:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-84.png
    :align: center
    :alt: figure 84

-  Write his/her comment and also attach files with the comment.

A requester can search and sort the comment thread.

Resolving a Request
===================

A Requester can resolve a Request in the following ways:

-  In the :ref:`List View <request-list-view-1>`, he clicks on the **Resolve**
   button adjacent to a Request’s Subject line. The Status changes to
   Resolve.

-  In the :ref:`Details View <request-details-view-1>`, he clicks on the **Resolve**
   button situated in the top right corner of the page. The Status
   Changes to Resolve.

Reopening a Request
-------------------

A requester can open a Request in the same ways he/she resolved it, instead of
**Resolve** he has to **Reopen**.

Editing Subject and Description
===============================

Requesters can edit the Subject and Description of a Request in the
following ways:

.. _rmf-84.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-84.1.png
    :align: center
    :alt: figure 84.1

-  In the :ref:`List View <request-list-view-1>`, he clicks on the **Edit**
   button adjacent to a Request’s Subject line. A dialog box opens, where he
   performs the edits and hits Update.

-  In the :ref:`Details View <request-details-view-1>`, he clicks on the **Edit**
   button situated in the top right corner of the page. A dialog box
   opens, where he performs the edits and hits Update.

Requester Linking Assets with Request tickets
=============================================

If linking assets is :ref:`allowed by the admin <Allows Requester to link Asset:>`, then a requester can attach assets, which he
is assigned to, with a request ticket. 

He can attach an asset while :ref:`creating a request <creating-a-request-1>`.

.. _rmf-84.2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-84.2.png
    :align: center
    :alt: figure 84.2

He can attach an asset from the :ref:`details view <request-details-view-1>` of a request.

.. _rmf-84.3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-84.3.png
    :align: center
    :alt: figure 84.3