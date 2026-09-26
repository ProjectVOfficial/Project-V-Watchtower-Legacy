# Security Policy

## Project status

Project V // Watchtower is a current Windows reference build that has **not** undergone an independent security audit.

Do not use it as the only protection for highly sensitive, classified, regulated, life-safety, or mission-critical information.

## Reporting a vulnerability

Do not publish exploit details, working proof-of-concept code, private keys, or sensitive logs in a public issue.

Preferred process:

1. Use GitHub private vulnerability reporting or a Security Advisory if enabled.
2. If private reporting is not enabled, open a minimal public issue requesting a private security contact. Do not include exploit details.
3. Include the affected version, operating system, impact, and the smallest safe reproduction description.
4. Allow reasonable time for triage before public disclosure.

No bounty program is promised unless separately announced.

## Security boundaries

### Trusted application components

Core Project V windows and native Tauri commands are trusted application components but remain subject to software defects.

### Plugins

Imported plugins are sandboxed and permission-gated. They should still be reviewed before installation.

### Remote web content

Public websites, communications services, and source pages are untrusted remote content. They should not receive Project V secrets or trusted IPC access.

### Local applications

Programs opened through Launch Deck run as separate Windows processes. Project V does not sandbox those applications.

### Local AI

A local model can produce incorrect, manipulated, or unsafe output. AI text is not evidence, authorization, or an executable instruction.

## Implemented controls

Depending on the enabled feature and runtime:

- Tauri desktop isolation
- Restricted IPC command surface
- Context isolation between trusted and untrusted content
- Operating-system credential vault for supported secrets
- Project Lock
- Sandboxed plugin frames
- Declared plugin permissions and network origins
- Restricted Source Browser and communications windows
- Network modes
- Safe Mode
- Last-known-good configuration
- Protected backups using AES-GCM and PBKDF2-SHA256
- Local blocked-request audit records
- Release checksum support

## Important limitations

The application does not protect against:

- a compromised Windows account or kernel;
- malware with the user's privileges;
- screen capture or keylogging malware;
- stolen unlocked devices;
- malicious firmware;
- compromised provider accounts;
- incorrect or poisoned external data;
- social engineering;
- weak user passphrases;
- unreviewed third-party applications;
- vulnerabilities in WebView2, Tauri, dependencies, or the application;
- traffic outside the application's guarded frontend request paths.

Project Lock is an application privacy control, not full-disk encryption.

Emergency Disconnect primarily blocks new guarded frontend requests. Existing remote windows, streams, or external processes may require separate closure.

## Release integrity

Current public Windows builds are not represented as Authenticode-signed.

Users should:

1. Download only from the official ProjectVOfficial GitHub repository.
2. Verify published checksums when provided.
3. Treat unexpected filename, size, hash, publisher, or repository changes as suspicious.
4. Preserve a known-good offline copy when appropriate.

## Secret handling

Never submit:

- API keys
- passwords
- OAuth tokens
- `.env` files
- updater private keys
- Authenticode certificate private keys
- personal research databases
- private case evidence
- exact sensitive locations
- unredacted diagnostic archives

## Dependency risk

Dependencies should be reviewed and updated deliberately. Automated forced upgrades can introduce breaking changes. Security advisories should be evaluated in the context of whether the affected package and code path are included and reachable in the released desktop application.

## Supported versions

Until a formal support policy is announced, only the newest published Project V // Watchtower release should be considered actively reviewed.
