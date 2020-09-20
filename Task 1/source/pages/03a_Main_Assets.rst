Main Assets
The main assets we have identified are crucial for the organization/hospital and is relevant to the task. First, we have the different hardware servers and the data they generate. These assets are the webserver, database server, authentication server and system, and internal servers. 
-----------


The webserver is responsible for most of the traffic between clients on the application. As the webserver is first point of contact for a user, it is important to keep it secure. The database server contains on-site science data and data necessary for the hospitals administration. The authentication server and system is responsible for validating users who want to use the application and authorization server to authorize resource access, a tampered authentication or authorization server compromises all of the hospitals security. Lastly we have the internal servers, which handle internal traffic (e.g. contacting a printer), research processing and internet on the premise.

All the servers generate data that needs to be protected, such as the data within the databases, keys and passwords in the authentication server, logging and user data from the webserver, and configuration files and software that needs to be kept safe on the internal servers. The software the hospital needs varies from needs, but will always take place on the internal servers. 

The Electronic Health Registry (EHR) is also vital to the organization. A disruption in this tool will prevent the healthcare personnel from doing their work and help their patients. Even though this is handled off-site, it is important that it is available and data is not tampered with on the way to the requesting user.  

Patients must input sensitive data, such as national identification number, name, date of birth, contact details and basic health information. This data is an asset, and the system will not function if this data has been disrupted, e.g. altered, falsey or wrong. It is important this data is validated upon input, and kept safe from attackers at all times.

Patient vitality data, measurements taken at a patients home and then sent to the system, is a vital asset to the organization. A disruption would cause a severe impact on the healthcare professionals ability to complete their task, and can cause massive damage to the hospitals reputation and even include damage or loss of life of a patient.

In every step of the way for data transported on the system, the data is logged. This includes metadata, for example from application traffic between two clients (e.g. patient and doctor), and eventlogs. Eventlogs are there to provide a look into what happened, and is necessary when something goes wrong. The logs may be disrupted, for example, in an attack and the attacker tries to erase logs to hide the attack or make the forensic work take longer.

To rank the identified assets we found, we use the National Institute of Standards and Technology asset ranking to rank our assets (NIST 800-18): 

.. image:: ../images/NIST_AssetRanking.png

Source: https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-18r1.pdf; 19.09-2020.

This is how we prioritize the identified assets in terms of confidentiality, integrity and availability. They are given a "low", "moderate", or "high" score dependent on the severity a disruption to the asset will cause. The "Score" column is for the asset prioritization and is the common score gained by confidentiality, integrity and availability.

.. csv-table::
	:header: **Asset**, **Confidentiality**, **Integrity**, **Availability**, **Score**
	:widths: 50, 15, 15, 15, 15

	"Authentication and Authorization Server", "High", "High", "High", "High (H)"
	"Database Server", "Low", "High", "Medium", "Medium (M)"
	"Webserver", "Low", "High", "High", "Medium (M)"
	"Internal Servers", "High", "High", "Low", "Medium (M)"
	"Authenticative data", "High", "High", "High", "High (H)"
	"Cookies (from webserver)", "Low", "Low", "Low", "Low (L)"
	"Logs (metadata, eventlogs, etc.)", "Low", "Medium", "High", "Medium (M)"
	"Configuration data", "Medium", "High", "Low", "Medium (M)"
	"System software", "High", "High", "High", "High (H)"
	"Science data", "Low", "Medium", "Low", "Low (L)" 
	"EHR", "Medium", "High", "High", "High (H)"
	"User data (e.g. date-of-birth, ID)", "High", "High", "Low", "Medium (M)"
	"Patient vitals (e.g. blood pressure)", "High", "High", "High", "High (H)"

.. \* Access to, for example, the webservers "robot.txt" (which can give information about file hierarchy) will most likely only be used for reconnaissance. 
	^^ Should stay or go?

Given the asset score, this is how we rank their prioritization of the assets:

.. csv-table::
	:header: **Asset Score**, **Description**
	:widths: auto

	"High (H)", "Very costly loss of major tangible assets or resources; significant violation of an organization’s mission, reputation or interest; or human death or serious injury"
	"Medium (M)", "Costly loss of tangible assets or resources, violation of an organization’s mission reputation or interest, or human injury"
	"Low (L)", "Loss of some tangible assets or resources or an effect on an organization’s mission, reputation or interest"

To sum up, we see that assets the hospital should focus mostly on user and patient data, the authentication and authorization security and their respective data, and finally the system software on the internal computers.

.. 
	"System Administrators", "HIGH", "HIGH", "HIGH"
	"Users", "HIGH", "HIGH", "HIGH"

.. 
   Identify the main assets that the system consists of
   ----------------------------------------------------
       -  Authentication server
       -  System administrators
       -  User:
          -  Patients
          -  Healthcare
          -  Social workers
       -  Patient/Healthcare environment
       -  EHR
