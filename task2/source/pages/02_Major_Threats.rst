Major threats
=============

- What are the major threats? Focus on threat identification and classification based on:
    - Threat to system/ data confidentially

    - Threat to system/ data integrity

    - Threat to system/ data availability

    - Threat to the system eligible users (actors) authentication

    - Threat to the system eligible users (actors) authorization

    - Threat to the system eligible users (actors) non-repudiation

    - Threat to the system eligible users (actors) privacy


In this section, we will identify potential threats and sources for the
Out-patient healthcare monitoring system. These threats will be identified by
using the STRIDE model as SRIDE per threat. STRIDE is just used as a guide in
order to specify the  The STRIDE methodology is defined as followed:

.. csv-table::
  :header: **STRIDE letter**, **Definition**, **Violates**
  :widths: 15, 40, 10

	"**S - Spoofing**", "Pretending to be someone or something else.", "Authentication"
  "**T - Tampering**", "Modification of elements you are not allowed to modify.", "Integrity"
  "**R - Repudiation**", "Denying that you did something or claiming that you are not responsible for the event.", "Non-reputation"
  "**I - Information Disclosure**", "Exposing information to someone who is not authorized.", "Confidentiality"
  "**D - Denial of Service**", "Preventing a system from providing a service or preventing users to access it.", "Availability"
  "**E - Elevation of privileges**", "Refers to situations where you are able to perform actions you are not supposed to.", "Authorization"


System and data confidentiality threats
---------------------------------------
- Sensitive user data is sent in cleartext over the network.
- Invalid user input exploits the database. (Form validation)
- External, abnormal requests reaches internal services outside of DMZ.
- Sensitive patient information is leaked to the public as a result of a data breach.
- Password hashes are leaked to the public as a result of a databreach.


System and data integrity threats
---------------------------------
- System software is out of date and exploitable.
- Healthcare worker modifies patient info incorrectly, resulting in vital incorrect patient data.
- System security logfiles are not recording information correctly according to system behavior.
- System security logfiles are not recording all of the information needed in order to document system security events.
- Inconsistency in configuration data leads to the system not functioning as intended.
- Incorrect modification in EHR might affect actions in the organization.




System and data availability threats
------------------------------------
- System monitoring fails and creates a gap in the logs.
- The system is inaccessible because of too many incoming requests.
- 



Authentication threats for system eligible users
------------------------------------------------
- Opportunist steals a logged in users cookie to access unauthorized information.
- External user spoofs email address to harvest authentication credentials through phising.



Authorization threats for system eligible users
-----------------------------------------------

- An unauthorized user has access to confidential patient information.
- Sysadmin rights are not terminated upon resignation.
- An internal user elevates his/hers privileges to perform unauthorized actions.



Non-repudiation threats for system eligible users
-------------------------------------------------
- Social worker forgets to commit vital patient information and denies not doing so.
- Healthcare worker denies accessing unauthorized information about other patients.
- A system administrator denies abuse of system privileges.
- Patients does not inform social workers, family members or healthcare workers about vital updates regarding their health status.
- Social worker or healthcare worker denies commiting/updating incorrect data about a patient.


+ Patient
+ Family member
+ Healthcare worker
+ social worker
+ System administrator



  .. To deler av systemet: Kan man spoofe/tampere etc. mellom klient og server?

Tabell: TR-ID, Trussel, Aktør, Element
