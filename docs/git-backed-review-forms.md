# Launch readiness: structured review answers

## The decision

Can this fictional pilot launch? Read the plan, identify the launch owner and customer segment, and inspect the readiness questions below. Use comments for questions about the plan and the form for structured answers. A submitted checklist does not automatically approve or deploy a release.

## Readiness answers

Name the release and its owner, choose the intended audience, and assess rollout
confidence. Explain any blocking risk before recording your recommendation.
Reviewers can comment on the surrounding prose and inspect Changes while keeping
Preview selected. Form answers are evidence for the launch decision, not a human
approval receipt.

<Form src="../forms/full-capability.form.yaml" />

## How this example is built

This sample shows Forms source ownership in a normal GitHub PR. The repository
contains standalone `.form.yaml`, `.form.yml`, and `.form.json` contracts. The
review document decides where a form appears, but the source file remains the
contract of record.

- `forms/full-capability.form.yaml` demonstrates the broad native field matrix.
- `forms/dedicated-fillout.form.yml` is a source contract for fill-only links.
- `forms/results-sync.form.json` is the JSON contract used by result sync.

## HTML Binding

The vendor risk page binds static HTML controls with `data-commentary-field`.
Commentary validates those values against the repo-backed contract and ignores
unsafe scripts, inline handlers, and external form actions.

## Safe MDX Layout

The companion MDX sample keeps rich layout as review content. It can place a
Forms block inside editorial structure, but executable behavior still comes
from the machine-readable Form Contract.
