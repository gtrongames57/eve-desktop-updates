FORGE native sign-in diagnostics. This release separates Windows LogonUser password rejection from a successful logon with a different account SID. It also distinguishes credential-buffer format failure, lockout, account restrictions, expired password and unavailable logon service. Only fixed categories leave the native helper; no password, username or raw helper output is returned.

This is diagnostic: Microsoft-account password compatibility remains unresolved until the next native test. It does not add PIN/Hello, bypass administrator/current-account verification, or retry credentials automatically. Stop retrying on rejection or lockout and report the fixed message.

Use the attached Welcome 1.0.2 pack with beta.4. The previous sample packs target their own app release only. 471 tests, resource browser denial/retry/install/read/restore, packaged source checks and Windows packaged validation run 40154815062 passed. Actual human password entry remains unverified.

Experimental E.V.E Windows x64 release 2.4.1-beta.4.

Close E.V.E and install this bootstrap manually once to enable published-release updates. Future releases require verified publisher metadata and native Install and restart approval. No Docker or Windows Sandbox is needed for published application releases. Signed data-only FORGE resource packs now support Windows account verification, protected revisions and rollback. Executable FORGE packages remain blocked; no isolated code runner is enabled. Keep application data and settings.

This installer is unsigned by Windows Authenticode; release authenticity is checked by the bundled Ed25519 release authority. Real Windows upgrade/restart acceptance remains pending; automated tests are not native installation certification.

Installer SHA-256: 7bd961cd11568384e94ab34f12d8f4daffa44cb291719d6da8f784a64b8433e7
