Document the threat modeling process
------------------------------------

.. - What has been done

..  We have identified
  - External interfaces
  - processes
  - dataflows
  - data stores

The threat modeling process that went into creating this document is inspired by lectures and methodologies mentioned in them. In this document is a re-identification and classification of system assets. we have additionally described the different roles in the system and which privileges can cause the most damage by being exploited. This is used to find the trust boundries between system process / data stores etc. and helps identify the external interfaces. This is illustrated in the data flow diagram on page 5.

..  We have modeled the system in an
  asset centric
    - CIA ranking
  Attacker centric
    - Goals
    - skills
    - risk tolerance
    - work factor / resources
    - activity level
  Software centric
    - Dataflow
    - data stores
    - trust boundries
    - processes

The system has in addition to it's asset & software centric threat modeling mention earlier, modeled the type of attacker we expect to face the system. This includes their capabilities along with other factors.

We used the STRIDE framework in order to identify as many threats to the system as possible. These where then linked to specific use-cases. Through the use of the DREAD framework we found the most dangerous ones to facilitate prioretization. We have found mitigation techniques for these threats by either remediating, transfering, or sometimes accepting the risk they present.


..  Threats
    - STRIDE to indetify threats to the system.
    - Linked threats to specific Use-cases
    - Described the acions necessary to perform the attack

..  Mitigate:
   - Remediate
   - Transfer
   - Accept



.. - Recommendation to  the  design team or/and to the policy makers at your organization (based on your findings of the threat modeling, what you think the policy makers/ designers, management board etc. should highly consider beforethey implement and deploy the system.). Focus on non-technical recommendation

There are many recommendations we wish to give after performing this threat assesment. The documents holds a lot of technical implementation details that we recommend the development team reads. To the design team we recommend to implement some form of multi-factor authentication and a system to keep configurations synchronized possibly through approaches from the concept of infrastructure as code. We also recommend some collaberation with policy makers to create a system to ensure all security patches are installed to protect the system. Security audits are advised specifically towards the client-side software.

We would of course recommend the teams working on this system to follow all of our proposals, but these are some of the more high-level mitigation techniques in our findings. This system faces risks with big impact and we therefore strongly encourage the securing of the system to be implemented in as many parts of the organization as possible from human resources to IT. 
