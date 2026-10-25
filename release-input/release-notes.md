Fix FORGE administrator-account detection in filtered Windows tokens. Account membership now inspects native TokenGroups and recognizes the built-in Administrators SID when enabled or deny-only. Password verification and matching the current account SID remain required. This is not an enabled-access check or elevation; no impersonation, group changes or automatic authentication retry is performed.

Native tests create a real restricted Windows token, verify deny-only access is rejected while membership remains detectable, and reject an absent SID. 471 regressions, browser resource install/rollback and packaged Windows run 40155795867 passed. Actual final install on the user’s PC still needs validation.

Use Welcome 1.0.4 with beta.6. Generate preview, run staging and attempt installation once. Report the fixed message if it fails.

Experimental E.V.E Windows x64 release 2.4.1-beta.6.

Close E.V.E and install this bootstrap manually once to enable published-release updates. Future releases require verified publisher metadata and native Install and restart approval. No Docker or Windows Sandbox is needed for published application releases. Signed data-only FORGE resource packs now support Windows account verification, protected revisions and rollback. Executable FORGE packages remain blocked; no isolated code runner is enabled. Keep application data and settings.

This installer is unsigned by Windows Authenticode; release authenticity is checked by the bundled Ed25519 release authority. Real Windows upgrade/restart acceptance remains pending; automated tests are not native installation certification.

Installer SHA-256: 388a243b7e3da43a2c5d22ea9cf3d853787f75d75661505a7d4ecf55c70be94b
