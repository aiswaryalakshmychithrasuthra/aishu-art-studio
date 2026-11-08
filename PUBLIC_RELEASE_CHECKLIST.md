# Before publishing binaries or full source

- [ ] Confirm you own or are authorised to publish every embedded photo, signature, drawing, logo and reference portrait.
- [ ] Remove or parameterise account-specific settings, including fixed Instagram usernames.
- [ ] Exclude authentication tokens, credentials, paired-device secrets, `.env`, API keys, local databases, Drive paths, user directories, crash logs and backup ZIPs.
- [ ] Audit build scripts for embedded machine-specific paths.
- [ ] Build each binary on the correct platform and test a clean installation on a separate device.
- [ ] Verify version number, app icon, package identifier and signing key strategy.
- [ ] Never label a debug APK as production-safe; only release a purpose-built artifact after review.
- [ ] On macOS, sign/notarise if distributing to other users; otherwise state clearly when a test app is unsigned.
- [ ] Test sync with backups; verify offline and conflict scenarios before promising 3-device automatic syncing.
- [ ] If public source code is intended, add an appropriate licence *after* deciding which elements may be reused.
- [ ] Add screenshots that do not show personal email, login tokens, file-system usernames, unrelated apps or private data.

## Staging approach

1. Public portfolio showcase (this starter).
2. Private audited source repository for development.
3. Public code / Beta release only after removing sensitive data and checking image rights.
4. Stable binaries only after QA, packaging and signing.
