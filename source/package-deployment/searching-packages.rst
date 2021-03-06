*************************************
Searching Packages/Registry Templates
*************************************

There are two broad ways to search in the Deployment :doc:`List View <package-registry-list-view>`:

-  Using a Search Bar

-  Using Filters

.. _sp-search-bar:

Search Bar
==========

The way the search bar works is same for Windows and Ubuntu Linux Package List
View. The search bar in the Windows Registry view is different.

The :doc:`Package/Registry List View <package-registry-list-view>` has a
search bar. The search bar (for Windows and Ubuntu Linux Package List View)
supports the Advanced Search feature where you get a set of predefined
search options to narrow down your searches. If you want to see all the
available options, then click on the search box. You can select a single
option or multiple options from the drop-down list.

.. _spf-19:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-19.png
    :align: center
    :alt: figure 19

You can also search with keywords in the search field. When you provide
a keyword, Motadata explores all the packages with the keyword in their
ID, Name, Description, Display Name, and Version; and for registry
templates, ID, Sub-key, Value Name, Name, and Description. A
package/template has to have at least one field matched (partial or
full) with the keyword; in case there are multiple keywords, a
package/template has to have at least one field matched for each
keyword.

A search query (for packages) can be made up of pre-defined options and
keywords. In any case, the output yields packages that satisfy all the
parameters of the search query.

Between two different conditions of the same option type OR logic is
followed. Between different types AND logic is observed. Between
keywords, and keywords and conditions AND logic is followed. An example
of same option type contradiction is Package Type equals Application
Patch vs. Package Type equals Operating System.

.. _spf-20:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-20.png
    :align: center
    :alt: figure 20

Custom Filters (Applicable on Package List Views)
-------------------------------------------------

You can make a filter using search options and keywords and save it by
clicking on the star icon to the far left of the search bar. Saved
search filters appear along with the platform-specific filters in :numref:`spf-21.1`. 
Custom filters are specific to a particular platform.

For example, a user saves a search query that filters packages with
Package Type: Application Patch and the keyword Deamon.

.. _spf-21.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-21.1.png
    :align: center
    :alt: figure 21.1

.. _spf-21.2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-21.2.png
    :align: center
    :alt: figure 21.2

Making a Filter as Default
^^^^^^^^^^^^^^^^^^^^^^^^^^

You can make a filter as default for the option Packages from the Deployment menu. The default filter opens when someone clicks
on Package from the menu.

.. _spf-21.2.1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-21.2.1.png
    :align: center
    :alt: figure 21.2.1

Searching Registry Templates
----------------------------

Search box on the :ref:`Registry Template List View <Windows Registry templates>` supports only keywords based searches.

.. _spf-21.3:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-21.3.png
    :align: center
    :alt: figure 21.3

Filters
=======

There are three primary filters available to sort packages and registry
templates in the product:

-  You can isolate packages for Windows and Ubuntu Linux from the Packages List View, and registry
   templates from the Package Menu. You can access the Package Menu from
   the :doc:`Launcher icon <package-registry-list-view>`.

.. _spf-22:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-22.png
    :align: center
    :alt: figure 22

-  In the :doc:`Package List View <package-registry-list-view>`, you can
   perform the following segregation:

   a. Segregate packages based on architecture type (32bit or 64bit).

    .. _spf-23:

    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-23.png
        :align: center
        :alt: figure 23

   b. Segregate packages based on Package type.

    .. _spf-24:
    
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/software-package-deployment/SP-24.png
        :align: center
        :alt: figure 24
