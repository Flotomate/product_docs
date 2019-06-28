.. _Getting Started with Email Setup:

******************
Email Server Setup
******************

Setting up an email server and linking that with the product allows the
product to send and receive emails.

Some of the capabilities that the product get after email setup are:

-  Requestors can log tickets using email.

-  The product can send :ref:`Email Notifications <setting email notifications>` and Announcements.

-  Technicians can change Request details using :ref:`Email Commands <email command settings>`.

Whether self-hosted or cloud-hosted, you can add any vanity email
address to Motadata using any one of the two email protocols: POP3 and
IMAP.

.. note:: Before configuring email, you have to create an email with your
          email host and make sure to enable the protocol you want to use (POP3 or
          IMAP).

.. note:: You need administrative rights to set the email configuration.

Email Server Configuration
==========================

-  Log in to your Dashboard and head to **Admin** from the Navigation
   Tabs. Use the search field, or you can find the Email Server
   Configuration under IT Infrastructure.

.. _adf-61.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-61.1.png
    :align: center
    :alt: figure 61.1

.. _adf-61.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-61.2.png
    :align: center
    :alt: figure 61.2

-  On clicking, you see the **Email Server Configuration** page. Your
   email host provides you with all the information needed to complete
   the process.

-  A summary of the required information:

    +-----------------------------------+-----------------------------------+
    | Outgoing Server                   | This is the hostname of your      |
    |                                   | outgoing SMTP server. For         |
    |                                   | example, the hostname of Google’s |
    |                                   | outgoing SMTP is smtp.gmail.com   |
    +-----------------------------------+-----------------------------------+
    | Outgoing Port                     | It refers to the outgoing port    |
    |                                   | number of the SMTP server.        |
    +-----------------------------------+-----------------------------------+
    | Outgoing Email                    | The outgoing email address.       |
    +-----------------------------------+-----------------------------------+
    | Outgoing Username                 | Username of the outgoing email    |
    |                                   | address.                          |
    +-----------------------------------+-----------------------------------+
    | Outgoing Password                 | Password of the outgoing email    |
    |                                   | address.                          |
    +-----------------------------------+-----------------------------------+
    | Outgoing Security Type            | Please refer to your email server |
    |                                   | specification to know what        |
    |                                   | security standards it supports.   |
    |                                   | Currently, we support TLS and     |
    |                                   | SSL.                              |
    +-----------------------------------+-----------------------------------+
    | Incoming Server                   | This is the hostname of your      |
    |                                   | incoming mail server. For         |
    |                                   | example, the hostname of Google’s |
    |                                   | incoming POP3 server is           |
    |                                   | pop.gmail.com and for IMAP        |
    |                                   | server, imap.gmail.com            |
    +-----------------------------------+-----------------------------------+
    | Incoming Port                     | It refers to the incoming port    |
    |                                   | number of the mail server.        |
    +-----------------------------------+-----------------------------------+
    | Incoming Email                    | The incoming email address.       |
    +-----------------------------------+-----------------------------------+
    | Incoming Password                 | Password of the incoming email    |
    |                                   | address.                          |
    +-----------------------------------+-----------------------------------+
    | Incoming Security Type            | Please refer to your email server |
    |                                   | specification to know what        |
    |                                   | security standards it supports.   |
    |                                   | Currently, we support TLS and     |
    |                                   | SSL.                              |
    +-----------------------------------+-----------------------------------+
    | Incoming Protocol                 | POP3 or IMAP                      |
    +-----------------------------------+-----------------------------------+
    | Incoming Supportidle              | Disable/Enable IMAP IDLE support  |
    +-----------------------------------+-----------------------------------+

-  After filling the fields, you can test the connection between the
   server and Motadata using **Test Connection**. Motadata warns you
   in case of a connection error.

-  Add any email addresses that you want to ignore (don’t want to
   receive emails from) in the **Ignore Email Addresses** field. Use
   **Update** to save your changes.

Motadata gives you two email fields one for outgoing and the other for
incoming. If you want, you can use two different addresses for outgoing
and incoming. You can use the **Email Server Configuration** page to
edit your settings later.

Enabling Email to Ticket
========================

The Email to Ticket feature allows users to create a Request by sending
an email to the incoming email ID of the product.

The subject of the email becomes the subject of the Request and the body
becomes the Description. Whether only registered users can send or
everyone depends on the **Allow to report Request without login** option
in **Admin** >> **Helpdesk Security**.

To enable this feature:

-  Go to **Admin** >> **Email Server Configuration** (IT
   Infrastructure).

-  There turn on the toggle **Enable Email to Ticket**.

-  The Category field specifies the default category applied to Requests
   created via email.

.. _adf-62:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-62.png
    :align: center
    :alt: figure 62