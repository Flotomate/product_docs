****************************************************
Allocating Machines/Node/Users in a Software License 
****************************************************

.. note:: Here a machine is referred either to a Workstation, Laptop or Server Asset. A Node is referred to a Hardware Asset.

Allocation gives a machine/node/user, in the CMDB, the right to
install a Licensed Software. It lets Motadata keep a count of all valid
installations of a Licensed Software. The count is vital for activating
compliance specific notifications relating to over and under usage of a
Licensed Software.

The Allocation is done manually on the :ref:`Details View<Accessing the Details View of a License>` of a Software
License. In case the License is either Single User, Volume Users or
Unlimited Users, you have to add users instead of Hardware Assets.

**To perform Asset/Node Allocation:**

.. note:: While performing allocation in a Node Lock License, the Hardware Assets are referred to as Nodes.

1. Go to **Asset** (A Navigation Tab) >> **Software Licenses**.

2. Click on the **Edit Icon** adjacent to the License that needs
   Allocation, or just click on the License name.

3. The Details View of the License opens. Scroll down to the
   **Allocation** tab. Here you can view the list of all the existing
   Allocations.

.. _amf-132:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-132.png
    :align: center
    :alt: figure 132

4. Click on the **Allocate**/**Allocate Node** button in the **Allocation** tab. The
   Allocate Assets/Node dialog box opens.

.. _amf-133:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-133.png
    :align: center
    :alt: figure 133

.. _amf-133.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-133.1.png
    :align: center
    :alt: figure 133.1    

5. The Allocate Assets/Node dialog box shows you all Hardware Assets
   (Workstations, Laptops, Servers, etc.) in the CMDB. You can search Assets and allocate them.

   The search bar allows you to use various combinations of predefined
   search options and keywords. If you want to see the list of all
   available search options, then click on the search bar. You can
   select an option or multiple options from the drop-down list.

    .. _amf-134:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-134.png
        :align: center
        :alt: figure 134

   You can search Hardware Assets with keywords. When you provide a
   keyword, Motadata searches all the Hardware Assets with the keyword in
   Name, Description, and Tags.

   You can make a filter using a chain of predefined search options and
   keywords.

   Perform search and find the Assets that you want to allocate.

6. Select the Assets and click on **Allocate** situated in the top
   right corner. The selected Assets are allocated to the License.

**To Perform User Allocation:**

1. Just like allocating Assets, certain License Types require you to
   allocate users instead of Assets (Single User, Volume Users, and Unlimited Users). In the Details View of such a
   License type, click on the **User Allocation** tab.

    .. _amf-135:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-135.png
        :align: center
        :alt: figure 135

   The tab shows all current users added to the License if any.

2. To add a new user/users, click on the **Allocate License User**
   button. This opens the **Allocate License User** dialog box.

    .. _amf-136:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-136.png
        :align: center
        :alt: figure 136

3. In the dialog box, you can view the names of all the Requesters in
   the system. You can select multiple users (Requesters) by clicking
   on the checkbox against their names.

   The search bar allows you to search users based on the following
   options:

    a. Name

    b. Email

    c. Location

    d. Department

    e. VIP Requester status

   You can set multiple conditions using the options; you can access
   the options by clicking on the search bar.

   Select the users whom you want to allocate the License and click
   on the **Allocate** button. Now you have successfully allocated
   the License.

**Viewing Allocation Count**

When allocating Assets to a License, one can see how many Assets have been allocated from the Details View.

.. _amf-136.1:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/asset-management/AM-136.1.png
    :align: center
    :alt: figure 136.1