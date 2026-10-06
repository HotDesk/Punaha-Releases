# Pūnaha downloads

Official release information and installation downloads from Hot Desk Consultancy Services Limited.

**Pūnaha 0.1 RC1 is being prepared. No installer release is publicly available from this repository yet.** The candidate remains a draft while redistribution and installation/registration acceptance checks are completed. A release candidate is for evaluation and acceptance testing.

This repository holds release documentation. The proprietary application source is maintained separately. GitHub's automatically generated **Source code** ZIP and tar.gz contain this repository's documents, not an installer or the application source.

## Current software offer

Pūnaha is one full proprietary product. The current issued **12-month licence term costs US$0**, starting on the signed activation's stated issue date. Personal and organisational use, multiple versions and independently registered installations are permitted, subject to technical compatibility and registration. Optional paid support is separate.

Future renewal pricing is undecided and may include a charge based on demand for additional functionality and the actual cost of maintaining and developing the software. Any proposed price and terms will be disclosed in advance. Paid renewal requires explicit acceptance; there is no automatic charge or obligation to renew. Existing issued terms and previously accepted commitments are honoured.

Read the complete [software licence](PUNAHA-LICENCE.md) and [privacy notice](PRIVACY.md). Availability on GitHub does not grant an open-source licence to the proprietary application. Third-party components retain their own terms, notices and applicable supplied source in each complete download.

## Registration and expiry

**Renew or export your data before the access cutoff.** A new installation after setup, and each expired registered term, has a **720 TPM powered-on-hour allowance**. This is not 30 calendar days, and includes time the TPM is powered on while the Product service is stopped.

After the allowance ends, ordinary processing, administration, customer-data access and exports stop. Data is retained, but Product access and export remain unavailable until valid registration or renewal is restored. Only necessary sign-in, registration, renewal, activation and recovery functions remain available. Online and offline activation both require the completed registration process; submitting a request alone is insufficient.

## Planned RC1 downloads

| Platform | Complete download |
|---|---|
| Windows x64 | `punaha-0.1.0-rc.1-terms-v2-windows-amd64.zip` |
| Ubuntu amd64 | `punaha-0.1.0-rc.1-terms-v2-ubuntu-amd64.tar.gz` |
| Debian 13 amd64 | `punaha-0.1.0-rc.1-terms-v2-debian13-amd64.tar.gz` |
| RHEL 9 x86_64 | `punaha-0.1.0-rc.1-terms-v2-rhel9-x86_64.tar.gz` |

The intended release tag is `v0.1.0-rc.1-terms-v2`. The embedded application version remains `0.1.0-rc.1`; `terms-v2` distinguishes this revised licence candidate. The public tag identifies these release documents; [RELEASE-INFO.json](RELEASE-INFO.json) records the separate application build identity and archive checksums.

Each archive contains its complete platform folder: installer, installation guide, registration guidance, licence, privacy notice, third-party notices and applicable supplied source, public certificates and verification helpers. Keep that folder together after extraction. The four original signed folders have not been edited to create these archives.

All platforms require a usable TPM 2.0/vTPM, administrator preparation and a separately configured supported database. Windows requires 64-bit Windows 11 or Windows Server 2022 or later; Linux requires the distribution dependencies and systemd. Choose one database engine: MySQL, PostgreSQL or Microsoft SQL Server. Database servers, model files and missing OS dependencies are not bundled. Consult the platform's `INSTALL.md` for exact requirements and the remaining qualification limits.

See [download verification](VERIFY-DOWNLOADS.md) before installing. Signatures use private, self-signed publisher trust that must be independently approved by your IT administrator. They do not establish public certificate trust or production qualification. This same-version rebuild is not a validated in-place upgrade from an earlier RC1 installation.

## Questions and feedback

Use [Pūnaha contact](https://punaha.com/contact) for product questions. Public GitHub issues may be used for non-sensitive feedback. Include the release tag, operating system, installation stage and a sanitised error description. Never post passwords, private keys, activation/request files, personal information or customer data in a public issue.
