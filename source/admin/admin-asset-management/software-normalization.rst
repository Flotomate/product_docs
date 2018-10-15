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

- Sometimes users want to control the kind of software that can be installed in their Computers and what can't. 
  And, they expect notifications of un-authorized event of installation. In this situation, one can mark all unauthorized Software
  as Prohibited (black list). Whenever, a Prohibited Software is discovered a notification is sent to the user and admin. 

How to Set Software Normalization
=================================

A user can create Normalization rules that can have two kinds of actions:

1. Upon trigger, Normalization sets certain field values of a Software Asset. For example, adding a Product
   to a Software Asset.

2. Upon trigger, Normalization consolidates all Software, satisfying the Normalization rules, into a single suit. 

Create a Normalization for Field Assignment
-------------------------------------------

- Go to **Admin** >> **Software Normalization** (under Asset Management).

.. _ad-n-1:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-1.png
    :align: center
    :alt: figure 1

- In the Software Normalization page, the **Field Assignment Rules** tab shows existing rules that does field assignment.
  Click on **Create a Normalization Rule** to make a new one.

.. _ad-n-2:

.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-2.png
    :align: center
    :alt: figure 2

- In the new page you have to create the rule:

    .. _ad-n-3:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/admin/AD-N-3.png
        :align: center
        :alt: figure 3

  Here we create a rule that automatically sets Software Type as Managed of Software Asset with Product equals Adobe, and for that
  we input the following.

  - "Change Software Type" as the name of the rule.

  - Rule type as Field Assignment.

  - We set the condition as *Product Equals to Adobe*; this means the rule is applicable on Software Asset with Product as Adobe. 
    Learn how to set complex condition statements.

  - We add an action: *Set Software Type to Managed*. The set action will be performed when the rule is triggered.

  - We set the execution priority as High. 

  