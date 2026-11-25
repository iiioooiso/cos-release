# CommitOS Desktop Releases

Official release distribution and auto-update channel repository for **CommitOS Desktop** — a personal operating system engineered for deep work, focus enforcement, and behavioral accountability.

> This repository hosts signed desktop installers and update manifests only.  
> Visit [cos.communx.org](https://cos.communx.org) to learn more or manage your account.

---

## Download

- **Latest Stable Release:** [Download from Releases](https://github.com/iiioooiso/cos-release/releases/latest)
- **All Releases (Stable & Beta):** [Browse All Releases](https://github.com/iiioooiso/cos-release/releases)

### Installer Formats (Windows x64)
- `commitOS_<version>_x64-setup.exe` — Standard Windows NSIS installer *(recommended; also used by the built-in auto-updater)*
- `commitOS_<version>_x64_en-US.msi` — Windows MSI enterprise/offline installer

---

## Release Channels

CommitOS supports two in-app update channels (configurable under **Settings → About → Release Channel**):

| Channel | Description | Manifest |
| --- | --- | --- |
| **Stable** | Verified production releases for daily use | [`stable/latest.json`](./stable/latest.json) |
| **Beta** | Early-access pre-releases with upcoming features | [`beta/latest.json`](./beta/latest.json) |

---

## Security & Verification

All in-app updates are cryptographically signed with Ed25519 (`.sig` assets) and verified automatically by the CommitOS desktop updater before installation. Updates are deferred while an active Focus or Critical mission is running.
