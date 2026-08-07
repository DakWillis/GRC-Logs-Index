# Contributing

## What this repository accepts

- Framework mapping corrections, citing the control and the framework version
- Additional failure modes for an existing control area, drawn from real practice
- Crosswalk additions for frameworks not yet covered — NIST SP 800-53 Rev 5, PCI DSS, HIPAA Security Rule
- Structural improvements to the index generator or the domain grouping
- Corrections to the numbering conflicts documented in `docs/PROVENANCE.md`

## What this repository does not accept

- Entries claiming to document posts that were not published
- Real organizational data of any kind, however anonymized it appears
- Control text copied from a published standard
- Theory without an execution or evidence dimension
- Framework summaries available in the standard itself

## How to contribute

1. Fork the repository
2. Branch: `fix/<control-or-day>` or `feat/<short-description>`
3. Edit the `DAYS` data in `build_index.py` rather than the generated markdown — `INDEX.md`, `domains/`, and `frameworks/CROSSWALK.md` are all generated output and edits there will be overwritten
4. Re-run `python3 build_index.py` and commit both the data change and the regenerated files
5. Open a PR stating what changed, which entries it affects, and what source confirms it

## On verification status

Do not promote an entry from `partial` to `verified` unless the complete field set has been confirmed against the published post. The status field is the integrity control for this entire repository — an entry marked verified is a claim that nothing in it was inferred.
