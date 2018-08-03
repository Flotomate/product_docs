******************************
Setting Up a Deployment Policy
******************************

A deployment policy is created to control how a Deployment Request actually carries 
out the deployment of Patches. A user can create multiple policies and select any one of those when creating a Deployment Request.

A Deployment Policy uses fine-grained configurations to control
deployment initiation, reboot policy, user interaction, and
notifications.

**Adding a Deployment Policy**

1. Click on the **Launcher** icon and select **Patch**.

2. Select Deployment Policy from the Patch menu.

.. _pf-38:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-38.png
   :align: center
   :alt: figure 38

3. The Deployment Policies page opens. Here you can view all your
   policies that you create. Click on **Create Deployment Policy**
   situated in the top right corner of the page.

.. _pf-39:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-39.png
   :align: center
   :alt: figure 39

4. The Create Deployment Policy dialog box opens. You get the following
   fields:

.. _pf-40:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-40.png
   :align: center
   :alt: figure 40
::
    a. **Name**: This field allows you to give a name to the policy.

    b. **Apply on Every Startup**: You can instruct the product server to send command to a Computer on every startup.

    c. **Initiate Policy**: You can instruct Computers to install the Patches immediately or during a system startup.

    d. **Reboot Policy**: You can instruct Computers to perform a reboot, shutdown or do nothing after a successful installation.

    e. **Allow-user-to-skip-deployment**: Do you want to give the users of Computers the option to skip a deployment?

    f. **Notify-user-before-deployment**: Do you want to notify the users of Computers before a deployment. 
       If you select **Yes,** then two new fields appear where you have to add a title and a message for the users.
   
5.  Fill in the fields and click **Add** to add the policy to the product list 
    of Deployment Policies.

**Edit a policy:**

-  Go to the Deployment Policy page.

-  Click on the Edit Icon adjacent to the policy which you want to edit.

-  Click on **Update** after performing the edits.

**Delete a policy:**

In the Deployment Policy page, click on the Delete Icon adjacent to the
policy that you want to delete. A confirmation box opens whereby
selecting Yes deletes the policy permanently.

.. note:: You cannot delete a policy if it is associated with a Deployment Request. You have to delete the request first then the policy.