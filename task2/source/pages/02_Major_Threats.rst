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
  "**R - Repudiation**", "Denying that you did something or claiming that you are not responsible for the event.", "Reputation"
  "**I - Information Disclosure**", "Exposing information to someone who is not authorized.", "Confidentiality"
  "**D - Denial of Service**", "Preventing a system from providing a service or preventing users to access it.", "Availability"
  "**E - Elevation of privileges**", "Refers to situations where you are able to perform actions you are not supposed to.", "Authorization"


System and data confidentiality threats
---------------------------------------
- Sensitive user data is sent in cleartext over the network.
- Malicious user input exploits the database by the means of SQLinjection.
- External, abnormal requests reaches internal services outside of DMZ.
- Sensitive patient information is leaked to the public as a result of a data breach.
- Password hashes are leaked to the public as a result of a data breach.



System and data integrity threats
---------------------------------
- System software is out of date and exploitable.
- Patient data is modified/updated incorrectly, resulting in the patient data having an incorrect state.
- System security logfiles are not recording information correctly according to system behavior.
- System security logfiles are not recording all of the information needed in order to document system security events.
- Inconsistency in configuration data leads to the system not functioning as intended.
- Incorrect modification in EHR might affect further actions in the organization.
- An older more vulnerable version of the web application is not properly removed from the internet after an application upgrade and gets exploited.
- The web application has client-side vulnerabilities that gets exploited and thus changes the site's visual apperance or behavior.


System and data availability threats
------------------------------------
- System monitoring/logging fails and creates a gap in the event logs.
- The webserver is inaccessible because of too many incoming requests.
- Third party software experiences downtime that causes lack of functionality in the system.
- The database server is inaccessible because of too many incoming requests.
- Users are not able to use the web application in emergency situations because of system downtime.


Authentication threats for system eligible users
------------------------------------------------
- A logged in user has his/her session cookie compromized.
- A healthcare worker has his or hers authenticative data stolen through phishing emails.
- A social worker or family member is not able to authenticate during an emergency situation because of system bugs.
- A system administrator spoofs his or hers identify in order to harvest user data or patient vitals.


Authorization threats for system eligible users
-----------------------------------------------

- A system user has unauthorized access to confidential patient information.
- Sysadmin rights are not terminated upon resignation.
- A patient, family member or social worker elevates his/hers privileges to perform unauthorized actions.
- A social worker's access to patient information is not terminated once the relationship has ended.


Repudiation threats for system eligible users
---------------------------------------------
- Social worker forgets to commit vital patient information and denies not doing so.
- Healthcare worker denies accessing unauthorized information about other patients.
- A system administrator denies abuse of system privileges.
- A patient does not inform social workers, family members or healthcare workers about vital updates regarding their health status.
- Social worker or healthcare worker denies committing/updating incorrect data about a patient.
- The system denies patients (or their family members/social workers) to submit updates regarding their health situation.


+ Patient
+ Family member
+ Healthcare worker
+ social worker
+ System administrator



  .. To deler av systemet: Kan man spoofe/tampere etc. mellom klient og server?

Tabell: TR-ID, Trussel, Aktør, Element
