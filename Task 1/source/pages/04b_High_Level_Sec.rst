    b. Identify and specify high level security requirements for the whole system
    -----------------------------------------------------------------------------

    - Logfiles should be detailed enough to point out the identity of a user, in case of a special event occurs.
    - A user shall not be able to create a password shorter than 8 characters long.
    - Data should not be stored in a way, that would made it possible for an attacker do dump every data record. 
        - Segregated 
    - The website must not be able to return any personal information, without the right access credentials.
    - Passwords must be encrypted.
    - The website have to be designed in a way, that it can not accept invalid URL requests.
    - System administrators shall not be able to read any patient information.
    - The website shall not be able to be accessed outside of the norwegian border.
        - Mitigates attacks from foreign countries. 
    - Required to use some sort of two-factor authentication when you have access that exceeds what a patient has.
    - A session lock that logs the user out after inactivity. 
    - Have regularly  encrypted backups.
    - The website must be secured with HTTPS protocol.
    - There server shall be secured with authentication and surveillanced at all time.
    - The servers operative system shall be patched with the latest security patches.
    - A system administrators access shall be terminated upon resignation. 

    .. Source: https://safecomputing.umich.edu/information-security-requirements
    