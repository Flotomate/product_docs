****************************************************
Manage Computer Groups (Package/Registry Deployment)
****************************************************

You can classify Computers into groups. Some of the use cases where
having Computer Groups can be convenient are as follows:

-  You want to deploy packages in Computers belonging to a particular
   department of a Remote Office. You can create a Computer Group having all the Computers
   of that department and quickly create a Deployment Request with that
   group.

-  If you want to deny a specific set of Computers of packages, then you
   can create a Computer Group and decline them the packages.

**Create a Computer Group**

-  Go to the Package/Registry List View.

-  Click on **All Computers Group** from the Package menu.

.. _spf-11:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-11.png
    :align: center
    :alt: figure 11

-  The Computer Group page opens. Here you can view all existing groups
   if any. Click on **Create Computer Group** situated in the top right
   corner of the page.

-  A new page opens. Here you can view all the Computers in the
   :doc:`Endpoint scope <configuring-endpoint-scope>`. You get options to
   select Computers manually and automatically from a Remote Office (which can be filtered using
   include and exclude conditions).

.. _spf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-12.png
    :align: center
    :alt: figure 12

-  In :numref:`SP-12`, enter a name and description of the group.

-  In whatever way you select Computers, they all become part of the
   group. Add a remote office to the first scope (if you want Computers from the Remote Office to be added automatically). 
   Learn how to add a :ref:`Remote Office <add-remote-office>`. 

-  You can add additional computers from the list, if any. By the way, you can create a group without a Remote office by selecting computers from the
   given list. Learn how to add :ref:`Additional Computers <Adding of Computers from List>`

-  You can create multiple scopes, each having their own Remote Office and additional computers, and the group will be
   a cumulative of all the Scopes. Learn more about :ref:`Scopes <endpoint-scope>`.   

-  When done, click on **Create** to save the group.

You can review computers in each Scope before adding them to a group. You also preview computers of a group (after creation) from 
Computer Group page.

.. _spf-13.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-13.1.png
    :align: center
    :alt: figure 13.1

.. _spf-13.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-13.2.png
    :align: center
    :alt: figure 13.2

.. _spf-13.3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-13.3.png
    :align: center
    :alt: figure 13.3    

You can search the preview list of a Group and Scope using a search bar (:numref:`spf-13.3`)
that supports Advance Search and is similar to the one used for
searching Computers in an :doc:`Endpoint
Scope <configuring-endpoint-scope>`. You can open the details of
any Computer by click on it.

**Edit/Delete Groups**

You can edit and delete any Computer Group.

.. _spf-14:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-14.png
    :align: center
    :alt: figure 14


View Archived Groups
====================

When a group is deleted, we store the group in a separate
section for future reference. It is because even when a group gets
deleted, it stays active in associated Deployment Requests.

You can view all archived groups in the Computer Group page by clicking on
**Archive Computer Group** (refer :numref:`P-14`). You
can also preview the Computer list of an archived group.