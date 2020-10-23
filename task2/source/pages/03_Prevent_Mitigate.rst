Prevent / Mitigate attacks
==========================

In this section, mitigations for the threats identified in the previous section
will be presented. Each mitigation will be described by the threat ID it applies
to, and will be categorized into a type of mitigation, as follows:

.. csv-table::
  :header: **Type**, **Definition**
  :widths: 15, 40

  "Remediate", "The threat in question can be partially or fully mitigated by implementing specific best practices."
  "Transfer", "The underlying issue cannot be directly remediated, although steps can be taken to transfer the risk to another component of the system."
  "Accept", "The threat cannot be mitigated, or the threat is not considered severe enough to require remediation."

.. csv-table::
  :header: **Threat ID**, **Type**, **Mitigation**
  :widths: 5, 10, 50

  "T01", "Remediate", "Implement current best practice on secure communication channels, including mandating TLS for all connections."
  "T02", "Remediate", "Ensure proper string escaping is done for all database inputs."
  "T03", "Accept", "This might happen and indicates that the firewall/router is misconfigured and must be updated."
  "T04, T05", "Transfer", "Implement strict access controls, keep all systems up to date, follow best practices on the principle of least privilege, and utilize contractual and legal controls to handle data breaches."
  "T06", "Remediate", "Ensure all software is kept up to date, that all security patches are automatically applied, and that devices are routinely scanned for outdated software."
  "T07", "", ""
  "T08, T09", "Remediate", "Review failure alerts received from devices and audit the configuration of security software to ensure logging takes place."
  "T10", "Remediate", "Synchronize configuration automatically across devices using industry standard practices for device fleet management."
  "T11", "", ""
  "T12", "Transfer", "Use security logs to detect and, where possible, prevent unusual traffic, based on a security incident and event management tool."
  "T13", "Transfer", "Perform a security audit on client-side software and implement fixes for any findings. Risk is thus dependent on the quality of the audit."
  "T14", "Accept", "Restart logging, and monitor the system to try to identify the root cause."
  "T15, T17", "Remediate", "Implement best practice for load balancing and/or clustering, and use dynamic scaling of server resources to match the incoming volume of requests."
  "T16", "Transfer", "Establish a service level agreement (SLA) with the third party vendor to define a specific, maximum tolerable amount of downtime, and a clear process to be executed by the vendor if this agreement cannot be met."
  "T18", "Remediate", "Ensure that a failover system is available on-demand with high availability that can handle incoming traffic while the main service is unavailable."
  "T19", "Remediate", "Bind session cookies to a specific IP address and ensure that session cookies have limited validity. Require reauthentication before performing critical tasks, such as changing the user's password."
  "T20", "Remediate", "Require multi-factor authentication for all healthcare workers."
  "T21", "Accept", "In an emergency where the system is unavailable, communication can fall back to conventional means, such as by telephone call to emergency services."
  "T22", "Transfer", "Introduce contractual and legal measures to deter system administrators from unauthorized access. Mandate logging of all login attempts, and mandate notifications to be sent to the user in question whenever their credentials are updated."
  "T23", "Remediate", "Implement industry best practices for enforcing principle of least privilege, and do not give system accounts access to patient information."
  "T24, T26", "Transfer", "Ensure due process for human resources to contact the IT department in cases where an employee is terminated."
  "T25", "Transfer", "Utilize contractual and legal measures to deter escalation of privileges by users. Establish logging for all security-related events, and utilize a security incident and event management tool to monitor systems for unusual behavior."
  "T27", "Transfer", "Ensure contractual and legal measures are established in the event that this happens. Ensure that the event can be backed up by evidence, such as logging all sign-in and data update requests."
  "T28", "Remediate", "Log all attempts to access patient data on a secure system."
  "T29", "Remediate", "Ensure industry best practices are implemented regarding auditing and logging of high privilege activity."
  "T30", "Accept", "Mandating patients to disclose information about their health could have legal privacy implications."
  "T31", "Remediate", "Ensure all updates to patient data is logged in conjunction with the user that performed the update."
  "T32", "Transfer", "Ensure users are able to get in contact with a help desk to log tickets regarding system malfunction."
