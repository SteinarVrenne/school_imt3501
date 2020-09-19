Identify and specify the main use cases of the system
-----------------------------------------------------

The Use Cases for this system is mainly performed by 4 main actors, Healthcare worker, System administrator, Patient-at-home devices and the Patient actor. The Patient actor is an abstraction for social workers and family members, whom function the same as a Patient actor. Patient-at-home devices are typically devices stationed at a patients home that will continually deliver data to the system about the patients vitals, such as blood sugar, blood pressure etc.. 

The diagram below represents the main use cases we have identified for this system.

.. Use cases 

.. Use case Tables

The tables below are detailed Use Case descriptions of flow for where the diagram fails to explain what is happening.

.. csv-table::
	:header: **UC - Log in as User**, **Description**
	:widths: 3, 10

	"Actor", "Patient"
	"Prerequisites", "Is a registered user"
	"Post requisites", "User is logged in"
	"Main flow", "1. User enters credentials 2. Credentials are sent to authentication server 3. User is logged in"
	"Side flow", ""
	"Deviations", "1.1 User enters wrong credentials and is returned an error"

.. csv-table::
	:header: **UC - Log in as Healthcare worker**, **Description**
	:widths: 3, 10

	"Actor", "Healthcare worker"
	"Prerequisites", "Is a registered user"
	"Post requisites", "Healthcare worker is logged in"
	"Main flow", "1. Healthcare worker enters credentials 2. Credentials are sent to authentication server 3. Healthcare worker is logged in"
	"Side flow", ""
	"Deviations", "1.1 Healthcare worker provides wrong credentials and is shown error message"

.. csv-table::
	:header: **UC - Log in**, **Description**
	:widths: 3, 10

	"Actor", "Patient and Healthcare worker"
	"Prerequisites", "Is a registered user"
	"Post requisites", "Actor is logged in"
	"Main flow", "1. Actor has sent right credentials 2. Authentication server approves 3. Authentication server sends approved"
	"Side flow", ""
	"Deviations", "1.1 Actor provides wrong credentials and is shown error message"

.. csv-table::
	:header: **UC - Register new Patient**, **Description**
	:widths: 3, 10

	"Actor", "Patient"
	"Prerequisites", ""
	"Post requisites", "Actor is now registered"
	"Main flow", "1. Actor sends in basic and sensitive information 2. Authentication server receives request 3. Authentication server creates user"
	"Side flow", ""
	"Deviations", "1.1 Actor provides invalid info and is denied a user"

.. csv-table::
	:header: **UC - Register new Healthcare worker**, **Description**
	:widths: 3, 10
	"Actor", "System Adminstrator"
	"Prerequisites", "Is a registered and valid user"
	"Post requisites", "New Healthcare worker account is made"
	"Main flow", "1. Actor has sent right credentials 2. Authentication server approves 3. Authentication server sends approved"
	"Side flow", ""
	"Deviations", "1.1 Actor provides invalid info and is returned an error"

.. csv-table::
	:header: **UC - Register new Patient**, **Description**
	:widths: 3, 10
	"Actor", "Patient"
	"Prerequisites", "Has valid identification"
	"Post requisites", "Patient has now an account in the system"
	"Main flow", "1. Actor has sent right credentials 2. Authentication server approves 3. Authentication server sends approved"
	"Side flow", ""
	"Deviations", "1.1 Actor provides invalid info and is returned an error"

.. csv-table::
	:header: **UC - Register new user**, **Description**
	:widths: 3, 10

	"Actor", "Patient and system administrator"
	"Prerequisites", ""
	"Post requisites", "New user has been created"
	"Main flow", "1. Actor has sent right credentials to authentication server 2. Authentication server creates new user 3. Authentication server returns success"
	"Side flow", ""
	"Deviations", "1.1 Actor provides invalid info and authentication server returns an error"
