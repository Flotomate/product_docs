************
Organization
************

Flotomate allows you to maintain company details in the product in the
following forms:

-  Account

-  Department information

-  Location details

-  Business hours

-  Branding

.. _ad-account:

Account 
=======

Flotomate has the account section where you can maintain the company’s
profile.

.. note:: Managing company details requires you to have Administrative
          rights.

- Go to **Admin** from the Navigation Tabs.

- Search **Account** in the search bar or you can find **Account** under 
  Organization. Click on **Account**; it opens the Account page.

The Account page is divided in to three sections; they are as follows:  

**Profile**

.. _adf-78:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-78.png
    :align: center
    :alt: figure 78

- Click **Edit** situated in the top right corner of the display area.
  The Profile fields become editable.

- You can enter the following information:

    a. Name of the company.

    b. Email of the company.

    c. Contact number of the company.

    d. Number of people employed by the company.

    e. Registered address of the company.

    f. Description of the company.

    g. Website URL of the company.

    h. Time zone of the company.

    i. Base currency in which the organization does all its transactions. When required, the base currency is converted against a
       foreign currency in the system list (Learn how to add a :ref:`Currency <Adding a Currency>`)

    j. The Activation Code in use is visible here.  

- Once you are done inputting data, click on **Update** to save the
  information.

You can edit the profile any time using the **Edit** option in the same
way you created your profile.

**License Information**

How much you can use our product is decided by the type of license you have.
In this section, you can view all license related information.

.. _adf-78.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-78.1.png
    :align: center
    :alt: figure 78.1

- Here you can view vital information about the License; for example,
  license type, number of Agents you can use, number of Assets you can discover, etc.

- You can access additional information about the license from the Action Menu.

.. _adf-78.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-78.2.png
    :align: center
    :alt: figure 78.2

**Version**

Here you can view the version details of the product. The details are automatically updated after every release.

.. _adf-78.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-78.3.png
    :align: center
    :alt: figure 78.3

.. _ad-departments:

Departments
===========

Flotomate allows you to add your organization’s department names and
sub-departments in the product. Each department can have sub-departments
up to level three.

Some of the benefits of having department names in the product are:

-  You can classify tickets, Assets, Projects and users by department.

-  You can create automated workflows using department as a condition.

-  You can create Requestor Groups by using department names.

-  You can generate department specific reports.

.. note:: Managing company departments requires you to have Administrative
          rights

**Add a Department**

.. note:: System Department is different from the Requestor Department,
          which is imported from the LDAP servers.

-  Go to **Admin** from the Navigation Tabs and click **Departments**
   under Organization. You can see all your available departments in the
   new page if any.

.. _adf-79:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-79.png
    :align: center
    :alt: figure 79

-  Use the **Add** button to add departments. The leftmost column has
   the level one departments, and all others columns have the
   sub-departments. Clicking on a department name activates the adjacent
   column, where sub-departments can be added, edited and viewed.

.. _adf-80:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-80.png
    :align: center
    :alt: figure 80

-  You can change the name of a department by clicking on the **Edit
   Icon**. Clicking on the Edit Icon opens a dialog box where you enter
   the new name and update.

-  Use the Delete Icon to delete any department.

Business Hours
==============

You can define the working hours of your organization in the product.
You can have separate working hours for each of your departments, and
you can even add all your holidays in a year.

Having a business hour/hours helps the product in determining the
available response time and resolution time of a Request (holidays are
subtracted from the calculation). These calculations are done to see
whether any SLAs have been violated or not. Of course, the SLAs have to
be configured to use business hours.

Learn more about :ref:`SLA <managing sla>`.

To add business hours:

1. Go to **Admin** >> **Business Hours** (Organization).

2. Business Hours page opens. Here you can set the business hours if
   any.

3. Click **Add Business Hour** situated in the top right corner of the
   page.

.. _adf-81:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-81.png
    :align: center
    :alt: figure 81

4. In the **Add Business Hour** dialog box, select the department (you
   can also select a sub-department) for which you want to set time.
   Give a name to the time profile.

5. You can set the business hours as default.

6. We have two options for setting working hours: **24hrs x 7days** and
   **Custom hours**. You can select any one of them.

    To set custom hours:

    a. Click **Custom hours**; you get a list of all days with a start
       and end time.

        .. _adf-82:
        .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-82.png
            :align: center
            :alt: figure 82

    b. Select the days that are applicable and set the start and end time.

6. Set holidays and write a small description. Click **Add** to add
   your new business hours.

.. _ad-location:

Location 
========

You can add your business location/locations in Flotomate along with the
time zone/zones. :ref:`business hours <business hours>` are auto configured based on the time zone of
each location.

Some benefits of having locations:

-  You can set a time zone for your business hours.

-  You can classify and segregate (:ref:`learn more <Data Segregation with Location Scope>`) tickets, Assets, and Projects by location.

-  You can create location specific Reports.

.. note:: changing Location settings require administrative rights.

**Add Location**

-  Go to the **Admin** from the Navigation Bar and click **Location**
   under Organization.

-  Location page opens. Here you can view the present locations in the
   system if any. Click **Add New** situated in the top right corner of
   the page.

.. _adf-83:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-83.png
    :align: center
    :alt: figure 83

-  Add Location dialog box opens. There you can input the following
   details:

   a. Name of the location.

   b. Country name.

   c. Time Zone of the location.

   d. Business Hours from a drop-down list.

   e. Address of the location.

   f. Description of the location.

   Fill in the details and hit **Save**.

-  Click on the Edit Icon adjacent to the Location that you want to
   change.

-  Edit Location dialog box opens where you have to make the changes.
   Don’t forget to save your changes.

-  You can delete a Location by clicking on the adjacent Delete Icon. On
   confirmation, the system deletes the location.

Branding
========

Flotomate allows you to upload brand assets like logo and Favicon; you
can customize the looks of the product so that people using the product
can identify the service as part of their organization.

.. note:: Editing brand information requires administrative rights.

**Add/Edit Branding Information**

-  Go to the **Admin** from the Navigation Bar and click **Branding**
   under Organization. The Branding page opens.

.. _adf-84:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-84.png
    :align: center
    :alt: figure 84

-  Add the Brand Text, Brand Logo, and Brand Favicon. You can toggle
   between logo and text, whichever way you want to show your identity
   on Flotomate (top left corner of the screen).

-  Set the Primary, Secondary and Logo Background colors. You can choose
   the text color to be primary or secondary. Whichever you choose as
   the text color, the other option becomes the background color; except
   when you have a logo, the Logo Background Color is selected as the
   only color.

-  You can set a name for the customer and technician portals. You can
   provide contact details in the form of email and phone number.

-  **Update** your changes when you are done. You can edit your Branding
   details anytime you want.