# eve-desktop-updates
update for eve

<!-- eve-update-feed -->
## E.V.E desktop beta releases

[Download the current beta installer](https://github.com/gtrongames57/eve-desktop-updates/releases/tag/v2.4.1-beta.3). Install it manually once to enable published-release checking inside E.V.E.

This repository distributes Windows x64 installers, signed release metadata and the update feed. The development source repository remains separate. Normal packaged application code is included in the distributed binary.

Automatic downloads are optional; installing requires native **Install and restart** approval. Existing app data is retained. Docker/Windows Sandbox are not required for this per-user published-release flow. FORGE imported-package installation remains separate. These are experimental beta releases; real Windows upgrade/restart acceptance is not inferred from automated tests.

Release signatures use the public authority bundled with the bootstrap app. Public-key fingerprint (SHA-256 SPKI): `ed28dda3d5beb8f72770c154f75bda805fb7f19a1f8d76ceeb2fc751bc177ce3`. Private signing keys and GitHub tokens must never be uploaded here.

<!-- eve-resource-pack -->
## Signed FORGE resource packs

Beta.2 adds signed data-only resource installs and restore, with native Windows account verification. [Download the Welcome resource pack](https://github.com/gtrongames57/eve-desktop-updates/releases/download/v2.4.1-beta.3/EVE-Forge-Welcome-1.0.1.eveforge). Update E.V.E before importing it, then preview and run staging checks before installation. Use the currently signed-in administrator account’s Windows password in the native prompt (not PIN/Hello). Application code/script packages remain blocked; native credential entry still needs your device acceptance test.
