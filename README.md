# Vendor governance cycle workspace

This repository holds the FY26Q4 vendor risk review artifacts.

## Layout

- `registry/FY26Q4/` - cycle manifest and the persisted export response.
- `reports/` - analyst deliverables, including the cycle risk register.
- `registry-archive` branch - retained full exports.

## Notes

- The quarterly registry export covers all active suppliers. For FY26Q4 the registry
  contains 47 active suppliers.
- The export job writes a single JSON document with one record per supplier, including
  its commercial, security and contact attributes and its full audit narrative.
- When a job response exceeds the reporting pipeline's inline response limit it is
  persisted as a saved response; the cycle manifest records that identifier.
- Ticket titles use the `[PRIORITY]` and `[WATCH]` prefixes so downstream automation can
  group remediation work.
