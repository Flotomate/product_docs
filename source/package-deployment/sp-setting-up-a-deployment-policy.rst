******************************
Setting Up a Deployment Policy
******************************

A deployment policy is created to control how a Deployment Request
.actually carries out the deployment of packages/registry entries. A
user can create multiple policies and select any one of those when
creating a Deployment Request.

A Deployment Policy uses fine-grained configurations to control
deployment initiation, reboot policy, user interaction, and
notifications.

**Adding a Deployment Policy**

1. Click on the **Launcher** icon and select **Package**.

2. Select **Deployment Policy** from the Package Menu.

.. _spf-28:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-28.png
    :align: center
    :alt: figure 28

3. The Deployment Policies page opens. Here you can view all your
   policies that you create. Click on **Create Deployment Policy**
   situated in the top right corner of the page.

.. _spf-29:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-29.png
    :align: center
    :alt: figure 29

4. The Create Deployment Policy dialog box opens. You get the following
   fields:

    .. _spf-30:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-30.png
        :align: center
        :alt: figure 30

   a. **Name**: This field allows you to give a name to the policy.

   b. **Apply on Every Start-up:** Checking this option makes the policy
      initiate a deployment via a request in a computer every time it boots
      up.

   c. **Initiate Policy**: You can instruct Computers to install the
      packages or perform registry deployment immediately (while the system
      is running) or during a system startup.

   d. **Reboot Policy**: You can instruct Computers to perform a reboot,
      shutdown or do nothing after a successful installation or deployment.

   e. **Allow-user-to-skip-deployment**: Do you want to give the users of
      Computers the option to skip a deployment?

   f. **Notify-user-before-deployment**: Do you want to notify the users of
      Computers before a deployment. If you select **Yes,** then two new
      fields appear where you have to add a title and a message for the
      users.

    .. _spf-31:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-31.png
        :align: center
        :alt: figure 31

   Fill in the fields and click **Add** to add the policy to the list of
   Deployment Policies.

**Edit a policy:**

-  Go to the :doc:`Deployment Policy <sp-setting-up-a-deployment-policy>`
   page.

-  Click on the Edit Icon adjacent to the policy which you want to edit.

-  Click on **Update** after performing the edits.

**Delete a policy:**

In the Deployment Policy page, click on the Delete Icon adjacent to the
policy that you want to delete. A confirmation box opens whereby
selecting Yes deletes the policy permanently.

.. note:: You cannot delete a policy if it is associated with a Deployment
          Request. You have to delete the request first then the policy.