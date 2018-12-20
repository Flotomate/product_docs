******************
Creating a Request 
******************

There are multitude of ways to create a Request (Incident) in our Helpdesk product. 
Technicians can create Requests using the email to ticket feature or they can use
the Create a Request dialog box.

The Create a Request dialog box is available on both the Requestor and
Technician Portal. However, the Create a Request form on the Technician
portal is different. It has additional fields that are specific to the
needs of a Technician.

Only people with create Request rights can create Requests. Please refer
:ref:`Roles <admin-user-management>` (Users) in the Administration Manual.

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

3. You have to set a Request Category in section-A (:numref:`rmf-2`). It helps to categorize a Request. 
   The product has two predefined Categories (:doc:`Incident and Service Requests <introduction-request-management>`) 
   to choose from, and you can add more categories. Each category can have
   Sub-Categories, up to three levels. Please refer :ref:`Request Category<ad-category>`
   (Helpdesk) in the Administration Manual to learn how to add
   Categories and Sub-Categories.

   The dialog box highlights the selected Category in the Category field
   in section-B (:numref:`rmf-2`).

4. You can fill the form using a template which is a quicker way to
   submit Requests that are recurring in nature. Section-B has the field that lets you populate the form from
   a custom template.

   You can manage custom templates from :ref:`Request Templates<ad-templates>` (Helpdesk)
   in **Admin**. Please refer the Administration Manual on how to add
   templates.

   .. note:: The person who creates Templates must have administrative rights.

   Loading a custom Template (if any) performs the following changes:

   a. It populates the Subject of the Request.

   b. It configures the following classifiers of the Request:

      i.  Urgency level of the Request.

      ii. Impact of the Request on the organization.

   c. It can add Tags to the Request.

   d. It can add a category and Requestor Account.

   e. It can add a Description.

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

7. In section-E, you set the Urgency, Impact and Tags. This
   data is vital for tracking and managing Requests.

   If you are using a template, then you don't have to set them manually.

   Tags are optional identifiers that you can add. You can add multiple
   tags if you want.

8. Section-F is the Description area where you write a detailed
   explanation of the Request. It should talk about the symptoms that
   lead to the Request. You can attach additional documents to support
   the resolution process in section-I.

9. In section-G, you can add a Technician Group, Location,
   Department and Requestor Accounts. These fields have a drop-down list of values predefined
   by an Administrator; you just need to select the appropriate values.

   Please refer the Administration Manual to know more about the :doc:`fields<admin-customization>`.

10. Fields in section-H are custom fields. You can add n number of fields from the admin section. 
    You can control the visibility of such fields. Learn how to create a :ref:`Request Custom Field<ad-custom-fields>`.    

11. Hit **Create** when you are done filling the form. Now you have
    successfully created your Request. An email is sent to the Requestor
    acknowledging the Request.

**Email to ticket**

Flotomate gives the option to set up an email as the Helpdesk email
address. Technicians can send an email to create a Request.

The question, who can create a Request, depends on the **Helpdesk Security (Users)**
settings in the **Admin** section. If settings allow creating Requests
without login (**Allow Guest Requester to Report a Request**) and email to ticket feature is allowed in **Email Server Configuration**, 
then anyone with the Helpdesk email can create a Request.
Else, the system accepts email Requests from registered emails only.

When a Technician creates a Request using an email, the email subject
becomes the Request Subject, email body becomes the Request Description,
and any attachments become the Request attachment.