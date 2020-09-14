Identify and specify detailed (fine-granular) security requirement of the system.
--------------------------------------------------------------------------------- 


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
| Summary           | Data should not be stored in a way, that would made it possible for an attacker do dump every data record.   |                                |
+-------------------+--------------------------------------------------------------------------------------------------------------+
| Description       | To prevent mass leakage of data records, we can spread the stored information to multiple databases. If an   |
|                   | attacker somehow gains access to one of the database files, it will not be able to tie that information to   |  
|                   | anyone.                                                                                                      |
+-------------------+--------------------------------------------------------------------------------------------------------------+

