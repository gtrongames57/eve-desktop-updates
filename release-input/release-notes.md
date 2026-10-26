Signed isolated backend testing stage. FORGE → Settings → Isolated signed feature tests can verify the attached testing-only .evetest package, review its code-only snapshot and run it in restricted Docker. Docker Desktop's Linux/WSL 2 engine must be running. No live feature installation occurs.

Try EVE-Feature-Probe-1.0.0.evetest after updating to beta.9: native picker verification → Review isolated snapshot → Run isolated backend tests. Expected: passed, nine checks true, cleanup completed, Windows compatibility not-tested, executable installation false. The feature exists only in the Docker copy.

The fixed reporter runs as a different user from the proposed app. Results bind the exact package, copied baseline, app version and derived image. Production settings, environment files, memories and provider credentials are excluded. Source drift, tampering, wrong reporter identity, false app logs and failed cleanup cannot enable installation. Docker may retain code-only build cache.

499 tests, six browser suites, real positive/negative Docker feature runs, baseline-preservation/recovery, native Windows app.asar import/review and three independent platform jobs passed. Windows-native feature compatibility and executable writer/backup/restart/rollback remain separate unfinished gates. Source ZIP includes docs/forge/SIGNED_BACKEND_TESTS.md.

Experimental E.V.E Windows x64 release 2.4.1-beta.9.

Close E.V.E and install this bootstrap manually once to enable published-release updates. Future releases require verified publisher metadata and native Install and restart approval. No Docker or Windows Sandbox is needed for published application releases. Signed data-only FORGE resource packs now support Windows account verification, protected revisions and rollback. Executable FORGE packages remain blocked; no isolated code runner is enabled. Keep application data and settings.

This installer is unsigned by Windows Authenticode; release authenticity is checked by the bundled Ed25519 release authority. Real Windows upgrade/restart acceptance remains pending; automated tests are not native installation certification.

Installer SHA-256: ec201067aa1c636a036d83564f1aabc4065629b693f03fd86ee65679dd048f0b
