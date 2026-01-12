# Verifying an ECI Document

This repository publishes cryptographic hash values for released ECI documents.

If you receive an ECI PDF, you can verify it by comparing your computed hash against the hash published here.

## Step 1 — Identify the hash entry

Open the relevant file in `versions/` (or `superseded/` for older versions).
Example: `versions/ECI-Architecture-Certification-Governance-v1.0_SHA256.txt`

## Step 2 — Compute the file hash

### Windows (PowerShell)
Run:
Get-FileHash "ECI - Architecture, Certification and Governance brief v1.0.pdf" -Algorithm SHA256

### macOS / Linux
Run:
sha256sum "ECI - Architecture, Certification and Governance brief v1.0.pdf"

## Step 3 — Compare

Compare the computed hash output to the HASH value in the registry entry.

- Match = verified and untampered.
- Mismatch = do not rely on the document.

## Notes

- Even a single character change produces a completely different hash.
- Publication date equals the GitHub commit date.


