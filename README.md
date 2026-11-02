# eve-desktop-updates
update for eve

<!-- eve-update-feed -->
## E.V.E desktop beta releases

[Download the current beta installer](https://github.com/gtrongames57/eve-desktop-updates/releases/tag/v2.4.1-beta.11). Install it manually once to enable published-release checking inside E.V.E.

This repository distributes Windows x64 installers, signed release metadata and the update feed. The development source repository remains separate. Normal packaged application code is included in the distributed binary.

Automatic downloads are optional; installing requires native **Install and restart** approval. Existing app data is retained. Docker/Windows Sandbox are not required for this per-user published-release flow. FORGE imported-package installation remains separate. These are beta releases. Release validation records Windows installer/update/recovery tests separately from user device acceptance.

Release signatures use the public authority bundled with the bootstrap app. Public-key fingerprint (SHA-256 SPKI): `ed28dda3d5beb8f72770c154f75bda805fb7f19a1f8d76ceeb2fc751bc177ce3`. Private signing keys and GitHub tokens must never be uploaded here.

<!-- eve-resource-pack -->
## Signed FORGE resource packs

Beta.2 adds signed data-only resource installs and restore, with native Windows account verification. [Download the Welcome resource pack](https://github.com/gtrongames57/eve-desktop-updates/releases/download/v2.4.1-beta.11/EVE-Forge-Welcome-1.0.7.eveforge). Update E.V.E before importing it, then preview and run staging checks before installation. Use the currently signed-in administrator account’s Windows password in the native prompt (not PIN/Hello). Resource packs cannot replace application code. Approved application updates use the separate signed installation flow with fresh native approval.

Beta.7: find and download official resource packs inside FORGE → Import Updates. Optional checks run when FORGE opens; downloads and installation still require consent.

Beta.8: Docker/WSL setup and a fixed built-in Linux isolation self-test are in FORGE Settings. Install Docker Desktop separately. Imported executable packages remain blocked; Linux canary success is not Windows compatibility evidence.

Beta.9: download EVE-Feature-Probe-1.0.0.evetest and use FORGE Settings → Isolated signed feature tests. Review the code-only snapshot before running the fixed Linux backend probe. This never installs the change into live E.V.E; Linux probe success does not establish Windows compatibility. Approved application updates use the separate signed installation flow.

## SHADOW ACCESS — beta.11

Open Settings → FORGE → Settings → Security & Permissions → SHADOW ACCESS. The current Windows administrator can create, expire, rotate, modify, and revoke random access codes for selected private or experimental modes. Codes are masked and stored only as salted password hashes. Unlocks require the code plus native administrator verification, apply only to assigned modes, and expire automatically. Revoking a code invalidates its active sessions.

Private modes are hidden from ordinary navigation and checked by the backend. This is an interface privacy feature with an additional authorization factor; it does not replace secure authentication or approve sensitive operations. Existing desktop, resource, and update approvals remain separate. Recovery and visibility-policy rollback require fresh native administrator verification. The website is unchanged.
