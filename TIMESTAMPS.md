# Cryptographic timestamps

This repository exists so that each version of each service's legal documents can be shown to have existed when it did. Three
independent dates back that up:

1. **The push.** GitHub records when each commit reached this public repository.
2. **OpenTimestamps.** Each version carries a `<id>.md.ots` proof beside it, which commits the file's SHA-256 to the Bitcoin
   blockchain. Anyone can check it without trusting this repository, GitHub or the authors.
3. **RFC 3161.** A manifest of every tracked file is signed by three independent trust authorities, one of them eIDAS-qualified,
   at each release and weekly. See [`timestamps/README.md`](./timestamps/README.md).

## One version, one file, one proof

A new version is a new file at a new address, so a proof here is never overwritten and never rotated. The weekly job adds a proof to
any version that has none and upgrades pending proofs once Bitcoin confirms them.

## What a proof does not show

That anyone published the text, that it was in force, or that a lawyer reviewed it. A proof shows existence by a date, nothing more.

## Releases

### 2026-11-25 — the first four versions

earth.333.eco terms and privacy policy (Draft of 9 November 2026) · developers.333.eco developer terms and privacy policy (Draft of 25
November 2026). Earlier drafts of each were served at the service's own address before this record began.
