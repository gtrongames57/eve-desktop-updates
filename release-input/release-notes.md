Fix FORGE credential-buffer reading: handle optional empty domain fields and plain/protected Windows credential formats. This does not bypass password verification, current-account SID matching or administrator checks. Password authentication is attempted only once; credentials are not returned to the renderer or HTTP service.

Native Windows tests now pack and unpack synthetic email-only, MicrosoftAccount-qualified and local-domain credentials in plain and protected formats without attempting account sign-in. 471 regressions, browser install/rollback checks and final native packaged Windows run 40155325042 passed. Real Microsoft-account acceptance on the user’s PC is still pending.

Use Welcome 1.0.3 with beta.5. Generate preview, run staging and attempt installation once. If it fails, report the fixed message rather than repeatedly entering credentials.

Experimental E.V.E Windows x64 release 2.4.1-beta.5.

Close E.V.E and install this bootstrap manually once to enable published-release updates. Future releases require verified publisher metadata and native Install and restart approval. No Docker or Windows Sandbox is needed for published application releases. Signed data-only FORGE resource packs now support Windows account verification, protected revisions and rollback. Executable FORGE packages remain blocked; no isolated code runner is enabled. Keep application data and settings.

This installer is unsigned by Windows Authenticode; release authenticity is checked by the bundled Ed25519 release authority. Real Windows upgrade/restart acceptance remains pending; automated tests are not native installation certification.

Installer SHA-256: 34414f9d505360a476d5f7d285705a862eb7d2272b64f1491890c6930c802a84
