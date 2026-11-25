# legal-versions

Every version of every estate service's legal documents (terms of service, privacy policy and the documents beside them), exactly as
each service served it. legal.333.eco renders them; this repository is the record.

- `<host>/<document>/<YYYY-MM-DD>-<fingerprint>.md` is one version, byte for byte: the date the document itself states, and the first
  six characters of its SHA-256. A version is never edited. A change is a new file at a new address.
- `index.json` lists every version: its date line, its full SHA-256, the operator the text names (or none yet), and the day it was
  first served at legal.333.eco.
- Every version carries an OpenTimestamps proof beside it (`.md.ots`, to Bitcoin), and `timestamps/manifests/` holds dated manifests
  of every file signed by three timestamp authorities (RFC 3161, one eIDAS-qualified). See [`TIMESTAMPS.md`](./TIMESTAMPS.md).

**What a timestamp shows, and what it does not.** It shows that a text existed by that date. It does not show who published it, that it
was in force, or that a lawyer reviewed it. Versions marked as drafts say so in their own words.

**Rights.** All rights reserved, until a decision is published here. These texts are the terms people agree to; copying them does not
change what they say to the people they bind.

The page you read is at https://legal.333.eco. Check any version yourself with `ots verify` and `./tsa-verify.sh`.
