Misuse case scenarios
=====================

It also important to understand how the misuse case scenario along with related
threat agents abuses a threat in order to violate system policies. Below we will
elaborate on how certain misuse cases specified in task 1 are related to identified
threats. We will also explain how related threat agents performs a certain attack
or exploits the threat.

- Which threats can happen to what use case (misuse case scenarios)?
    - Which threat would trigger what use case?

    Use case, followed by threats:
        - Log in as user
            - Password hashes are leaked to the public as a result of a databreach.
            - System software is out of date and exploitable.
            - The system is inaccessible because of too much incoming requests.
            - Opportunist steals a logged in users cookie to access unauthorized information.
            - External user spoofs email address to harvest credentials through phising.


        - Read patient vitals
            - An internal user elevates his/hers privileges to perform unauthorized actions.
            - Sensitive user data is sent in cleartext over the network.
            - Invalid user input exploits the database.

        - Register new patient / healthcare worker
            - Internal user modifies patient info, resulting in uncorrect information.




    - How would threat agents proceed/preform the attack?

        - Password hashes are leaked to the public as a result of a databreach.
            - The threat agent, most likely an individual dumps the database of the system to the public. This can be used by either an SQL injection, or gaining access to the database server.

        - System software is out of date and exploitable.
            - Any threat agent have the resources to search for active CVEs about the program online, and use software like Metasploit to easily peform an attack.

        - The system is inaccessible because of too much incoming requests.
            - This threat could either because of to much normal traffic, or a malicious DDOS attack.

        - Opportunist steals a logged in users cookie to access unauthorized information.
            - This kind of attack requires some amount of skill and knowledge, so the actor are most likely groups or state actors.
              In order to preform this kind of attack, the attacker needs to trick the user to upload their cookies, by sending them a script which sends the cookies to the attacker.
              They can use the users cookies in their own browser, to log in without username or password to the platform.

        - External user spoofs email address to harvest credentials through phishing.
            - Performing an attack like this are not very complicated at all, which means it can be done by any threat actor.
              This is done by sending an email to a system user, in which the attacker try to trick the user to type in their password on a fake website.
              Often they tell the user that they need to reset their password, and prompts them with a fake website, that steals the credentials.


        - An internal user elevates his/hers privileges to perform unauthorized actions.
            - An attack like this can only be performed by an already existing user in the system.
              Example of doing this: .....
              One other way of doing this is by stealing cookies, like mentioned above. This was a vulnerability found in Blackboard recently.

        - Sensitive user data is sent in cleartext over the network.
            - If the website is not strictly configured to transfer data using HTTPS, anyone using a middle man attack can listen in on the the traffic using software like Wireshark.
              Attackers can also listen in on wireless signals, and eavesdrop the TCP stream, if they are nearby, and the attacker are using a wireless network connection.

        - Invalid user input exploits the database.
            - Poorly constructed databases can be exploited by injection. The attacker can experiment with how the database sanitize, and read inputs.
            - The skill level required to preform this kind of attack varies based on how good the database is constructed.





    - What is the risk and the impact for your system according to the list of the identified threats (prioritize the threats)?


..  ----------------------------------------------------------------------------------------
    | Threat ID  |              Threat                          | DREAD Value |  Mitigated |
    +------------+----------------------------------------------+-------------+------------+
    |   T1       | Access to the database                       |   eks:  10  | eks: no    |
    |   T2       | System software out of date, and exploitable |             |            |
    |   T3       | System is inaccessible                       |             |            |
    |   T4       | Data sent in cleartext                       |             |            |
    |   T8       | Invalid database input                       |             |            |
    |   T10      | Spoofing of email address, phishing          |             |            |


..       DREAD = is a threat risk ranking method
         Damage potential (1-3): How big will be the damage if the attack succeed
         Reproducability 	    How easy it is for the attack/threat to be repoduced
         Exploitability		    How easy it is for the attack to be launched
         Affedted users		    How many are affected
         Discoverability	    How easy it is to discover the vulnerability
