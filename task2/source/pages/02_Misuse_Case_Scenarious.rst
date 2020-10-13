Misuse case scenarios
---------------------

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



        - Sensitive user data is sent in cleartext over the network.



        - Invalid user input exploits the database.



        - Internal user modifies patient info, resulting in uncorrect information.






    - What is the risk and the impact for your system according to the list of the identified threats (prioritize the threats)?







