Trust levels
------------

- What are the trust levels of system users and threat agents?
    - Who are the eligible users (actors) in your system (revisit use cases)?

      + Patient
      + Family member
      + Healthcare worker
      + social worker
      + System administrator

    - What is the role(s) will the eligible users (actors) play in your system?

      Patient and family will have the role of contacts. They have the ability to contact a healthcare worker or to be contacted by them. It is also neccesary for them to be able to alter the information we have registered on them.

      Healthcare workers also have the ability to contact the patients. They additionally need the privilege to view the health information of multiple patients, and the ability to register new info and alter other.

      .. Assumption: System admins can only apply doctors from a central DB and cannot create their own doctor account to spy on everyone.

      The most trusted and therefore most powerfull role in the system is the system administrator. They are responsible for creating and discarding doctor profiles, access to all system hardware in order maintain it. They have the ability to take down the entire system which if designed incorrectly even could happen accidentilly.

    - Who are the ineligible users (threat agents) that may jeopardize your system?

      + Script kiddies
      + Nation state actors
      + Organized crime
      + Insider HCW
      + Insider Sys-admin

    - How the eligible users’ role(s) can be compromised by the ineligible users(threat agents) and jeopardize your system and the eligible users (actors)’ data?
