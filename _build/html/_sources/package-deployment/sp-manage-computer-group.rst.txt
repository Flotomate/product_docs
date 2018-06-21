**********************
Manage Computer Groups
**********************

You can classify Computers into groups. Some of the use cases where
having Computer Groups can be convenient are as follows:

-  You want to deploy packages in Computers belonging to a particular
   department. You can create a Computer Group having all the Computers
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

-  A new page opens. Here you can view all the Computers added to the
   :doc:`Endpoint scope <configuring-endpoint-scope>`. You get options to
   select Computers manually and automatically from a Network (based on
   include and exclude conditions).

.. _spf-12:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-12.png
    :align: center
    :alt: figure 12

-  Provide a name to the Computer Group.

-  In whatever way you select Computers, they all become part of the
   group. The manual and automatic methods of selection are similar to
   the ones used for adding Computers to an :doc:`Endpoint
   Scope <configuring-endpoint-scope>`.

-  Add the Computers and click on **Create** to save the group.

-  You can review the Computer list of a group from the Computer Group
   page.

.. _spf-13.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-13.1.png
    :align: center
    :alt: figure 13.1

.. _spf-13.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-13.2.png
    :align: center
    :alt: figure 13.2

-  You can search a Computer Group list using a search bar (:numref:`spf-13`)
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

When a group is archived (delete), we store the group details in a
separate section for future reference. It is because even when a group
gets deleted, it stays active in associated Deployment Requests.

You can view all archived groups in the Computer Group page by clicking
**Archive Computer Group** button situated in the top right corner. You
can also preview the Computer list of an archived group.