# Contribution Plan

Account: `chrisx9z`

## First profile step

Create a public repository named exactly `chrisx9z`, then add `README.md` from this folder. GitHub will show it on the profile page.

Recommended commit message:

```text
Add profile README
```

Short commit comment:

```text
Creates a concise profile README so visitors can quickly understand my focus, contribution style, and current goals.
```

## Weekly contribution loop

1. Pick one small issue with `good first issue`, `help wanted`, or `documentation`.
2. Read `README.md`, `CONTRIBUTING.md`, open issues, and recent PRs.
3. Comment only when useful: state the exact fix you plan to make.
4. Make the smallest correct change.
5. Open a PR with:
   - problem summary
   - implementation summary
   - test or verification steps
   - linked issue

## Good first contribution filters

Use these GitHub searches:

```text
is:issue is:open label:"good first issue" label:documentation
is:issue is:open label:"help wanted" label:documentation
is:issue is:open "typo" "README"
is:issue is:open "broken link" "documentation"
```

Issue discovery tools:

- https://github.com/topics/good-first-issue
- https://goodfirstissues.com/
- https://www.goodfirstissue.org/
- https://goodfirstissue.dev/
- https://kanywst.github.io/IssueHub/

Prefer repositories that have:

- recent commits in the last 30 days
- a clear `CONTRIBUTING.md`
- active maintainer replies
- passing CI on recent PRs

Avoid for now:

- stale issues with no maintainer response
- issues requiring broad architecture changes
- drive-by typo PRs without checking project rules

## PR template

```markdown
## Summary

Fixes/Improves ...

## What changed

- ...

## Verification

- [ ] Read the relevant contribution guide
- [ ] Ran ...
- [ ] Checked ...

Closes #
```

## Commit comment rule

Add one short comment for each commit. Keep it factual and specific:

```text
This commit ...
```

Good examples:

```text
This commit documents the expected setup flow so new contributors can get started without guessing.
This commit fixes the broken README link and verifies the target page still exists.
This commit adds a focused regression test for the behavior described in the issue.
```

Avoid vague comments:

```text
Updated files.
Small fix.
Changes.
```

## Issue comment template

```markdown
I can take this. I plan to keep the change scoped to ...

Before opening a PR, I will verify ...
```
