Main Assets
===========
The main assets we have identified are crucial for the organization/hospital and is relevant to the task. First, we have the authentication server/system which will authenticate incoming requests. Next, we have the system administrators, whom are responsible for authenticating healthcare workers in the system. 

Users of the system, such as patients, healthcare workers and social workers are also assets of the system, as they generate the data that is most vital to the system. Breaking this trust to the customers, would affect the system and hospitals credibility. 

.. Credibility is another identified asset to the organization, because damage to the organizations credibility would impact the organizations ability to perform its task as fewer users may want to use the system.  

The Electronic Health Registry (EHR) is also vital to the organization. A disruption in this tool will prevent the healthcare personnel from doing their work and help their patients. 

Patients must input sensitive data, such as national identification number, name, date of birth, contact details and basic health information. This data is an asset as the system will not function if this data has been disrupted, e.g. altered, falsey or wrong. 

.. 
   Should this be included?

Patient vitality data, measurements taken at a patients home and then sent to the system, is a vital asset to the organization. A disruption would cause a severe impact on credibility and the healthcare professionals ability to complete their task. 

.. end of commment above ^

To rank the identified assets we found, we used the National Institute of Standards and Technology asset ranking to rank our assets:

.. image:: ../images/NIST_AssetRanking.png

Source: https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-18r1.pdf 

This is how we prioritize the identified assets in terms of confidentiality, integrity and availability. They are given a "low", "moderate", or "high" score dependent on the severity a disruption to the asset will cause.

.. csv-table::
	:header: **Asset**, **Confidentiality**, **Integrity**, **Availability**
	:widths: 40, 15, 15, 15

	"Authentication Server", "HIGH", "HIGH", "HIGH"
	"System Administrators", "HIGH", "HIGH", "HIGH"
	"Users", "HIGH", "HIGH", "HIGH"
	"EHR", "HIGH", "HIGH", "HIGH"
   "User data", "HIGH", "HIGH", "HIGH"
   "Patient vitals (e.g. blood pressure)", "HIGH", "HIGH", "HIGH"



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
