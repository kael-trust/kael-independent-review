# KAEL Independent Review Authority

This private repository is the trusted review side for KAEL.

## Trust boundary

**Trusted administrative principal:** `kael-review-owner` / `kael-trust`.

**Untrusted implementation side:** the MK-CLOUDS NAS, `ZoeBoyMK`, Docker on that NAS, the current KAEL repository, `zoeboymk-glitch`, and local `state/reviews` data.

The implementation-side GitHub account must not receive administrative or write access to this repository.

## Current phase

N1 (external administrative boundary) has been created.

Before a production review workflow is added, this repository will measure:

1. GitHub Actions OIDC availability on this private repository;
2. the exact workflow identity claims available for independent attestation;
3. a keyless Sigstore attestation path that does not require a long-lived signing key;
4. the exact verification predicate KAEL may later consume.

No KAEL production deployment or authority is granted by this repository.
