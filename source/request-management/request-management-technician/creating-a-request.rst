******************
Creating a Request 
******************

Technicians can create Requests using the email to ticket feature and
the Create a Request dialog box.

The Create a Request dialog box is available on both the Requestor and
Technician Portal. However, the Create a Request form on the Technician
portal is different. It has additional fields that are specific to the
needs of the Technicians.

Only people with create Request rights can create Requests. Please refer
Roles (Users) in the Administration Manual.

1. Log in to the Technician Portal. Hover your mouse over the **Create**
   button in one of the Navigation Tabs. You see a popup menu; click on
   **Request**.

.. _rmf-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-1.png
    :align: center
    :alt: figure 1

2. The **Create-a-Request** dialog box opens.

.. _rmf-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-2.png
    :align: center
    :alt: figure 2

.. _rmf-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/request-management/RM-3.png
    :align: center
    :alt: figure 3

3. You have to set a Request Category in section-A (:numref:`rmf-2`). It is a
   way to categorize Requests. The product has two predefined Categories
   (:doc:`Incident and Service Requests <introduction-request-management>`) to choose
   from, and you can add more categories. Each category can have
   Sub-Categories, up to three levels. Please refer Request Category
   (Helpdesk) in the Administration Manual to learn how to add
   Categories and Sub-Categories.

   The dialog box highlights the selected Category in the Category field
   in section-B (:numref:`rmf-2`).

4. You can fill the form using a template which is a quicker way to
   submit Requests that are recurring or part of a Service Request
   catalog. Section-B has the field that lets you populate the form from
   a custom template.

   You can manage custom templates from **Request Templates** (Helpdesk)
   in **Admin**. Please refer the Administration Manual on how to add
   templates.

   .. note:: The person who creates Templates must have administrative rights.

   Loading a custom Template (if any) performs the following changes:

   a. It populates the Subject of the Request.

   b. It configures the following classifiers of the Request:

      i.   Priority of the Request.

      ii.  Urgency level of the Request.

      iii. Impact of the Request on the organization.

   c. It can add Tags to the Request.

   d. It can add a Description.

5. In section-C, you need to add the Requestor email and name (Requestor
   Email ID and Requestor Name). You cannot create a Request with an
   unauthenticated email. You have to ask an Administrator to enable
   Request creation without login to do so.

   You can add other emails using **Add Cc Email**. That adds them to
   the Watcher list, which means they get notifications that the
   Requestor gets.

6. In section-D, you add the Subject line that gives a brief
   introduction to the Request. If you use a Template, the field
   auto-populates. Else, you have to fill it yourself because it is a
   mandatory field.

7. In section-E, you set the Status, Priority, Urgency, and Impact. This
   data is vital for tracking and managing Requests.

   If you are not using a template, then you have to set them manually
   according to your requirements.

   Tags are optional identifiers that you can add. You can add multiple
   tags if you want.

8. Section-F is the Description area where you write a detailed
   explanation of the Request. It should talk about the symptoms that
   lead to the Request. You can attach additional documents to support
   the resolution process in section-H.

9. In section-G&H, you can add Technician Group, Location, and
   Department. These fields have a drop-down list of values predefined
   by an Administrator; you just need to select the appropriate values.

   Please refer the Administration Manual to know more about the fields.

10. Hit **Create** when you are done filling the form. Now you have
    successfully created your Request. An email is sent to the Requester
    acknowledging the Request.

**Email to ticket**

Flotomate gives the option to set up an email as the Helpdesk email
address. Technicians can send an email to create a Request.

The question, who can create a Request, depends on the **Helpdesk**
settings in the **Admin** section. If settings allow creating Requests
without login, then anyone with the Helpdesk email can create a Request.
Else, the system accepts email Requests from registered emails only.

When a Technician creates a Request using an email, the email subject
becomes the Request Subject, email body becomes the Request Description,
and any attachments become the Request attachment.