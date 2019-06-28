*************************
Workflow and SLA Use Case
*************************

.. _use-case-1:

User Story
==========

Ravi, the IT manager, is using Motadata to manage his company’s service
desk. He knows how hectic managing the service desk can be; he has been
using Motadata’s **Workflow** automation to manage all his Requests.

The Antivirus subscriptions of the marketing department are about to
expire. Ravi knows a significant flow of Requests is about to come. He
logs into the dashboard and creates a **Workflow** called Antivirus Key
Renew.

.. _adf-47:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-47.png
    :align: center
    :alt: figure 47

Ravi’s Workflow is for a **Request**. When there’s an incoming Request,
his conditions are checked against the **Request**. If a **Request**\ ’s
subject contains the word *antivirus* or description contains the word
*antivirus*, and the Department Id is Marketing then the **Request**\ ’s
Technician group is set to Network, Urgency is set to High, the
Antivirus tag is added, and due date is set to some date & time.

He then sets a custom **SLA** for the Antivirus event and names it
virus@event.

.. _adf-48:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-48.png
    :align: center
    :alt: figure 48

The **SLA** virus@event sets the minimum response time to 8 hours and
resolution time to 1 day (business time) when a **Request** has a
Category, Service Request and Department ID, Marketing.

Ravi sets the escalation in such a way that if the **Request** is not
responded within 10 hours then the **Request** is auto-assigned to John,
and if the resolution does not happen within a day then the priority is
automatically set to high.