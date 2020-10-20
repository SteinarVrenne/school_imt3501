Major threats
=============

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
.. csv-table::
  :header: **Threat ID**, **Threat**, **User/Asset**, **Element**
  :widths: 5, 40, 10, 10

  "T01", "Sensitive user data is sent in cleartext over the network.", "User data", "Data flow"
  "T02", "Malicious user input exploits the database by the means of SQLinjection.", "Database server", "Data storage"
  "T03", "External, abnormal requests reaches internal services outside of DMZ.", "Internal Servers", "Data flow"
  "T04", "Sensitive patient information is leaked to the public as a result of a data breach.", "Patient vitals", "Data storage"
  "T05", "Password hashes are leaked to the public as a result of a data breach.", "Authenticative data", "Data storage"


System and data integrity threats
---------------------------------
.. csv-table::
  :header: **Threat ID**, **Threat**, **User/Asset**, **Element**
  :widths: 5, 40, 10, 10

  "T06", "System software is out of date and exploitable.", "System software", "Process"
  "T07", "Patient vitals is modified/updated incorrectly, resulting in the patient data having an incorrect state.", "Patient vitals", "Data storage"
  "T08", "System security logfiles are not recording information correctly according to system behavior.", "Logs", "Process"
  "T09", "System security logfiles are not recording all of the information needed in order to document system security events.", "Logs", "Data storage"
  "T10", "Inconsistency in configuration data leads to the system not functioning as intended.", "Configuration data", "Process"
  "T11", "Incorrect modification in EHR might affect further actions in the organization.", "EHR", "External entity"
  "T12", "An older more vulnerable page or version of the web application is not properly removed from the internet after an application upgrade and gets exploited.", "Webserver & System software", "Process"
  "T13", "The web application has client-side vulnerabilities that gets exploited and thus changes the site's visual apperance or behavior.", "Process"


System and data availability threats
------------------------------------
.. csv-table::
  :header: **Threat ID**, **Threat**, **User/Asset**, **Element**
  :widths: 5, 40, 10, 10

  "T14", "System monitoring/logging fails and creates a gap in the event logs.", "Logs", "Data flow"
  "T15", "The webserver is inaccessible because of too many incoming requests.", "Webserver", "Process"
  "T16", "Third party software experiences downtime that causes lack of functionality in the system.", "System software", "Process & External entity"
  "T17", "The database server is inaccessible because of too many incoming requests.", "Database serber", "Process & Data storage"
  "T18", "Users are not able to use the web application in emergency situations because of system downtime.", "Webserver", "Process"


Authentication threats for system eligible users
------------------------------------------------
.. csv-table::
  :header: **Threat ID**, **Threat**, **Asset**, **Element**
  :widths: 5, 40, 10, 10

  "T19", "A logged in user has his/her session cookie compromized.", "Cookies, Authenticative data", "Data flow"
  "T20", "A healthcare worker has his or hers authenticative data stolen through phishing emails.", "Authenticative data", "Data storage"
  "T21", "A social worker or family member is not able to authenticate during an emergency situation because of system bugs.", "System software, authentication & authorization servers", "Data flow"
  "T22", "A system administrator spoofs his or hers identity in order to harvest user data or patient vitals.", "User data & patient vitals", "Data storage"


Authorization threats for system eligible users
-----------------------------------------------
.. csv-table::
  :header: **Threat ID**, **Threat**, **Asset**, **Element**
  :widths: 5, 40, 10, 10

  "T23", "A system user has unauthorized access to confidential patient information.", "User data & patient vitals", "Data storage"
  "T24", "Sysadmin rights are not terminated upon resignation.", "Authentication & authorization servers", "Data flow"
  "T25", "A patient, family member or social worker elevates his/hers privileges to perform unauthorized actions.", "Authentication & authorization servers", "Data flow"
  "T26", "A social worker's access to patient information is not terminated once the relationship has ended.", "Authentication & authorization servers, patient vitals", "Data storage"


Repudiation threats for system eligible users
---------------------------------------------
.. csv-table::
  :header: **Threat ID**, **Threat**, **Asset**, **Element**
  :widths: 5, 40, 10, 10

  "T27", "Social worker forgets to commit vital patient information and denies not doing so.", "Patient vitals", "Data storage"
  "T28", "Healthcare worker denies accessing unauthorized information about other patients.", "Patient vitals, user data", "Data storage"
  "T29", "A system administrator denies abuse of system privileges.", "Authentication & authorization servers", "Data flow"
  "T30", "A patient does not inform social workers, family members or healthcare workers about vital updates regarding their health status.", "Patient vitals", "External entity"
  "T31", "Social worker or healthcare worker denies committing/updating incorrect data about a patient.", "Patient vitals", "Data flow"
  "T32", "The system denies patients (or their family members/social workers) to submit updates regarding their health situation.", "Data flow", "Patient vitals"
