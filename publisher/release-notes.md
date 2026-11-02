E.V.E 2.4.1-beta.11 adds SHADOW ACCESS to the existing FORGE Security & Permissions panel.

- Masked purple holographic code entry and explicit unlock/relock states.
- Administrator-verified creation, permission changes, expiration, rotation, revocation, and recovery.
- Public/private/experimental mode visibility enforced by the backend, with scoped expiring unlock sessions.
- Salted Argon2id hashes with a memory-hard scrypt fallback for desktop runtimes that do not provide Argon2id; no plaintext-code storage or master bypass.
- Persisted attempt limits, sanitized access history, native administrator verification, and visibility-policy rollback. Mode access does not approve sensitive desktop or update operations.

Install using EVE-Setup-2.4.1-beta.11-x64.exe, or check published app updates in the installed desktop app and review Install and restart. Close E.V.E before a manual installation. Keep your previous installer for rollback. Existing Fish Audio configuration, voice/provider settings, memory files, and integrations remain in your user profile.

After installation, open Settings → FORGE → Settings → Security & Permissions → SHADOW ACCESS. Choose Verify administrator & manage access, configure a mode's visibility, and create a code for its explicit mode permissions. A valid code also requires native administrator verification. Codes do not grant administrator privilege or replace other approval checks.

Validation includes 626 automated tests, browser unlock/relock checks, Windows Electron encrypted-registry persistence across launches, packaged-app permission checks, and real Windows installer/update/recovery acceptance. Automated Windows approvals are synthetic fixtures; the preceding SHADOW ACCESS review build was accepted by the user on Windows.

This is an official release on E.V.E's existing beta desktop channel. The website has not been updated. Windows Authenticode signing is not provided; E.V.E checks publisher-signed release metadata.

Installer SHA-256: febc7fff233c83a8a4b21f3b2d9ea8849b8243022234daec18af5b841ab9378f
