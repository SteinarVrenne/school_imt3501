Misuse case scenarios
=====================

It also important to understand how the misuse case scenario along with related
threat agents abuses a threat in order to violate system policies. Below we will
elaborate on how certain misuse cases specified in task 1 are related to identified
threats. We will also explain how related threat agents performs a certain attack
or exploits the threat.

Which threats can happen to what use case?
------------------------------------------

Which threat would trigger what use case?
.........................................

Login as user
"""""""""""""

.. csv-table::
  :header: **Threat ID**, **Threat**
  :widths: 15, 40   

        "T05", "Password hashes are leaked to the public as a result of a data breach."
        "T06", "System software is out of date and exploitable."
        "T15", "The webserver is inaccessible because of too many incoming requests."
        "T17", "The database server is inaccessible because of too many incoming requests."
        "T19", "A logged in user has his/her session cookie compromized."
        "T22", "A system administrator spoofs his or hers identity in order to harvest user data or patient vitals."
        "T10", "Inconsistency in configuration data leads to the system not functioning as intended."
        "T12", "An older more vulnerable page or version of the web application is not properly removed from the internet after an application upgrade and gets exploited."
        "T15", "The webserver is inaccessible because of too many incoming requests."
        "T16", "Third party software experiences downtime that causes lack of functionality in the system."
        "T18", "Users are not able to use the web application in emergency situations because of system downtime."
        "T20", "A healthcare worker has his or hers authenticative data stolen through phishing emails."
        "T21", "A social worker or family member is not able to authenticate during an emergency situation because of system bugs."
        "T24", "Sysadmin rights are not terminated upon resignation."

Read patient vitals
"""""""""""""""""""

.. csv-table::
  :header: **Threat ID**, **Threat**
  :widths: 15, 40 

       "T25", "A patient, family member or social worker elevates his/hers privileges to perform unauthorized actions."
       "T01", "Sensitive user data is sent in cleartext over the network."
       "T02", "Malicious user input exploits the database by the means of SQLinjection."
       "T04", "Sensitive patient information is leaked to the public as a result of a data breach."
       "T10", "Inconsistency in configuration data leads to the system not functioning as intended."
       "T11", "Incorrect modification in EHR might affect further actions in the organization."
       "T12", "An older more vulnerable page or version of the web application is not properly removed from the internet after an application upgrade and gets exploited."
       "T07", "Patient vitals is modified/updated incorrectly, resulting in the patient data having an incorrect state."
       "T13", "The web application has client-side vulnerabilities that gets exploited and thus changes the site's visual apperance or behavior."
       "T15", "The webserver is inaccessible because of too many incoming requests."
       "T16", "Third party software experiences downtime that causes lack of functionality in the system."
       "T18", "Users are not able to use the web application in emergency situations because of system downtime."
       "T20", "A healthcare worker has his or hers authenticative data stolen through phishing emails."
       "T21", "A social worker or family member is not able to authenticate during an emergency situation because of system bugs."
       "T23", "A system user has unauthorized access to confidential patient information."
       "T26", "A social worker's access to patient information is not terminated once the relationship has ended."
       "T28", "Healthcare worker denies accessing unauthorized information about other patients."
            
Register new patient / healthcare worker
""""""""""""""""""""""""""""""""""""""""

.. csv-table::
  :header: **Threat ID**, **Threat**
  :widths: 15, 40 

       "T10", "Inconsistency in configuration data leads to the system not functioning as intended."
       "T15", "The webserver is inaccessible because of too many incoming requests."
       "T16", "Third party software experiences downtime that causes lack of functionality in the system."
       "T18", "Users are not able to use the web application in emergency situations because of system downtime."
       "T24", "Sysadmin rights are not terminated upon resignation."

The rest of our threats are still dangerous to the system, however they do not fit into one of the three use cases.


How would threat agents proceed/preform the attack?
...................................................
    

-  **T01**, Sensitive user data is sent in cleartext over the network.
    - If the website is not strictly configured to transfer data using HTTPS, anyone using a middle man attack can listen in on the the traffic using software like Wireshark.
      Attackers can also listen in on wireless signals, and eavesdrop the TCP stream, if they are nearby, and the attacker are using a wireless network connection.
      Any of the threat actors are capable and a threat of attacking using this method.

-  **T02**, Malicious user input exploits the database by the means of SQLinjection.
    - Poorly constructed databases can be exploited by injection. The attacker can experiment with how the database sanitize, and read inputs.
      The skill level required to preform this kind of attack varies based on how good the database is constructed.
      This is for example the way to capture all of the users registered on a website. Any threat actors will be interested in that list.

-  **T03**, External, abnormal requests reaches internal services outside of DMZ.
    - A respons like this dont usually happen, and is almost impossible without inside knowledge of how the internal network is connected.
      The routers firewall have to be wrongly configured, or contain a weakness in order for this request to be accepted.
      We estimate that only nation state actors have the skill, and time to preform a reconnaissance attack like this.

-  **T04**, Sensitive patient information is leaked to the public as a result of a data breach.
    - In order to breach the database of a system, you either have to have some kind of system user access, or exploit some input into tricking the database to output all of its records.
      The kind of attacker who seek public attention is the type of attackers who wants to spread a bad reputation among the system. Most likely hacktivists.
      This can either be information about one user, or all of the systems users.

-  **T05**, Password hashes are leaked to the public as a result of a data breach.
    - The threat agent, most likely an individual, or small group dumps the database of the system to the public. 
      In order to preform this kind of attack, you can use the same methods as described in threat 04.
      This can be used by either an SQL injection, or gaining access to the database server.
      The attacker are likely to preform this attack, to sell the users passwords for financial gain.

-  **T06**, System software is out of date and exploitable.
    - Any threat agent have the resources to search for active CVEs about the program online, and use software like Metasploit to easily perform an attack.
      This is some of the first things an attacker look for when scouting out a system.

-  **T09**, System security logfiles are not recording all of the information needed in order to document system security events.
    - This is a event that a hacker might to in order to hide their tracks.
      They have been inside the system, gained the information they seeked, and now wants nobody to know that they were in.
      To to this, they can simply delete the logfiles, and command history.
        
-  **T12**, An older more vulnerable page or version of the web application is not properly removed from the internet after an application upgrade and gets exploited.
    - Attackers who finds this vunerable page can simply use a exploit framework like metasploit, to gain higher level access to the system.

-  **T13**, The web application has client-side vulnerabilities that gets exploited and thus changes the site's visual apperance or behavior.
    - !!!!!!!!!!!!!.

-  **T15**, The webserver is inaccessible because of too many incoming requests.
    - This threat could either because of to much normal traffic, or a malicious DDOS attack.
      The threat agent 

-  **T17**, The database server is inaccessible because of too many incoming requests.
    - This threat could either because of to much normal traffic, or a malicious DDOS attack.
      The threat agent

-  **T18**, Users are not able to use the web application in emergency situations because of system downtime.
    - Attackers can perform a distrubuted denial of service attack on the system, in order to take it offline. 
      They dont gain any information, people who have a motivation to take the system offline like hacktivists might do it.  

-  **T19**, A logged in user has his/her session cookie compromized.
    - This kind of attack requires some amount of skill and knowledge, so the actor are most likely groups or state actors.
      In order to preform this kind of attack, the attacker needs to trick the user to upload their cookies, by sending them a script which sends the cookies to the attacker.
      They can use the users cookies in their own browser, to log in without username or password to the platform.

-  **T20**, A healthcare worker has his or hers authenticative data stolen through phishing emails.
    - An attackers can, with the correct email address to the healthcare worker, send them a mail that looks like it comes from a credible source, that makes the healthcare worker press a link, or file attatchment.
      The attacker can either make the user install a file with malware, which grants them access to the workers system, or they can make the user click a weblink.
      This weblink could be a fake login page just like the one they use to access the system, or the weblink can contain cross site scripting code that makes the worker post information back to the attacker, like authentication details.

-  **T24**, Sysadmin rights are not terminated upon resignation.
    - A fired ore resigned system administrator can utilize that its user access is not terminated.
      This is not an official threat actor, however the system administrator might make a deal with a malicious person our group, to use their access to gain information.

-  **T25**, A patient, family member or social worker elevates his/hers privileges to perform unauthorized actions.
    - An attack like this can only be performed by an already existing user in the system.
      One way of doing this is by stealing cookies, like mentioned above. This was a vulnerability found in Blackboard recently.

-  **T26**, A social worker's access to patient information is not terminated once the relationship has ended.
    - This threat is similar to threat 24. In short term they can be contacted by a malicious person or group, in order to keep them updated on the patients health.
                     
The threats that are not mentioned in the text above, are not a threat connected to one of the threat agents, rather a threat that some of the systems own users, or systemadministrator can perform without intention.
    
    
What is the risk and the impact for your system according to the list of the identified threats?
................................................................................................

.. How the table should look
..  ----------------------------------------------------------------------------------------
    | Threat ID  |              Threat                          | DREAD Value |  Mitigated |
    +------------+----------------------------------------------+-------------+------------+
    |   T1       | Access to the database                       |   eks:  10  | eks: no    |
    |   T2       | System software out of date, and exploitable |             |            |

.. csv-table::
  :header: **Threat ID**, **Threat**, **DREAD Value**, **Mitigated**
  :widths: 5, 40, 10, 10

  "T01", "Sensitive user data is sent in cleartext over the network.", "2.6", "no" 
  "T02", "Malicious user input exploits the database by the means of SQLinjection.", "2.4", "no"
  "T03", "External, abnormal requests reaches internal services outside of DMZ.", "1.6", "no"
  "T04", "Sensitive patient information is leaked to the public as a result of a data breach.", "2.4", "no"
  "T05", "Password hashes are leaked to the public as a result of a data breach.", "2.6", "no"
  "T06", "System software is out of date and exploitable.", "2.8", "no"
  "T07", "Patient vitals is modified/updated incorrectly, resulting in the patient data having an incorrect state.", "x", "no"
  "T08", "System security logfiles are not recording information correctly according to system behavior.", "x", "no"
  "T09", "System security logfiles are not recording all of the information needed in order to document system security events.", "x", "no"
  "T10", "Inconsistency in configuration data leads to the system not functioning as intended.", "x", "no"
  "T11", "Incorrect modification in EHR might affect further actions in the organization.", "x", "no"
  "T12", "An older more vulnerable page or version of the web application is not properly removed from the internet after an application upgrade and gets exploited.", "2.6", "no"
  "T13", "The web application has client-side vulnerabilities that gets exploited and thus changes the site's visual apperance or behavior.", "1.6", "no"
  "T14", "System monitoring/logging fails and creates a gap in the event logs.", "x", "no"
  "T15", "The webserver is inaccessible because of too many incoming requests.", "2.8", "no"
  "T16", "Third party software experiences downtime that causes lack of functionality in the system.", "x", "no"
  "T17", "The database server is inaccessible because of too many incoming requests.", "2.8", "no"
  "T18", "Users are not able to use the web application in emergency situations because of system downtime.", "3", "no"
  "T19", "A logged in user has his/her session cookie compromized.", "1.8", "no"
  "T20", "A healthcare worker has his or hers authenticative data stolen through phishing emails.", "2", "no"
  "T21", "A social worker or family member is not able to authenticate during an emergency situation because of system bugs.", "x", "no"
  "T22", "A system administrator spoofs his or hers identity in order to harvest user data or patient vitals.", "2.4", "no"
  "T23", "A system user has unauthorized access to confidential patient information.", "1.4", "no"
  "T24", "Sysadmin rights are not terminated upon resignation.", "2.2", "no"
  "T25", "A patient, family member or social worker elevates his/hers privileges to perform unauthorized actions.", "1.4", "no"
  "T26", "A social worker's access to patient information is not terminated once the relationship has ended.", "x", "no"
  "T27", "Social worker forgets to commit vital patient information and denies not doing so.", "x", "no"
  "T28", "Healthcare worker denies accessing unauthorized information about other patients.", "2.4", "no"
  "T29", "A system administrator denies abuse of system privileges.", "2.6", "no"
  "T30", "A patient does not inform social workers, family members or healthcare workers about vital updates regarding their health status.", "x", "no"
  "T31", "Social worker or healthcare worker denies committing/updating incorrect data about a patient.", "x", "no"
  "T32", "The system denies patients (or their family members/social workers) to submit updates regarding their health situation.", "x", "no"

..       DREAD = is a threat risk ranking method
         Damage potential (1-3): How big will be the damage if the attack succeed
         Reproducability  (1-3): How easy it is for the attack/threat to be repoduced
         Exploitability   (1-3): How easy it is for the attack to be launched
         Affedted users	  (1-3): How many are affected
         Discoverability  (1-3): How easy it is to discover the vulnerability

..       D + R + E + A + D / 5 = Score