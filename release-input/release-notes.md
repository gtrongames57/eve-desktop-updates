Docker/WSL isolation setup stage. FORGE → Settings → Docker isolation self-test now provides consent-bound local engine detection, pinned official image download, fixed built-in Linux canary, Stop and interrupted-canary cleanup. Install Docker Desktop with its WSL 2 backend on your Windows PC separately, then leave its Linux engine running.

The canary has no host folders or E.V.E credentials, no network, a non-root user, read-only root, dropped capabilities, no-new-privileges, private IPC/cgroup namespace, and CPU/memory/swap/PID limits checked inside the container. Normal/failure cleanup, foreign-label protection and fresh-host recovery are tested. This stage runs only the built-in script; executable packages and installation remain blocked. Linux does not certify Windows native compatibility.

484 automated tests, five browser suites, real Docker tests, independent Linux run 40397460601 and packaged Windows run 40397460373 passed on source checkpoint 26ad2df. User-PC Docker Desktop named-pipe/self-test acceptance remains pending. The source ZIP includes docs/forge/DOCKER_ISOLATION_SETUP.md.

Experimental E.V.E Windows x64 release 2.4.1-beta.8.

Close E.V.E and install this bootstrap manually once to enable published-release updates. Future releases require verified publisher metadata and native Install and restart approval. No Docker or Windows Sandbox is needed for published application releases. Signed data-only FORGE resource packs now support Windows account verification, protected revisions and rollback. Executable FORGE packages remain blocked; no isolated code runner is enabled. Keep application data and settings.

This installer is unsigned by Windows Authenticode; release authenticity is checked by the bundled Ed25519 release authority. Real Windows upgrade/restart acceptance remains pending; automated tests are not native installation certification.

Installer SHA-256: baf0e02290c9c033e29a8350032541ee9378435a5d041c8d9a2ee11ecb2bd2cb
