********************
System Configuration
********************

Agent Self Upgrade
==================

Developing our Agent application is an ongoing process, which is why we
release a new version periodically. In every version, the application is
better compared to the previous either in terms of performance,
capabilities or both.

The Agent Self Upgrade feature allows for a smooth transition from one
version of the Agent to another. Using this feature, an admin can
centrally deploy an Agent.exe from the product server, which is received
by all the (active) computers in the :ref:`Endpoint
scope <endpoint-scope>`. The received **agent.exe** auto-installs
itself during the next boot cycle.

Some of the benefits of using the latest version of the Agent
application:

-  Newer versions of the Agent are more stable and give better
   performance.

-  Upgrading gives you more capabilities/features.

-  Upgrading to a newer version eliminates possible security flaws.

Initiating an Upgrade Request:
------------------------------

-  Go to the **Admin** (A Navigation Tab) >> **Agent Self Upgrade**
   (Systems).

.. _adf-149:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-149.png
    :align: center
    :alt: figure 149

-  The Agent Self Upgrade page opens. Here you can view all your
   existing requests. To create a new one, click on **Create Upgrade
   Request** situated in the top right corner.

-  A new dialog box opens with the following fields:

    .. _adf-150:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-150.png
        :align: center
        :alt: figure 150

    a. In section A, you give a name to the request. You can search for a
       request by its name in the Agent Self Upgrade page.

    b. You write the Agent version in section B that you are going to
       deploy.

    c. In section C, you select a platform (either Windows or Linux).

    d. Select an architecture in section D.

    e. You attach the exe file of the Agent in section E.

    f. Write a description of the new Agent in section F.

   When you are done, click on **Create**. The main server immediately
   activates the request.

Rejecting an Upgrade Request
----------------------------

You can reject an already published upgrade request in the following
way:

-  Open Agent Self Upgrade page from Admin.

-  Click on the **Reject** button adjacent to the request that you want
   to stop.

.. _adf-151:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-151.png
    :align: center
    :alt: figure 151

-  On confirmation, the server stops sending the command for upgrade to
   all computers in the scope. Computers that have already upgraded stay
   unaffected.