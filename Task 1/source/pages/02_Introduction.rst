Introduction
============

This paper covers a fictional case study for an "out-patient healthcare
monitoring system" to be used between healthcare workers and their patients and
is the first mandatory delivery for IMT3501 - Software Security at NTNU Gjøvik
fall 2020. First, we will state some assumptions regarding this project. Based
on our assumptions, we will identify core business goals for the organization in
order to define a scope for the system.

Furthermore, functional specifications for our case will be defined, followed by
a more in-depth security requirements specification process.

Assumptions and clarifications
------------------------------
   - We assume that this solution will take place in Norway and according to
     Norwegian laws and policies.
   - We assume the company requires the use of a secure development framework.
   - We are aware that our security requirement specification might not cover everything
     in the field. Our requirement specification just touches the surface of the necessities
     needed in such a real-world project. We have tried finding the most relevant and
     important requirements for the scope and time limitations of our case.

Identifying business goals
--------------------------

The goal of the Out-patient Healthcare Monitoring system is to build a healthcare
monitoring system for patients that are discharged and have returned home from the
organization. This way healthcare workers can monitor and follow up on their
patients' health status. It is also important for the business that the patients
can communicate with the healthcare workers in order to update them on their
current status. To ensure correct patient information at all times,
healthcare workers should be able to find and edit their information through the
system.

As this system processes a lot of sensitive personal information, secure storage
and data transfer is of importance for the healthcare organization. System
actors should be able to use the system with trust and confidence. Thus
retaining the confidentiality of user information is a high priority for the
organization. It is also important that healthcare workers are able to update
information about patients effectively, so that the organization ensures
preservation of integrity regarding "basic healthcare information". Failing to
do so may cause serious trouble for patients in a medical manner.

In order to follow up discharged patients correctly, ensuring
system availability is important. Discharged patients should be able to reach the healthcare
organization without undue trouble. Failing to do so may consume precious time in a
possibly critical health situation. The organization wants to ensure that newly
discharged patients in particular feel safe by means of a stable and highly available system.

Definitions
-----------

.. csv-table::
  :header: **Term**, **Definition**
  :widths: 15, 40

	"**EHR**", "Electronic health record"
  "**GP**", "General Practitioner"
  "**DB/DBMS**", "Database/database management system"
  "**SR**", "Security requirement"
  "**GDPR**", "General Data Protection Regulation"
  "**User**", "A user of the healthcare system is defined as either a patient (including eventual relatives), a social worker or a healthcare worker (doctors, nurses etc.)"
