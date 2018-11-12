.. _helpdesk security:

**********
Preference
**********

A lot of security issues can be thwarted just by controlling the way people use the system. With the Helpdesk Security settings
an admin can control the following:

.. note:: Open Helpdesk Security settings by going to **Admin** >> **Helpdesk Security** (under Users).

.. _adf-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-28.png
    :align: center
    :alt: figure 28

**Allow Guest Requesters to Report a Request:**

Turning on this option allows guests, without a Requestor account, to submit a Request from the Customer Portal, but they cannot view and manage their
submitted Requests. Guests, with a Requestor account, can view their
Requests in the **My Request** section after logging-in.

**Allow Technician to Report a ticket from a Guest Requester:**

Turning on this option allows Technicians to submit Requests in the
name of people who are not requestors. The product doesn't demand for authentication.

**Allows Requester to link Asset:**

.. note:: Related Topic: :ref:`Creating a Request`

Turning this option enables logged in Requesters to link Assets directly from the Create a Request form of the *Customer Portal*. 
A Requester can only link Assets that are :ref:`Used By <Classifying Assets>` him/her. 

.. _adf-28.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-28.1.png
    :align: center
    :alt: figure 28.1

**Allow Technician for Do Not Disturb mode:**

Turning this option allows Technicians to globally mark them unavailable for assignment of Request tickets through Auto Assignment. 
This option is only available on the Technician portal. Learn more about :ref:`Technician Profile <pro-edit-profile>`. 