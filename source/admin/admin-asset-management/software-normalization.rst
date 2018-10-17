**********************
Software Normalization
**********************

Software Normalization is a rules based automation that does the following:

- Change of Software Asset details when certain set condition/conditions are triggered. 

- Consolidating Software that fulfill certain conditions.

- Control Software installation type by putting Software either in white list or black list (Prohibited Software). 

Software Normalization can be useful in the following scenarios:

- In reality, most of our users are not interested in managing each and every Software Asset discovered. They want to manage 
  a small set of Software Assets mainly for the purpose of compliance management. Here Software Normalization can be used 
  to change Software Type of Software satisfying certain predefined conditions. 

  Normalization can also be used to set Software Asset fields (i.e Product) upon discovery for better reporting and compliance management.

- Sometimes users want to control the kind of software that can be installed in their Computers and what can't be installed. 
  And, they expect notifications of an un-authorized instance of installation. In this situation, one can mark all unauthorized Software
  as Prohibited (black list). Whenever, a Prohibited Software is discovered a notification is sent to the user and admin. 

Setting Software Normalization
==============================

A user can create Normalization rules that can have two kinds of actions:

1. Upon trigger, Normalization sets certain field values of a Software Asset. For example, adding a Product
   to a Software Asset.

2. Upon trigger, Normalization consolidates all Software, satisfying the Normalization rules, into a single suit. 

Create a Normalization Rule for Field Assignment
------------------------------------------------

- Go to **Admin** >> **Software Normalization** (under Asset Management).

.. _ad-n-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-1.png
    :align: center
    :alt: figure 1

- In the Software Normalization page, the **Field Assignment Rules** tab shows existing rules for field assignment.
  Click on **Create a Normalization Rule** to make a new one.

.. _ad-n-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-2.png
    :align: center
    :alt: figure 2

- In the new page you have to create a rule:

    .. _ad-n-3:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-3.png
        :align: center
        :alt: figure 3

  Here we create a rule that automatically sets Software Type as Managed in Software Assets with Product equals Adobe, and for that
  we input the following.

  - "Change Software Type" as the name of the rule.

  - Rule type as Field Assignment.

  - We set the condition as *Product Equals to Adobe*; this means that the rule is applicable on Software Assets with Product as Adobe. 
    Learn how to set complex condition statements.

  - We add an action: *Set Software Type to Managed*. The set action will be performed when the rule is triggered.

  - We set the execution priority as High. In a scenario where multiple rules are applied to a single Software, the rules with the
    High priority are applied first, followed by the Medium and then the Low.

  - We turn on **Re-normalize on Next Run**. Turning this option allows Software that have been normalized under this rule
    to be available for re-normalization by another rule.

- When you are done creating a rule, click on **Create**.


Create a Normalization Rule for Suite
-------------------------------------

- Go to **Admin** >> **Software Normalization** (under Asset Management).

.. _ad-n-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-1.png
    :align: center
    :alt: figure 1

- In the Software Normalization page, the **Suite Rules** tab shows existing rules for creating Software suites.
  Click on **Create a Normalization Rule** to make a new one.

- In the new page you have to create a rule:

    .. _ad-n-4:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-4.png
        :align: center
        :alt: figure 4

  Here we create a rule that automatically adds Software to Microsoft Office 2013 (to make a suite) if the name contains the 
  keywords "Microsoft Office" or only "Office" in their name, and for that we input the following.

  - "MS Office Suite" as the name of the rule.

  - Rule type as **Suite**.

  - We set the condition as Name either contains "Microsoft Office" or only "Office".  

  - We add an action: **Add to Suite AST-69: Microsoft Office OSM UX MUI (English) 2013**. 

  - We set the execution priority as High. In a scenario where multiple rules are applied to a single Software, the rules with the
    High priority are applied first, followed by the Medium and then the Low.

  - We keep **Re-normalize on Next Run** turned off. Turning this option allows Software that have been normalized under this rule
    to be available for re-normalization by another rule.

- When you are done creating a rule, click on **Create**.

Software Installation Control Settings
--------------------------------------

Control settings allows you put all Software either in the Managed List or Prohibited List. You can access the settings from:
**Admin** >> **Software Normalization** >> **Software Installation Control Settings**. 

.. _ad-n-5:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-5.png
      :align: center
      :alt: figure 5

.. _ad-n-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-6.png
      :align: center
      :alt: figure 6

In the control settings dialog box, you get the following options:

- **Prohibited Software**: If selected then all Software except those with Type either Managed or Prohibited are marked as Prohibited.

- **Managed Software**: If selected then Software with type "None" are marked as Un-Identified.

Initiating Normalization
------------------------

A normalization rule is automatically triggered every 60 minutes. When a Software is eligible for multiple rules then rules with
priority **High** are applied first. A normalized Software can only be re-normalized when the rule that normalized the Software has
**Re-normalize on Next Run** option turned on. 

A user can initiate all Normalization rules at once from the :ref:`Software Asset List <Asset List View>` page.

.. _ad-n-7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-7.png
    :align: center
    :alt: figure 7

.. _ad-n-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-8.png
    :align: center
    :alt: figure 8

On clicking the option, a dialog box will ask, "you want to apply normalization in all asset?", here a user has two options:

- Clicking on **Yes** will apply all normalization rules on all Assets irrespective of whether they are normalized or not. 

- Clicking **No** will apply all normalization rules on Assets that are not normalized. 