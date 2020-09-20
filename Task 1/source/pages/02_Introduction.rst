Introduction
============

This paper covers a fictional case study for an "Out-patient healthcare
monitoring system" to be used between healthcare workers and their patients and
is the first mandatory delivery for IMT3501 - Software Security at NTNU Gjøvik
fall 2020. Firstly, we will cover some assumptions regarding this project. Based
on our assumptions, we will identify core business goals for the organization in
order to define a scope for the system.

Furthermore, functional specifications for our case will be defined, followed by
a more in-depth security requirements specification process.

Assumptions
-----------
   - We assume that this solution will take place in Norway and according to
     Norwegian laws and policies.
   - We assume the company requres the use of a secure development framework. 

Identifying business goals
--------------------------

The Out-patient Healthcare Monitoring system wish to build a healthcare
monitoring system for patients that are discarded and returned home from the
organization. This way healthcare workers might watch and followup on their
patients health status. It is also important for the business that the patients
to be able to communicate with the healthcare workers in order to update their
current situations. To ensure correct patient information at all times,
healthcare workers should be able to find and edit their information through the
system.

As this system processes a lot of sensitive personal information, secure storing
and data transfer is of importance for the healthcare organization. System
actors should be able to use the system with trust and confidence, thus
retaining the confidentiality of user information is a high priority for the
organization. It is also important that healthcare workers are able to update
information about patients effectively, so that the organization ensures
preservation of integrity regarding "basic healthcare information". Failing to
do so might cause serious trouble for patients in a medical manner. (Vi burde
kanskje ha noe policies på dette (?))

In order to followup discarded patients correctly, it is important to ensure
system availability. Discarded patients should be able to reach the healthcare
organization without troubles. Failing to do so might lessen precious time in a
possible serious health situation. The organization wants to ensure that newly
discarded patients especially, feels safe through a stable and available system.

Definitions
-----------

   - **EHR:** Electronic health record.
   - **GP:** General Practitioner.
   - **DB/DBMS:** Database and database management system.
   - **SR:** Security Requirement.
   - **GDPR:** General Data Protection Regulation.
