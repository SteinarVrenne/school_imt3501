Identify and specify the main abuse cases of the system
-------------------------------------------------------

.. TEMPLATE:
    .. csv-table::
    	:header: **AC - **, **Description**
    	:widths: 3, 10

    	"Actor", ""
    	"Purpose", ""
    	"Description", ""
    	"Countermeasures", ""

Confidentiality abuse cases
"""""""""""""""""""""""""""

.. csv-table::
	:header: **AC - Bruteforce login**, **Description**
	:widths: 3, 10

	"Actor", "Any external person"
	"Purpose", "Access person's account"
	"Description", "External threat actors who want to access the account of a patient, healthcare worker, social worker etc. to see or modify the details stored in the system."
	"Countermeasures", "A login limit will be enforced where after 5 incorrect login attempts, further attempts will be blocked."


.. csv-table::
	:header: **AC - Unauthorized access**, **Description**
	:widths: 3, 10

	"Actor", "Healthcare personnel, social worker"
	"Purpose", "Gain unauthorized access to personal data"
	"Description", "Personnel gaining access personal data that they should not have access to, based on their employment status, patients in their care, and other factors."
	"Countermeasures", "Employee in question may be penalized and may be terminated, legal action may be pursued according to the level of severity. Login sessions automatically expire in the case where the employee has forgotten to sign off and have left their device unattended."

.. csv-table::
	:header: **AC - Exploitation**, **Description**
	:widths: 3, 10

	"Actor", "Any"
	"Purpose", "Looking for and exploiting vulnerabilities"
	"Description", "Any actor, internal or external, finding and exploiting a security vulnerability, by automated or manual means, in order to gain access to or disrupt the service."
	"Countermeasures", "Frequent patching."

.. csv-table::
	:header: **AC - Unauthorized sharing**, **Description**
	:widths: 3, 10

	"Actor", "Healthcare personnel, social worker"
	"Purpose", "Sharing confidential data"
	"Description", "The actor obtains data (personal data, server configuration, software details, healthcare data) by permission, and then shares it to other parties that do not have access, without proper authorization for such sharing."
	"Countermeasures", "Employee in question may be penalized and may be terminated, legal action may be pursued according to the level of severity."

..
    Confidentiality!
    - Uatorisert personell leser personlig data
        - Løsning: Sessionavbrytelse
        - Miste jobb => miste tilgang med en gang
    - Utnytte exploits => løsning: patche regelmessige
    - Uatorisert deling av informasjon
        - Gjelder: servere (konfigurasjonsfiler, hvilken software/hardware og versjon), helsedata, personlig informasjon

Integrity abuse cases
"""""""""""""""""""""

.. csv-table::
    :header: **AC - Wrong data**, **Description**
    :widths: 3, 10

    "Actor", "System users"
    "Purpose", "Adding inaccurate data to the system"
    "Description", "The user, by mistake, saves data to the system that is incorrect/wrongful."
    "Countermeasures", "Sanity checking on user inputs, input validation, cross-checking."

.. csv-table::
	:header: **AC - Config errors**, **Description**
	:widths: 3, 10

	"Actor", "System administrators"
	"Purpose", "Wrongly configuring the system or its components"
	"Description", "The administrator, by mistake, enters a wrong configuration for the system, or for an individual component of it, causing system malfunction."
	"Countermeasures", "Implementing a change management protocol, implementing a testing/staging environment on which changes are performed and checked for stability before deployment to production."

..
    Integritet!
    - Legge in feil data - altså brukerfeiler
    - Konfigurasjonsfeil

Availability abuse cases
""""""""""""""""""""""""

.. csv-table::
    :header: **AC - Denial of Service**, **Description**
    :widths: 3, 10

    "Actor", "External person/organization (e.g. script kiddies, foreign governments)"
    "Purpose", "External actor wants to make the system unavailable for use"
    "Description", "A (distributed) denial of service attack is carried out using e.g. a botnet, in an attempt to overload the servers in the system, making them unable to handle incoming legitimate requests. This would render the service unusable for the duration of the attack."
    "Countermeasures", "Denial of service protection services, proper firewalling, ensuring adequate network bandwidth."

.. csv-table::
	:header: **AC - Power outage**, **Description**
	:widths: 3, 10

	"Actor", "Incidental"
	"Purpose", "Major unforeseen incident renders system infrastructure without power"
	"Description", "A power outage is caused by a natural disaster or other major event."
	"Countermeasures", "The system is connected to a UPS (uninterruptible power supply), backup generators, and uses redundant power supplies."

.. csv-table::
	:header: **AC - Network outage**, **Description**
	:widths: 3, 10

	"Actor", "Network engineers"
	"Purpose", "Network access is lost"
	"Description", "Maintenance work, construction work, etc. causing an accidental fiber cut, or upstream infrastructure stops working due to network equipment failure."
	"Countermeasures", "Redundant network connections for the entire system."

..
    Availability!
    - DoS/DDoS
    - Strømabrudd / internettbrudd
        - Løsning: flere netttilkoplinger

Attacks
"""""""

Angrep!
- Bufferoverflow
- SQLi
- XSS
- Phishing, spearphishing
- Ransomware
- Man in the middle
- Privilege escalation
- DoS / DDoS

Angripere!
- Insidere
    - Gjelder alle som kan logge inn
- Statlig aktør
- Hacker
