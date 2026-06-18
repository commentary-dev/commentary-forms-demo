# Git-Backed Review Forms

This sample shows Forms source ownership in a normal GitHub PR. The repository
contains standalone `.form.yaml`, `.form.yml`, and `.form.json` contracts. The
review document decides where a form appears, but the source file remains the
contract of record.

## Standalone Contracts

- `forms/full-capability.form.yaml` demonstrates the broad native field matrix.
- `forms/dedicated-fillout.form.yml` is a source contract for fill-only links.
- `forms/results-sync.form.json` is the JSON contract used by result sync.

## Markdown Embed

The release checklist embeds the full capability contract directly in rendered
Markdown. Reviewers can still comment on the surrounding prose and use Raw or
Diff mode when exact source matters.

<Form src="../forms/full-capability.form.yaml" />

## HTML Binding

The vendor risk page binds static HTML controls with `data-commentary-field`.
Commentary validates those values against the repo-backed contract and ignores
unsafe scripts, inline handlers, and external form actions.

## Safe MDX Layout

The companion MDX sample keeps rich layout as review content. It can place a
Forms block inside editorial structure, but executable behavior still comes
from the machine-readable Form Contract.
