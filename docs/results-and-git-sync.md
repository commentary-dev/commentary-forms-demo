# Forms Results And Git Sync

This sample shows how Forms results move between review-time submissions,
workspace result collections, and canonical git result files.

## Result Collections

Commentary groups submissions by source context. Git-backed review forms use PR
or branch ownership hints. Draft Review forms default to the draft owner.
Dedicated fillout links default to the fillout owner.

<Form src="../forms/results-sync.form.json" />

## Canonical Git Result Files

The demo branch includes canonical result documents under
`forms/results/launch-readiness/`. These files contain the form reference,
contract hash, submission metadata, submitter mode, validation diagnostics, and
source context needed for deterministic import.

## Writeback Availability

Writeback is optional and requires the separate GitHub Writeback App. Public
demo and stable fixture repositories are read-only samples; mutating tests must
target `commentary-dev/commentary-forms-mutable-e2e`.

## Diagnostics

The malformed result fixture intentionally omits required metadata. Local
preflight should flag it as malformed without treating the public repository as
a write target.
