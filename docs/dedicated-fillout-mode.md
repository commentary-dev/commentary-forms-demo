# Dedicated Fillout Mode

Dedicated fillout links are for respondents who only need to answer a form.
They should not see file navigation, review comments, diff controls, or source
editing affordances.

## Source Contract

The source owner edits the contract in the review or owner workflow. The
fillout page only renders the current fillable shape.

<Form src="../forms/dedicated-fillout.form.yml" />

## Reply Modes

An identified link records the authenticated submitter. An anonymous link omits
submitter identity and explains that the result owner can still see the answer
values. Repeat submission settings are explicit per link.

## Result Ownership

Dedicated fillout results are scoped to the fillout owner. They do not become
public just because the source review or demo repository is public.
