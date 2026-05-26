# Open Source Log

This log tracks real contribution work: issues reviewed, pull requests opened, and lessons learned.

## 2026-05

### Profile setup

- Created a public GitHub profile repository.
- Added a concise profile README.
- Added a repeatable contribution workflow.
- Added commit comment examples.
- Added issue and pull request templates.

### Next contribution targets

- Find one documentation issue with a clear owner response.
- Reproduce or verify the issue before commenting.
- Open one small PR with a focused summary and verification notes.

### 2026-05-26 - chaoss/CollectOSS

- Issue/PR: https://github.com/chaoss/CollectOSS/issues/340 and https://github.com/chaoss/CollectOSS/pull/341
- Change: Replaced old CollectOSS Read the Docs host references with `docs.collectoss.org`.
- Verification: Confirmed `collectoss.readthedocs.io` no longer appears in the repository and checked the new docs pages return HTTP 200.
- Result: Pull request opened against `chaoss/CollectOSS`.
- Lesson: A small documentation PR is stronger when it also checks that replacement links are live.

### 2026-05-26 - kingkyylian/linwarden

- Issue/PR: https://github.com/kingkyylian/linwarden/issues/49 and https://github.com/kingkyylian/linwarden/pull/50
- Change: Added a maintainer checklist for public repository metadata and linked it from launch guidance.
- Verification: Ran `tests.test_action_metadata` and `python -m compileall -q src tests scripts`.
- Result: Pull request opened against `kingkyylian/linwarden`.
- Lesson: Documentation tasks with explicit acceptance criteria are good second contributions because verification can stay concrete.

## Entry template

```markdown
### YYYY-MM-DD - Repository

- Issue/PR:
- Change:
- Verification:
- Result:
- Lesson:
```
