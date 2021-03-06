.. _add-endpoint-scope:

**************
Endpoint Scope
**************

Depending on the License agreement you have with us, the number of
Computers you can manage for Patch/Packages/Registry is
limited. All discovered Computers (with our Agent application) stay out
of the scope (target) of Remote Deployment by default; you have to bring them within
the scope (target).

The Endpoint Scope lets you view all available Computers (both in and out of Endpoint Scope) and add them to the scope of Remote Deployment. 
You can set certain conditions that will allow the main server to add any new Computers automatically to the scope. You can also
add Computers manually.

There is a counter on the Endpoint Scope page that shows how many Computers are allowed within the scope. 
In no situation, you can exceed the mentioned number.

.. note:: Only Computers configured with our Agent Application are visible in the Endpoint Scope page.

.. _add-computer-scope:

Add Computers to a Scope
========================

-  Go to **Admin** (a Navigation Tab) >> **Endpoint Scope**
   (Patch/Package Management).

.. _P-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-1.png
   :align: center
   :alt: figure 1

-  The Endpoint Scope page opens.

.. _P-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-2.png
   :align: center
   :alt: figure 2

-  You can view the total number of Computers that you can add as
   *Total Endpoints in Scope* number. 

.. _P-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-3.png
   :align: center
   :alt: figure 3

.. _add-remote-office:   

Adding a Remote Office (Automatic Addition of Computers)
--------------------------------------------------------

-  You can associate a :doc:`Remote Office <remote-office>` with a Scope (target); this allows the Scope (target) to
   automatically add Computers (with the Agent application) in the
   Remote Office based on include and exclude conditions. You can use both
   manual and automatic addition of Computers together; they are not
   mutually exclusive.

   .. note:: Related Topic: :doc:`Remote Office <remote-office>`

.. _P-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-4.png
   :align: center
   :alt: figure 4

-  Once you select a Remote Office, you can add conditions. The
   conditions are of two types: include and exclude. Both the types
   create a set of Computers from which to either include or exclude.
   When there’s an intersection or conflict between the two types then
   exclude conditions/condition override the include set. For example,
   to add Computers within an IP range and with a hostname containing “Digit”
   , and excluding those with "Vector" in their Hostname, yields the following conditions (refer: :numref:`P-5.2`):

   .. note:: Without include and exclude conditions, all Computers in a Remote office will be added.

.. _P-5.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-5.1.png
   :align: center
   :alt: figure 5.1

.. _P-5.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-5.2.png
   :align: center
   :alt: figure 5.2

Adding of Computers from List
-----------------------------

-  You can manually search and add Computers to a scope (target). The search bar
   supports the Advanced Search feature where you get search options by
   clicking on the search bar.

.. _P-6.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-6.1.png
   :align: center
   :alt: figure 6.1

.. _P-6.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-6.2.png
   :align: center
   :alt: figure 6.2

::
    You can also enter keywords to search for a Computer. When entering a
    keyword, the product explores all the Computers with the keyword in
    their Name, Hostname, Domain name, OS name and Service Pack. A Computer
    has to have at least one field matched (partial or full) with the
    keyword; in case there are multiple keywords, a Computer has to have at
    least one field matched for each keyword.

    You can combine search options with keywords. Between two different
    conditions of the same type OR logic is followed. Between different
    types AND logic is observed. An example of same type contradiction is Network
    equals Windows vs. OS Network equals Dell-Servers. Between keywords and conditions AND logic is followed.

.. _P-7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-7.png
   :align: center
   :alt: figure 7

-  Once you have found your Computers, add by selecting them, and they
   move to the Selected Computers list. Manually selected Computers
   override the exclude criteria/conditions set for the Remote Office.

.. _P-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-8.png
   :align: center
   :alt: figure 8

-  Once you are done setting conditions and adding Computers, click on
   **Update**.

.. _endpoint-scope:

Adding Multiple Scopes
----------------------

-  You can create more than one Scope (target) to accommodate multiple Remote Offices
   (a Scope can have only one Remote Office). The actual Endpoint Computer list is
   cumulative of all available Scopes (added manually and
   automatically).

.. _P-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-9.png
   :align: center
   :alt: figure 9

.. _P-9.1.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-9.1.1.png
   :align: center
   :alt: figure 9.1.1   

.. _preview-scope-list:

Preview Computer List
=====================

Once you are done with adding Computers and setting conditions, you can
view the final list of all the Computers in all the Scopes (targets) and also individual scopes using the Preview function.

Open Endpoint Scope from **Admin**. Click on **Preview** to generate the
Computer list. The preview button is also there for each scope.

.. _P-9.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-9.1.png
   :align: center
   :alt: figure 9.1

.. _P-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/patch-management/P-10.png
   :align: center
   :alt: figure 10

You can search for a Computer. The search bar supports the Advanced
Search feature. It is similar to the search bar in a :ref:`Scope <endpoint-scope>`.     