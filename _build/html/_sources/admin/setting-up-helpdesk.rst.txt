*******************
Setting Up Helpdesk
*******************

Email Command Settings
======================

You can change the details of a **Request** remotely using an email.
Along with changing details, you can also add a note to a Request.

You create an email command tag, and you have to enclose your Request
details within the email command tags along with [[**Request** Id]] in
the subject field.

Setting Up Email Command:
-------------------------

.. note:: Whatever parameters you want to change, you have to have the
          necessary permissions in your role.

1. Go to **Admin** >> **Email Command Settings** (Helpdesk).

2. The Email Command Settings dialog box opens. You can change only the
   details in Available Commands of a Request. Add your email command
   in the Email Command field.

.. _adf-109:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-109.png
    :align: center
    :alt: figure 109

3. The Subject and Content section of the page gives you a preview of
   how to format an email to change a Request. The Request Id has to be
   in the subject section, and whatever you write in the email body,
   other than the command line, appears under collaborate in the
   Request details page(:numref:`adf-110`).

.. _adf-110:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-110.png
    :align: center
    :alt: figure 110

Request Feedback Settings
=========================

You can send an email to a Requestor of a Request asking for a Feedback.
The email contains a link to the feedback form. You can choose whether
to send the link with the Resolved and Closed email notification or send
it manually in a separate email.

-  Go to **Admin** >> **Request Feedback Settings** (Helpdesk).

.. _adf-111:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-111.png
    :align: center
    :alt: figure 111

-  You can automatically send a feedback link to a Requestor in the
   following ways:

   a. **Resolving a Request**: If you toggle the Resolved button on, a
      feedback link is sent with the email notification on Resolving a
      Request.

   b. **Closing a Request**: If you toggle the Closed button on, a
      feedback link is sent with the email notification on Closing a
      Request.

-  If you turn **Send feedback manually** button on, then you can send a
   feedback link to a Requester from the Details View of a Request.

.. _adf-112.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-112.1.png
    :align: center
    :alt: figure 112.1

.. _adf-112.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-112.2.png
    :align: center
    :alt: figure 112.2

-  On clicking on a feedback link you get following page:

.. _adf-113:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-113.png
    :align: center
    :alt: figure 113

Priority Matrix
===============

In the product, Priority is a way to set the importance of a Request
ticket. A Technician can set the Priority of a Request manually or
automatically using the Priority Matrix feature.

**To open Priority Matrix:**

-  Go to **Admin** (A Navigation Tab) >> **Priority Matrix** (in
   Helpdesk). The Priority Matrix page opens.

.. _adf-114:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-114.png
    :align: center
    :alt: figure 114

The Priority Matrix is a matrix with the column head having the Urgency
values and rows having the Impact values. For example, if you want to
set the Priority for Urgency **Low** and Impact **On Department** as
**High** then you have to set the following row column value:

.. _adf-115:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-115.png
    :align: center
    :alt: figure 115

This way you have to set the values for all row and column combinations.
The system automatically sets the Priority of a Request based on the
matrix. You can decide whether you want users to override the set
Priority using the toggle (:numref:`adf-114`).