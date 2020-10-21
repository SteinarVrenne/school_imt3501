Data Flow Diagram
-----------------

Based on the STRIDE-model, we have identified the attack vectors for the different data flows between the processes and/or entities. The identified threats in the Data Flow Diagram is written in depth under "Major Threats". The trust boundaries are written more about in depth at "Trust Levels"

The bubbles represent a process in the system, the boxes are external entities that interact with the system. These are outside of the architect or developers control, and represents users and/or web clients, but in the Data Flow Diagram they have description of whom they represent. The arrows represent which way the data is flowing. In cases it has attached threat vectors according to STRIDE and which operations they perform. Data stores are represented with a lower line and an upper line, which in this case is EHR, Authentication and Database server. The trust levels in the system is indicated with dotted lines, which represent the trust boundaries identified in the system.

A User is a normal user of the system whom is only supposed to use the service. This can be a patient, social worker or a family member of the patient. These users are not supposed to add anything to the system other than request services and features.

IT Maintenance is a specific process which can have several subprocesses and is very specific to each case. This can include, but not limited to, updating outdated software, patching security vulnerabilities etc.. 

.. 
    - Revisit the general architecture you created and the functionalities you defined in theuse cases, then design the system in terms of DFD (Data Flow Diagram)
    - Define the high-level way of disassembling the system and focusing on itsfunctional components, and to analyze the flows of data through the systemcomponents.