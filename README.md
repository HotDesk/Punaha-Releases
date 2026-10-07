# Pūnaha downloads

Official release information and installation downloads from Hot Desk Consultancy Services Limited.

**[Pūnaha 0.1 RC1 downloads](https://github.com/HotDesk/Punaha-Releases/releases/tag/v0.1.0-rc.1-terms-v2)** are available for invited evaluation. The current packages were rebuilt on **7 October 2026** (`browser-20261007`); the embedded application version remains **0.1.0-rc.1**. The browser JavaScript is now minified with internal identifier mangling and no source maps. Full installation and production acceptance remain outstanding.

This repository holds release documentation. The proprietary application source is maintained separately. GitHub's automatically generated **Source code** ZIP and tar.gz contain this repository's documents, not an installer or the application source.

## Current software offer

Pūnaha is one full proprietary product. The current issued **12-month licence term costs US$0**, starting on the signed activation's stated issue date. Personal and organisational use, multiple versions and independently registered installations are permitted, subject to technical compatibility and registration. Optional paid support is separate.

Future renewal pricing is undecided and may include a charge based on demand for additional functionality and the actual cost of maintaining and developing the software. Any proposed price and terms will be disclosed in advance. Paid renewal requires explicit acceptance; there is no automatic charge or obligation to renew. Existing issued terms and previously accepted commitments are honoured.

Read the complete [software licence](PUNAHA-LICENCE.md) and [privacy notice](PRIVACY.md). Availability on GitHub does not grant an open-source licence to the proprietary application. Third-party components retain their own terms, notices and applicable supplied source in each complete download.

## Registration and expiry

**There is currently no facility to register a Pūnaha installation in RC1. Registration will be available in the first production version.** Export before the allowance ends; registration cannot currently restore normal use in RC1. Downloading or installing this candidate does not issue a 12-month activation.

**Renew or export your data before the access cutoff.** A new installation after setup, and each expired registered term, has a **720 TPM powered-on-hour allowance**. This is not 30 calendar days, and includes time the TPM is powered on while the Product service is stopped.

After the allowance ends, ordinary processing, administration, customer-data access and exports stop. Data is retained, but Product access and export remain unavailable until valid registration or renewal is restored. Only necessary sign-in, registration, renewal, activation and recovery functions remain available. Online and offline activation both require the completed registration process; submitting a request alone is insufficient.

## Current RC1 downloads

Get the complete signed Windows, Ubuntu, Debian 13 or RHEL 9 package from the [RC1 release page](https://github.com/HotDesk/Punaha-Releases/releases/tag/v0.1.0-rc.1-terms-v2). Select the files with `browser-20261007` in their names and use `SHA256SUMS-browser-20261007.txt`.

The public tag identifies release documentation; [RELEASE-INFO.json](RELEASE-INFO.json) records the separate private application source identity and exact archive hashes. GitHub’s automatic Source code archives are not application installers.

Each archive contains its installer, installation guide, registration availability notice, licence, privacy notice, third-party notices and applicable source, public certificates and verification helpers. Every delivered file is covered by a signed manifest; installers, executables, download archives and checksum lists also have the signatures described in the verification guide.

The Windows MSI includes the runtime permissions correction. The older repair2 bundle is not needed for this rebuild and must not be applied to it. The default program folder is `Program Files\Punaha`; the display name remains Pūnaha. Intel SYCL requires an ASCII-only Local runtime path. Use a fresh, separate evaluation installation; same-version Windows upgrades are blocked.

All platforms require a usable TPM 2.0/vTPM, administrator preparation and a separately configured supported database. Windows requires 64-bit Windows 11 or Windows Server 2022 or later; Linux requires the distribution dependencies and systemd. Choose one database engine: MySQL, PostgreSQL or Microsoft SQL Server. Database servers, model files and missing OS dependencies are not bundled. Consult the platform's `INSTALL.md` for exact requirements and the remaining qualification limits.

See [download verification](VERIFY-DOWNLOADS.md) before installing. Signatures use private, self-signed publisher trust that must be independently approved by your IT administrator. They do not establish public certificate trust or production qualification. This same-version rebuild is not a validated in-place upgrade from an earlier RC1 installation.

## Questions and feedback

Use [Pūnaha contact](https://punaha.com/contact) for product questions. Public GitHub issues may be used for non-sensitive feedback. Include the release tag, operating system, installation stage and a sanitised error description. Never post passwords, private keys, activation/request files, personal information or customer data in a public issue.
