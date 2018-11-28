********************************************
Creating a HR Technician Using Authorization
********************************************

**Scenario**: Acme Inc receives HR related queries through their helpdesk. They want to control who sees such tickets. 

**Action**: An admin decides to use the Group Access feature of Flotomate ITSM and create a Technician Group for each function.
Group Access would allow technicians to view tickets assigned to their group. The admin creates a group called Human Resource and
adds a Human Resource to that group as a technician.

*Adding HR as Technician from Admin >> Technicians >> Add Technician*:

.. _us-cm-8:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-8.png
    :align: center
    :alt: figure 8

*Adding Steve to Human Resource group from Admin >> Technician Groups:*

.. _us-cm-9:
.. figure:: https://s3-ap-southeast-1.amazonaws.com/flotomate-resources/use-case/US-CM-9.png
    :align: center
    :alt: figure 9

**Outcome**: Requester Steve will only have access to Request tickets from location Mumbai and having Technician Group: Human Resource.
The group filter will be applicable for Request tickets only. 