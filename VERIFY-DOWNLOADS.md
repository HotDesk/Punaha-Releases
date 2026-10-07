# Verify a Pūnaha download

Use these instructions for the RC1 `browser-20261007` downloads from the official release page. These are evaluation packages; signature verification does not establish production acceptance.

## 1. Select the complete platform archive

Obtain the appropriate named installer archive and `SHA256SUMS-browser-20261007.txt` from the same official release in `HotDesk/Punaha-Releases`. Do not select GitHub's automatic **Source code** archives: they contain release documentation only.

On Windows, calculate the ZIP hash:

```powershell
Get-FileHash -LiteralPath .\punaha-0.1.0-rc.1-browser-20261007-windows-amd64.zip -Algorithm SHA256
```

Compare every hexadecimal character with the matching line in `SHA256SUMS-browser-20261007.txt`. On Linux, from the directory containing the selected archive and checksums, use:

```bash
sha256sum --check --ignore-missing SHA256SUMS-browser-20261007.txt
```

Confirm that your downloaded archive is listed as `OK`. Files for other platforms may be absent. A checksum mismatch means that the download must not be installed.

The archives, checksum list and release-details JSON each have a matching `.sig` asset signed with the release certificate. Independently approve the certificate fingerprint below before relying on it. On Linux, use trusted OpenSSL tools to verify a downloaded file (substitute its exact name for FILE):

```bash
openssl x509 -inform DER -in punaha-release-signing.cer -pubkey -noout > release-public.pem
openssl dgst -sha256 -verify release-public.pem -signature FILE.sig FILE
```

Check the DER certificate hash before extracting its public key. Continue with the exact signed inner inventory after extracting the archive.

## 2. Extract without modifying the platform folder

Extract the archive using the operating system's archive tool. Each has one platform folder: `Windows`, `Ubuntu`, `Debian13` or `RHEL9`. Keep its original files and subdirectories together. Do not add the outer checksum file or these repository documents inside it: the bundle verifier checks an exact signed inventory.

## 3. Establish publisher trust and verify the signed inventory

Before using a supplied helper, IT must independently approve the expected certificate fingerprints through an established vendor/onboarding channel. The values below are SHA-256 hashes over the DER `.cer` bytes. A value downloaded beside an installer is a reference, not independent evidence of trust.

| Purpose | SHA-256 certificate fingerprint |
|---|---|
| Windows publisher | `11a90675305b50a3bdca95ab8f86a821658d527d21903d81e30c873c67291275` |
| Release manifests | `7f76f8e1af2fed2a5098f3f78443be95b77d4b39d1d84cbd70cd84ba29cb84b5` |

Read the extracted platform's `INSTALL.md` for its trust preparation, verification commands and installation procedure. The manifest uses RSA-SHA256 and covers every other bundle file except its detached signature. The Windows installer is also Authenticode signed and timestamped. The Linux DEB/RPM and standalone executables also have detached RSA-SHA256 signatures. The RPM has no native OpenPGP signature; detached RSA signatures do not replace an organisation's RPM repository-signing policy.

Do not bypass operating-system, certificate or endpoint security policies to run a candidate. Certificate enrolment is a persistent administrative change and requires the organisation's approved process. The supplied certificates expire in September 2028; future verification requires current approved material and applicable timestamp/trust checks.

## 4. Read the terms and installation requirements

Read `PUNAHA-LICENCE.md`, `PRIVACY.md`, `THIRD_PARTY_NOTICES.md`, `REGISTRATION.md` and `RELEASE-CANDIDATE.md`. Prepare the required database, TPM and operating-system dependencies before first-time setup. The bundled candidate documents identify acceptance work still outstanding; integrity verification does not establish application correctness, production readiness or third-party redistribution permission.
