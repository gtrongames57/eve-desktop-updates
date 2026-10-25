FORGE verification diagnostics patch. Failed resource installs now distinguish a rejected current-account sign-in, cancelled verification, a non-administrator account, unavailable native verification, and bounded resource-worker failures. Consent resets after each attempt. This patch helps diagnose failures; it does not claim to fix every Windows/Microsoft account configuration or add PIN/Hello support.

Use the attached Welcome 1.0.1 pack with beta.3; the beta.2 Welcome 1.0.0 pack targets beta.2 only. Generate preview, run resource staging, then choose Verify Windows account and install resources. Enter passwords only in the native Windows prompt.

470 tests, resource browser denial/retry/install/restore, packaged source checks and packaged Windows validation run 40154237923 passed. Actual human password entry remains to be tested on your PC.

Experimental E.V.E Windows x64 release 2.4.1-beta.3.

Close E.V.E and install this bootstrap manually once to enable published-release updates. Future releases require verified publisher metadata and native Install and restart approval. No Docker or Windows Sandbox is needed for published application releases. Signed data-only FORGE resource packs now support Windows account verification, protected revisions and rollback. Executable FORGE packages remain blocked; no isolated code runner is enabled. Keep application data and settings.

This installer is unsigned by Windows Authenticode; release authenticity is checked by the bundled Ed25519 release authority. Real Windows upgrade/restart acceptance remains pending; automated tests are not native installation certification.

Installer SHA-256: f1c7cd4f9567d502a56948619b5768aa9257b28c0a7da9d7b5814fb3de03c7c6
