# Commentary Forms Demo

This branch shows how a GitHub repository can own real Form Contract files while
Commentary renders, validates, stores, exports, and hands off structured
answers.

## What This Demonstrates

- Markdown review documents embedding GitHub-backed Forms.
- Static HTML using `data-commentary-form` and `data-commentary-field`.
- The current native renderer field matrix, including conditional logic,
  computed and hidden fields, pages, review mode, and unsupported placeholders.
- Agent-readable summary metadata for downstream review workflows.
- A custom renderer bridge fixture for Live Preview Reviews.

## Suggested Commentary Routes

```text
/review/github/commentary-dev/commentary-forms-demo/document?branch=demo%2Ffull-power&file=docs%2Flaunch-readiness.md&demo=1
/review/github/commentary-dev/commentary-forms-demo/document?branch=demo%2Ffull-power&file=docs%2Fsecurity-review.md&demo=1
/review/github/commentary-dev/commentary-forms-demo/document?branch=demo%2Ffull-power&file=public%2Fvendor-risk.html&demo=1
```

The `preview/custom-renderer/index.html` page is intended for Live Preview
Review bridge smoke after GitHub Pages is enabled for this repository.

