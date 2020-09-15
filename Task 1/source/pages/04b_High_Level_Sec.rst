Identify and specify high level security requirements for the whole system
--------------------------------------------------------------------------

These are our highlighted security requirements for the system.
**(Tenker vi endrer denne tabellen til kun "titler" på kravene, og utdyper de videre i 4c slik som i ITSM. Fikser senere)**

.. csv-table::

  "**Requirement index**", "**Requirement specification**"
	"SR.01", "Logfiles should be detailed enough to point out the identity of a user, in case of a special event."
	"SR.02", "A user shall not be able to create a password shorter than 8 characters long."
	"SR.03", "Data should not be stored in a way that makes it possible for an attacker to dump data records."
	"SR.04", "Users without corresponding permissions should not be able to retrieve any personal patient-information from the website."
  "SR.05", "All passwords must be encrypted."
  "SR.06", "The website should not accept invalid URL requests."
  "SR.07", "System administrators should not be able to read any patient information in any way."
  "SR.08", "Two-factor authentication is required for all users that has higher privileges than patients."
  "SR.09", "Inactive user sessions should terminate after inactivity."
  "SR.10", "Encrypted backups should be performed regularly."
  "SR.11", "The website should be secured with encryption (TLS)"
  "SR.12", "Authentication, authorization and system monitoring should be present at all times."
  "SR.13", "Operating systems and softwares used in the healthcare system should always stay up to date with the latest updates/patches."
  "SR.14", "A system administrators access shall be terminated upon resignation."
  "SR.15", "The website shall not be able to be accessed outside of norwegian borders. "

.. Source: https://safecomputing.umich.edu/information-security-requirements
