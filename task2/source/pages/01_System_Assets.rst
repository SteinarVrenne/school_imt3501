System assets
-------------

- Revisit task 1 and identify and prioritize the system assets.
    - Sensitive and personal information.


    - What are the most critical assets for your system. Categorize based on CIAproperties.


    - Does your system access/use/share assets with/ to other third party.


From task 1 we identified the following assets in the system: "Authentication and Authorization Server", "Database Server", "Webserver", "Internal Servers", "Authenticative data", "Cookies (from webserver)", "Logs (metadata, eventlogs, etc.)", "Configuration data", "System software", "Science data", "EHR (Electronic Health Register", "User data (e.g. date-of-birth, ID)", "Patient vitals (e.g. blood pressure)"


This is how we prioritize the identified assets in terms of confidentiality,
integrity and availability. They are given a "low", "moderate", or "high" score
dependent on the severity a disruption to the asset will cause. The "Score"
column is for the asset prioritization and is the common score gained by
confidentiality, integrity and availability.

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
	"EHR (Electronic Health Register", "Medium", "High", "High", "High (H)"
	"User data (e.g. date-of-birth, ID)", "High", "High", "Low", "High (H)"
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

To sum up, we see that assets the hospital should focus mostly on are user and
patient data, the authentication and authorization security and their respective
data, and finally the system software on the internal computers.