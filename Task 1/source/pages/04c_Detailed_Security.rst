Detailed security requirements specification
--------------------------------------------

In this part, we will cover the details of our security requirements specification process.
Our specified requirements will be indexed and ordered in the manner of importance.
To elaborate further on each requirement, it will be described a little more detailed.
In addition, the requirement will also be tied up to a class, category and related system assets.
These are defined in the "Definitions" section.

SR.01 - Data should be securely stored
""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Confidentiality, Privacy.
| **Security Mechanism:** Mitigate.
| **Related assets:**
| **Requirement:** Data about patients should be stored securely in order to
  protect users privacy, maintain confidentiality and mitigate exposure in case of an unauthorized data dump.


SR.02 - Authorized users only should be able to access patient information
""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Integrity, confidentiality, authorization, privacy.
| **Security Mechanism:** Prevention.
| **Related assets:**
| **Requirement:** Authorized healthcare workers only should be able to access
  patient information such as ... ... to prevent leakage of sensitive patient data.


SR.03 - System monitoring should be present at all times
""""""""""""""""""""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Availability, intrusion, accountability.
| **Security Mechanism:** Detection.
| **Related assets:**
| **Requirement:** Monitoring of system assets such as ... ... should be present at all times in order to
  detect potential intrusions, unauthorized access, system errors or down time.


SR.04 - OS and Software should be updated
"""""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Integrity, immunity.
| **Security Mechanism:** Mitigation.
| **Related assets:**
| **Requirement:** Operating systems and software used in the healthcare system
  should always stay up to date with the newest patches in order to mitigate
  possible vulnerabilities.


SR.05 - Encrypted backups are required.
"""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Confidentiality, secure maintenance.
| **Security Mechanism:** Response.
| **Related assets:**
| **Requirement:** Encrypted backups related to ... and ... are required and should be performed
  regularly in order to maintain confidentiality and proper response in case of a system breakdown.


SR.06 - Passwords should be hashed
""""""""""""""""""""""""""""""""""

| **Requirement categories:** Confidentiality.
| **Security Mechanism:** Mitigation.
| **Related assets:**
| **Requirement:** All passwords stored in the systems databases should be
  hashed with a secure hash algoritm, such as e.g. SHA-256, in order to prevent
   clear text exposure in case of a data breach.


 SR.07 - Web-application communication needs to be encrypted
 """""""""""""""""""""""""""""""""""""""""""""""""""""""""""

 | **Requirement categories:** Confidentiality, immunity.
 | **Security Mechanism:** Prevent.
 | **Related assets:**
 | **Requirement:** All communication related to the system web-application should
  benefit TLS encryption in order to prevent ... ... sent in clear text and malicious packet sniffers.


SR.08 - Two-factor authentication is required
"""""""""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Integrity, identification & authentication.
| **Security Mechanism:** Prevention.
| **Related assets:**
| **Requirement:** Two-factor authentication is required for all users that has
  a higher level of privileges than patients in order to prevent unwanted access to
  sensitive patient information.


SR.08 - Prohibit short passwords
""""""""""""""""""""""""""""""""

| **Requirement categories:** Non-repudiation.
| **Security Mechanism:** Prevention
| **Related assets:**
| **Requirement:** Two-factor authentication is required for all users that has
  a higher level of privileges than patients, in order to prevent unwanted access to
  sensitive patient information.



Kategorier (ignorer):
  - Identification & Authentication: ensures that users and applications are correctly identified and the identities are verified
  - authorization: Ensures that users and applications can only access data and functions they are authorized to
  - Immunity: prevent unauthorized code and programs from infecting the application
  - Intrusion detection: detect any attempt to intrude into the system
  - Non-repudiation: ensure that users and entities can not deny (not) performing an interaction
  - Privacy: ensure privacy related rules and regulations. Ensure PbD principles and compiant with GDPR
  - Security auditing - accountability: ensure the possibility to audit and
    monitor the status of critical and security functions. Audit should
    include information such as ID, event, time, and asset
  - Secure maintenance: ensure secure maintenance and secure operations, e.g., configuration management


Deterrence, Prevention, detection, mitigation, and response

Liste (ignorer):

- Data should be securely stored.
- Users need to be authenticated in order to authorize.
- Only authorized users should be able to access patient information.
- System monitoring should be present at all times.
- OS and softwares used should always stay up to date.
- Encrypted backups should be performed regularly.
- All passwords should be encrypted.
- The website should be secured with encryption (TLS).
- Two-factor authentication is required for user sign in.
- All passwords should be at least 8 characters long.
- Inactive user sessions should terminate after inactivity.
- Logfiles should be detailed enough to point out the identity of a user.
- A system administrators access shall be terminated upon resignation.
- The website should not accept invalid URL requests.
- The system should not be accessable outside Norwegian borders.













+-------------------+--------------------------------------------------------------------------------------------------------------+
| SR.01                                                                                                                            |
+===================+==============================================================================================================+
| Requirement name: | Detailed logfiles                                                                                            |
+-------------------+--------------------------------------------------------------------------------------------------------------+
| Summary           | Logfiles should be detailed enough to point out the identity of a user, in case of a special event occurs .  |
+-------------------+--------------------------------------------------------------------------------------------------------------+
| Description       | The websites logfile shall have a detailed logging system. Every event that is logged must have added the    |
|                   | correspondent user ID to the event.  With this added information, the system administrators, which are       |
|                   | responsible for any security occurrences will easily be able to pinpoint who to blame.                       |
+-------------------+--------------------------------------------------------------------------------------------------------------+


+-------------------+--------------------------------------------------------------------------------------------------------------+
| SR.02                                                                                                                            |
+===================+==============================================================================================================+
| Requirement name: | Prohibit short passwords.                                                                                    |
+-------------------+--------------------------------------------------------------------------------------------------------------+
| Summary           | A user shall not be able to create a password shorter than 8 characters long.                                |
+-------------------+--------------------------------------------------------------------------------------------------------------+
| Description       | In order to prevent brute force attack, we will enforce users to create passwords longer than 8 characters   |
|                   | long.                                                                                                        |
+-------------------+--------------------------------------------------------------------------------------------------------------+


+-------------------+--------------------------------------------------------------------------------------------------------------+
| SR.03                                                                                                                            |
+===================+==============================================================================================================+
| Requirement name: | Separate stored information                                                                                  |
+-------------------+--------------------------------------------------------------------------------------------------------------+
| Summary           | Data should not be stored in a way, that would made it possible for an attacker do dump every data record.   |
+-------------------+--------------------------------------------------------------------------------------------------------------+
| Description       | To prevent mass leakage of data records, we can spread the stored information to multiple databases. If an   |
|                   | attacker somehow gains access to one of the database files, it will not be able to tie that information to   |
|                   | anyone.                                                                                                      |
+-------------------+--------------------------------------------------------------------------------------------------------------+
