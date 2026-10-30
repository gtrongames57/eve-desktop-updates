E.V.E 2.4.1-beta.10 is the official Windows x64 desktop update on the existing beta channel.

### Included
- Signed FORGE application updates with fresh native Windows approval, protected backup, private restarted-app health verification and automatic rollback on failed startup.
- Independent **EVE Recovery** Start menu entry for interrupted updates.
- Fix for **Install signed app update** remaining disabled after refresh, cancellation or a failed handoff.
- Published release downloads remain optional; installation still requires native **Install and restart** confirmation.

### Install
Close E.V.E, download **EVE-Setup-2.4.1-beta.10-x64.exe**, run it, and reopen E.V.E. The full installer does not need a separate Windows receipt. Existing settings, voices/provider credentials and conversations remain in the user profile. No Python setup, Docker or Windows Sandbox is required for published desktop updates.

For the exact trial version **2.4.1-beta.9.acceptance.3.probe.1**, **EVE-Trial-to-Beta10.zip** provides a smaller alternative. Extract it; in FORGE choose **Install signed app update**, select its `.eveinstall` file, then its `.windows.json` receipt. This path requires fresh native Windows account approval. The receipt expires seven days after signing and cannot be reapplied after reaching beta.10. Other versions should use the full installer.

Future published releases are checked under **FORGE → Settings → Published app updates**. Isolated `.evetest` packages remain testing-only; general arbitrary-code installation is not enabled. Signed resource `.eveforge` packs retain their separate approval flow.

### Validation
614 automated tests and required project checks passed. The real Chromium regression covers the corrected native update control. Native Windows tests cover fresh installation, actual signed-ASAR restart/proof completion, deliberately invalid healthy-startup proof with automatic rollback, exact current-trial-to-official bridge, full NSIS upgrade, unchanged encrypted settings/custom voice/provider readback, normal shutdown and profile-retaining uninstall. Automated account approval is synthetic; actual installations still request the native user confirmation/account approval appropriate to their path.

Release authenticity uses the Ed25519 publisher authority already bundled in E.V.E and verified installer hashes. The installer is not Windows Authenticode-signed. This remains a beta-channel release, not a guarantee that every feature is defect-free.

Installer SHA-256: `3df1ac0326e955f82657cd971166a4b5895b91bc268b49962b8b87ad8ec2c2f6`.

Runtime source checkpoint: `038b088d26e36fdd5fe238431909ee5872cf6626`. Native Windows validation run: 41001039970. The accepted trial’s existing release verifier accepts this installer inventory. No production private signing key entered CI.
