# ECI Verification Registry

This repository is the public verification registry for selected ECI (Enterprise Conversation Infrastructure) documents.

It provides cryptographic hashes for released PDF documents so recipients can verify authenticity and detect tampering.

## Owner

ECI and all associated intellectual property is owned by Erik Andersen.

## What this repository is

- A public, read-only integrity verification register.
- A place where released document hashes are published with version identifiers.

## What this repository is not

- It does not distribute the underlying confidential PDFs.
- It does not grant any licence to use, reproduce, or implement ECI architecture.

## How to verify a document

See VERIFYING.md.

## Registry structure

- `versions/` contains active document hash entries.
- `superseded/` contains hash entries for superseded versions.

## Policy

- Hash entries are append-only in practice (new versions are added, old versions remain visible).
- Releases are versioned.
- Any change to a document requires a new version and a new hash.
