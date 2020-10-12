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
- IdC: Sensitive user data is sent in cleartext over the network.
- IdC: Invalid user input exploits the database. (Form validation)
- External, abnormal requests reaches internal services outside of DMZ.
- Sensitive patient information is leaked to the public as a result of a data breach.
- Password hashes are leaked to the public as a result of a databreach.


System and data integrity threats
---------------------------------
- System software is out of date and exploitable.
- Internal user modifies patient info, resulting in uncorrect information.


System and data availability threats
------------------------------------
- DoS: System monitoring fails and creates a gap in the logs.
- The system is inaccessible because of too much incoming requests.



Authentication threats for system eligible users
------------------------------------------------
- Opportunist steals a logged in users cookie to access unauthorized information.
- External user spoofs email address to harvest credentials through phising.



Authorization threats for system eligible users
-----------------------------------------------

- IdC: An unauthorized user has access to confidential patient information.
- EoP: Sysadmin rights are not terminated upon resignation.
- An internal user elevates his/hers privileges to perform unauthorized actions.



Non-repudiation threats for system eligible users
-------------------------------------------------






  .. To deler av systemet: Kan man spoofe/tampere etc. mellom klient og server?

Tabell: TR-ID, Trussel, Aktør, Element
