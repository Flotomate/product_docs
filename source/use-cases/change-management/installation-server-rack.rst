****************************************************
Installation of New Server Racks (Change Management)
****************************************************

**Scenario**: Acme Inc is planning to increase its server capacity in its Ahmedabad facility. The facility is about to get New
server Racks. The new Racks are part of a major change in the IT infrastructure of Acme Inc. A Technician has been assigned as the 
Change Manager to implement the installation of the server racks. 

**Primary Actors**: Change Manager, Change Implementor, Change Reviewer, and Facility Manager. 

**Action**: On arrival of the new server Racks. The following actions take place:

- The Change Manager (John Diaz) creates a Change Request and becomes the assigned Technician and the Change Manager.

    .. _us-cm-1:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-01.png
          :align: center
          :alt: figure 1

  Learn more about :doc:`Creating a Change <submitting-a-rfc>`. 

- The Change Manager then accepts the Change. Learn more about :ref:`Change Workflow`.  

- The Change Manager modifies the following details:

  a. Sets the Change reason.

  b. Sets the target environment.

  c. Sets the Change and Rollout time.

  d. Documents the Planning process (Impact, Rollout and Backout plan).

  e. Links the three associated servers with the Change.

.. _us-cm-2:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-02.png
    :align: center
    :alt: figure 2

.. _us-cm-3:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-03.png
    :align: center
    :alt: figure 3

- The Change moves to the Planning stage. The Change Manager now has to seek approval from the Facility Manager (Hector Troy) before 
  implementing the Change. Learn more about :ref:`cm-asking-for-approval`.

    .. _us-cm-4:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-04.png
        :align: center
        :alt: figure 4

  The Facility Manager rejects the approval on the ground that the date of rollout is not conducive.

    .. _us-cm-5:
    .. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-05.png
        :align: center
        :alt: figure 5

  The Change Manager moves the Change to the Planning stage and sets a new rollout date. The Change is again sent for
  Approval. This time the Facility Manager accepts the Change.

- Now the Change is in the Implementation Stage. Here the Change Manager appoints a Change Implementer (Amartya Gupta). 

.. _us-cm-6:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-06.png
    :align: center
    :alt: figure 6

- The Change Manager and Implementer communicate using the Collaboration feature. Learn more about :ref:`cm-collaborate-schedule-and-planning`.

- The Implementer initiates the Implementation process of the server Racks on the set date & time. 

- The Change moves to the In-Review stage, where the Change Manager appoints a Change Reviewer (Raj Mohan). 

.. _us-cm-7:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-07.png
    :align: center
    :alt: figure 7

- The Change Reviewer completes the In-Review stage; this marks the Closure of the Change. 
