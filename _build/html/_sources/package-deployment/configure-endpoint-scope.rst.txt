**************************
Configuring Endpoint Scope
**************************

Depending on the License agreement you have with us, the number of
Computers you can manage with the product is limited. All discovered
Computers (with our Agent application) stay out of the scope of the main
server by default; you have to bring them within the scope before you
can use package management.

The Endpoint Scope lets you view all available Computers (not in the
Scope) and add them to the Scope. You can set certain conditions that
allow the product to add any new Computer automatically. You can also
add Computers manually.

There is a counter that shows how many Computers are within the scope
and how many you can still add. In no situation, you can exceed the
total number of Computers you are allowed to add to the Scope.

.. note:: Only Computers configured with our Agent application is visible
          on Endpoint Scope page.

Add Computers to a Scope
========================

-  Go to **Admin** (a Navigation Tab) >> **Endpoint Scope**
   (Patch/Package Management).

.. _spf-1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-1.png
    :align: center
    :alt: figure 1

-  The Endpoint Scope page opens.

.. _spf-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-2.png
    :align: center
    :alt: figure 2

-  You can view the total number of Computers that you can add from the
   Total Endpoint Scope number. The Total Available shows you the number
   of Computers you can still add to reach the Total Endpoint Scope
   number.

.. _spf-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-3.png
    :align: center
    :alt: figure 3

**Adding a Network (Automatic Addition of Computers)**

-  You can associate a Network with a Scope; this allows the Scope to
   automatically add Computers (with the Agent application) in the
   Network based on include and exclude conditions. You can use both
   manual and automatic addition of Computers together; they are not
   mutually exclusive.

.. _spf-4:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-4.png
    :align: center
    :alt: figure 4

-  Once you select a Network, you now have to add conditions. The
   conditions are of two types: include and exclude. Both the types
   create a set of Computers from which to either include or exclude.
   When there’s an intersection or conflict between the two types, then
   exclude conditions/condition override the included set. For example,
   to add Computers within an IP range with a hostname containing “Digi”
   and excluding those with Linux OS, yields the following conditions:

.. _spf-5.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-5.1.png
    :align: center
    :alt: figure 5.1

.. _spf-5.2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-5.2.png
    :align: center
    :alt: figure 5.2

**Manual Adding Computers**

-  You can manually search and add Computers to a scope. The search bar
   supports the Advanced Search feature where you get search options by
   clicking on the search bar.

    .. _spf-6.1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-6.1.png
        :align: center
        :alt: figure 6.1

    .. _spf-6.2:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-6.2.png
        :align: center
        :alt: figure 6.2

   You can also enter keywords to search for a Computer. When entering a
   keyword, the product explores all the Computers with the keyword in
   their Name, Hostname, Domain name, OS name and Service Pack. A Computer
   has to have at least one field matched (partial or full) with the
   keyword; in case there are multiple keywords, a Computer has to have at
   least one field matched for each keyword.

   You can combine search options with keywords. Between two different
   conditions of the same type OR logic is followed. Between different
   types AND logic is observed. An example of same type contradiction is OS
   Name contains Windows vs. OS Name contains Linux.

.. _spf-7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-7.png
    :align: center
    :alt: figure 7

-  Once you have found your Computers, add by selecting them, and they
   move to the Selected Computers list. Manually selected Computers
   override the exclude criteria/conditions set under the Network.

.. _spf-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-8.png
    :align: center
    :alt: figure 8

-  Once you are done setting conditions and adding Computers, click on
   **Update**.

-  You can create more than one Scope to accommodate multiple Networks
   (a Scope can have only one Network). The actual Computer list is
   cumulative of all available Scopes (added manually and
   automatically).

.. _spf-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-9.png
    :align: center
    :alt: figure 9

Preview Computer List
=====================

Once you are done with adding Computers and setting conditions, you can
view the final list of all the Computers (added manually and
automatically) in all Scopes using the Preview function.

Open Endpoint Scope from **Admin**. Click on **Preview** to generate the
Computer list.

.. _spf-10:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-10.png
    :align: center
    :alt: figure 10

You can search for a Computer. The search bar supports the Advanced
Search feature. It is similar to the search bar in a
:ref:`Scope <add-computers-to-a-scope>`.