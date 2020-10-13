Trust levels
------------

  .. - What are the trust levels of system users and threat agents?
    .. - Who are the eligible users (actors) in your system (revisit use cases)?

The users of the system are the same as those identified in the use-case diagram in task 1. These are the following:

  + Patient
  + Family member
  + Healthcare worker
  + Social worker
  + System administrator

  .. - What is the role(s) will the eligible users (actors) play in your system?

Patient and family will in their role only alter things regarding contacting. They have the ability to contact a healthcare worker or to be contacted by them. It is also neccesary for them to be able to alter the information we have registered on them. This role also includes the social workers visiting the patients.

Healthcare workers also have the ability to contact their patients. They additionally need the privilege to view the health information of multiple patients, and the ability to register new and alter old info regarding the patients.

  .. Assumption: System admins can only apply doctors from a central DB and cannot create their own doctor account to spy on everyone.

The most trusted and therefore most powerfull role in the system is the system administrator. They are responsible for creating and discarding doctor profiles, access to all system hardware in order maintain it. They have the ability to take down the entire system which if designed incorrectly even could happen accidentilly.

  .. - Who are the ineligible users (threat agents) that may jeopardize your system?

Several threat agents are mentioned in task 1. We will elaporate on these in this document. There are many actors who have something to gain from our facilities and the information we have acces to. They vary in goals, competense, resources, and persistence.

.. csv-table:: Threat agent overview
   :header: "Threat agent", "Goal", "Competanse", "Resources", "Persistence"
   :widths: 20, 20, 20, 20, 20

   "Script kiddy", "entertainment, status", "Low", "Low", "Low"
   "Nation-states", "intelligence, influence, infiltration", "High", "High", "High"
   "Organized crime", "Monatary", "Medium", "High", "Low"
   "Insider HCW", "", "Low", "Low", "Low, (in cases of revenge High)"



.. +--------------+------+------------------------+-------------+
.. | Threat agent | Goal | Competanse | Resources | Persistence |
.. +==============+======+============+===========+=============+
.. |
.. +------------------------------------------------------------
.. |
.. +------------------------------------------------------------
.. |
.. +------------------------------------------------------------
.. |
.. +---------------------------------------------------------------




  + Script kiddies
    - Goal
  + Nation state actors
  + Organized crime
  + Insider HCW
  + Insider Sys-admin

  ..  - How the eligible users’ role(s) can be compromised by the ineligible users(threat agents) and jeopardize your system and the eligible users (actors)’ data?
