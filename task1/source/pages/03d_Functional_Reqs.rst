Identify and specify the functional requirements of the system
--------------------------------------------------------------


Below is a list of what functionalities the platform must offer. These requirements say what the website must contain, and how it should function.

*FR = Functional requirement No.*

- FR 01: The webpage shall have a homepage, with a highly visible login button, that will take the user to its own homepage.
- FR 02: The system administrators shall have a admin panel, that contains server information no other users have access to. This admin panel shall also have a feature to add new health workers to the system.
- FR 03: A "Contact page" shall provide the name and contact information to all of the health care workers that is responsible for that patient.
- FR 04: Patients shall be able to enroll their personal information, to create an account.
- FR 05: The homepage of healthcare workers should contain a inbox, with messages from their patients.
- FR 06: The system administrators shall receive a warning, if the servers have more then 75% system load, and less than 15% storage left.
- FR 07: Healthcare workers shall have a way of making contacts with other workers, and send messages between each other.
- FR 08: When a health worker clicks on one of their patients, they shall receive the patients health record, current medications, day journal, and personal information.
- FR 09: The patients homepage shall contain a day journal, in which they can write down how they feel each day. The health care workers assigned to them shall have access to reading the journal.
- FR 10: The login page shall have protection against brute-force login, and sql injection. After 5 failed login attempts, the user shall receive an email about their failed login attempts, with a link to resetting their password.
- FR 11: No downtime during the days. Since there will be less activities in the nights, with less health care workers on shift, the system have a maximum downtime of 10 minutes for one day.
- FR 12: The system shall have a response time within 5 seconds. If the website uses longer time to respond, the system administrators will receive a notification, and have to respond rapidly to minimize the response time.
- FR 13: The website must scale to be be usable on mobile devices.
- FR 14: Healthcare workers shall only be able to register using their work email.
- FR 15: The system shall be updated with patient vitals provided with Patient-at-home devices connected to the system.
