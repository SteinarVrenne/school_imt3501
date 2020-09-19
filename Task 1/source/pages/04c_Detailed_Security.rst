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


SR.09 - Prohibit short passwords
""""""""""""""""""""""""""""""""

| **Requirement categories:** Non-repudiation.
| **Security Mechanism:** Mitigate.
| **Related assets:**
| **Requirement:** Passwords shorter than 8 characters long should be prohibited,
  in order to mitigate the process of potential bruteforce attacks.


SR.10 - Inactive user sessions should terminate
"""""""""""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Availability, identification & authentication
| **Security Mechanism:** Mitigation.
| **Related assets:**
| **Requirement:** User sessions that has been inactive for more than 15 minutes
  should be terminated in order to mitigate the risk of session cookies being stolen.


SR.11 - Logfiles needs to be detailed
"""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Accountability.
| **Security Mechanism:** Detection.
| **Related assets:**
| **Requirement:** Event logfiles needs to be detailed and include timestamps,
  event types and healthcare worker identity.


SR.12 - Cancellation of system admins access rights
"""""""""""""""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Integrity, secure maintenance, immunity, authorization, authentication.
| **Security Mechanism:** Prevention.
| **Related assets:**
| **Requirement:** Access rights for system administrators should be terminated
  upon resignation in order to prevent unauthorized access after the business relationship.


SR.13 - The system should not be accessible outside Norwegian borders
"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

| **Requirement categories:** Availability, identification & authentication, intrusion detection.
| **Security Mechanism:** Prevention.
| **Related assets:**
| **Requirement:** As this system is designed for Norwegian healthcare only, it
  should not be reachable for IP addresses outside of Norway.




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
