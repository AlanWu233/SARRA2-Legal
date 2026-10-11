# SARRA2 Legal

This public, documents-only repository contains verified English SARRA2 legal
documents and their versioned manifest. The default branch is `main`.

## Files

- `legal/privacy.md`: Privacy Policy.
- `legal/terms.md`: Terms of Use.
- `legal/disclaimer.md`: Disclaimer.
- `config.json`: Legal-document manifest.

The current manifest publishes privacy version 2, terms version 1, and disclaimer
version 1 with `silent` update behavior. Its publication and effective timestamps
are October 11, 2026 (UTC). The prepared documents retain their verified bytes,
including the terms document's September 15, 2026 last-updated date.

## Manifest Schema

`config.json` is UTF-8 JSON with the following top-level fields:

| Field | Meaning |
| --- | --- |
| `schemaVersion` | Integer schema version, currently `1`. |
| `manifestVersion` | Positive integer incremented for each manifest publication. |
| `language` | Document language, currently `en`. |
| `documents` | Array containing `privacy`, `terms`, and `disclaimer`. |

Each document entry contains:

| Field | Meaning |
| --- | --- |
| `id` | Stable document identifier: `privacy`, `terms`, or `disclaimer`. |
| `version` | Positive integer incremented whenever that document changes. |
| `updatedAt` | Publication timestamp in ISO 8601 UTC format. |
| `effectiveAt` | Effective timestamp in ISO 8601 UTC format. |
| `sha256` | Lowercase SHA-256 digest of the exact UTF-8 Markdown file bytes. |
| `url` | Direct HTTPS raw-file URL pinned to the full 40-character document commit. |
| `updateBehavior` | Explicit value: `silent`, `notificationRequired`, or `consentRequired`. |

## Publication Process

1. Prepare and verify the English Markdown documents. Keep the approved bytes
   consistent with the bundled application documents, with no placeholders.
2. Commit and push changed documents first. Record the full 40-character commit.
3. Increment each changed document's `version` and the `manifestVersion`. Update
   its timestamps, compute SHA-256 from its exact bytes, and pin its URL to the
   pushed document commit. Unchanged entries can retain their existing pinned URLs.
4. Select update behavior explicitly. Minor editorial changes may use `silent`.
   Material changes must use `notificationRequired` or `consentRequired`, according
   to the approved notice or consent requirement.
5. Commit and push the manifest last, after all referenced documents are available.
6. Download the manifest and documents without authentication. Verify direct HTTPS
   responses, exact file bytes, and all declared SHA-256 hashes.

Never place tokens, credentials, private application source, or deployment
configuration in this repository or its documents. Publication here does not
deploy a Worker or enable application operational configuration. Private
application source remains unchanged by this repository's publication process.
