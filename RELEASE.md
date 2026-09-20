# Release repository policy

This repository is intentionally limited to public release artifacts.

## Publish a release

1. Build and sign the APKs in the private source repository.
2. Verify each APK with `apksigner verify --verbose`.
3. Generate `SHA256SUMS.txt` from the final files.
4. Create a GitHub Release and upload only the signed APKs, optional AAB, and checksum file.
5. Update the release notes and confirm that the product website reads the new release.

Do not commit Flutter source, backend code, Firebase configuration, API keys, signing keys, `key.properties`, or build output to this repository.
