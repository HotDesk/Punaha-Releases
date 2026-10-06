# Pūnaha Product and Support privacy notice

Version: rc1-20261006-v1 | 6 October 2026

## Who handles information

Hot Desk Consultancy Services Limited, Wellington, New Zealand, provides Pūnaha and handles the registration and Support information described here. Contact privacy@punaha.com about access, correction or a privacy concern. We may need to verify your identity before disclosing or changing information. You may also contact New Zealand's Office of the Privacy Commissioner at https://www.privacy.org.nz/.

The operator of a customer-hosted installation controls its local accounts, databases, content, logs, integrations and backups. If an organisation operates the installation you use, contact that organisation about its handling of your information. This notice does not replace its own privacy obligations. The public marketing website has a separate notice at https://punaha.com/privacy.

## Information kept in your installation

Product stores the information needed for the features you choose: accounts and permissions, authentication records, documents and searchable content, model and integration settings, prompts and responses, workflows and cases, operational history, audit events and logs. The content and connection details depend on your configuration. Administrators control local retention, exports, storage and backups. Logs and diagnostics can contain identifiers and operational details; review and minimise them before sharing.

Registering the installation does not upload its documents, prompts, database contents, passwords or private signing keys. Separately configured external models, cloud stores, identity providers, connectors, email actions or other workflow steps can send information to the destinations selected by your administrator or users. Review those destinations and their terms before enabling them.

## Registration, activation and renewal

Product keeps a protected local and Control-database record of the installation identity, node identity, TPM powered-clock readings, activation serial, registered term and consumed registration allowance. It uses these records to enforce 720 powered-on hours for initial registration and each renewal period, detect rollback and coordinate cluster nodes. These clock records are not included in the registration request or continuously sent to Support. Licence expiry stops ordinary processing after the allowance; it does not delete customer data.

The administrator initiates registration or exports an encrypted registration request. The request identifies the installation and product build, its public verification key and fingerprint, request identifiers and validity times, and its node inventory. Node information includes identifiers, display names, roles, membership status and hardware details such as operating system, CPU, memory, GPUs and storage capacity. Recovery and decommissioning requests additionally contain the relevant licence reference, requested action, reason and installation-binding evidence. Avoid personal names or sensitive business information in node names and free-text reasons unless needed.

Before an online registration request, Product offers a separate choice to include the signed-in user's email as a Support contact hint. Declining that choice does not send the hint. Offline request files do not include that email hint. Support still needs a verified account and contact email to identify the person completing registration; this is collected directly by Support and does not transfer the Product password or session.

Support records the account holder's name and verified email, customer name, organisation or personal registration context, membership and authority, exact legal document identifier/version/hash, acceptance time and method, review decisions, activation history and security/audit events. These records support registration, licence renewal, account security, recovery, troubleshooting and evidence of the terms accepted. If required registration information is not supplied, an activation cannot be issued and the initial registration allowance can expire.

## Authentication and optional services

Local Support login uses password hashes rather than storing the chosen password in readable form. If organisational single sign-on is configured, the configured identity provider receives sign-in requests and returns identity claims needed to link the account. Session cookies and browser storage support authentication and the interface.

Optional support or billing records may include the selected installation, service/order description, approval reference, amount, status, provider reference and acceptance evidence. When an enabled hosted payment provider is used, payment details are entered with that provider. The implemented billing boundary uses Airwallex sandbox or a local simulator; this RC preparation does not enable live payments. Product licensing remains free and independent of support purchases.

The inspected Support build is a development runtime: verification and invitation messages can be held in its local development outbox, and production hosting and email delivery require separate configuration. This notice does not represent those services as already deployed.

## Recipients and locations

Authorised customer administrators and authorised Pūnaha staff can access information for their assigned tasks. Configured hosting, database, email, identity and payment providers may process the information needed to provide their services. The customer chooses providers used by its Product installation. Information sent to external services may be processed outside New Zealand or the customer's location according to those services and the deployment arrangements. Production Support provider locations must be communicated as part of production onboarding; this candidate does not promise a particular hosting country.

If another administrator invites you or supplies your information, it may come from that administrator rather than directly from you. We use it for the stated account, registration or service purpose. Do not supply another person's information without appropriate authority and notice.

## Retention, security and choices

Local Product retention depends on the installation's settings and the operator's records and backup practices. Licence expiry does not delete local data. Support registration, activation, acceptance, billing and audit records are retained for account/service operation, security, dispute handling and applicable record-keeping obligations. Expired sessions or tokens cannot be used as fresh authorisation; that does not mean all associated records are automatically deleted. Licence expiry or uninstall does not itself delete Support records, and this build does not implement a general automatic purge of those records. Contact us to discuss access, correction and retention of your information.

Access controls, protected secrets, signed registration/activation records and encrypted offline transport help protect information. No system is guaranteed completely secure. Protect exported files and backups and do not share credentials or private keys with Support. Provide only the diagnostic material needed for the issue and remove unrelated personal or confidential content first.

The Product registration flow does not enable marketing analytics or continuous vendor access to customer content. Optional external integrations and any separately visited public website follow their own configuration and notices. Choosing to share an email hint is distinct from accepting software terms or receiving this notice. A new notice version will identify material changes in this handling.
