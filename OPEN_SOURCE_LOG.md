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

### 2026-05-26 - kingkyylian/linwarden

- Issue/PR: https://github.com/kingkyylian/linwarden/issues/51 and https://github.com/kingkyylian/linwarden/pull/52
- Change: Added a contributor issue curation checklist and linked it from contributor ideas.
- Verification: Ran `tests.test_action_metadata` and `python -m compileall -q src tests scripts`.
- Result: Pull request opened against `kingkyylian/linwarden`.
- Lesson: Contributor-facing docs should make scope, labels, acceptance criteria, and verification explicit.

### 2026-05-26 - kingkyylian/linwarden

- Issue/PR: https://github.com/kingkyylian/linwarden/issues/35 and https://github.com/kingkyylian/linwarden/pull/54
- Change: Moved the security reporting link into the README Security Model section.
- Verification: Ran `tests.test_action_metadata` and `python -m compileall -q src tests scripts`.
- Result: Pull request opened against `kingkyylian/linwarden`.
- Lesson: Small documentation changes are more useful when they place guidance exactly where readers need it.

### 2026-05-26 - edehvictor/StellarYield

- Issue/PR: https://github.com/edehvictor/StellarYield/issues/466 and https://github.com/edehvictor/StellarYield/pull/483
- Change: Documented backend rate-limited endpoints, expected `429` behavior, and frontend retry guidance.
- Verification: Confirmed limiter source references and documented endpoint limits with `rg`.
- Result: Pull request opened against `edehvictor/StellarYield`.
- Lesson: Crypto/Web3 docs contributions should tie guidance back to concrete route and middleware source files.

### 2026-05-26 - stellar/awesome-stellar

- Issue/PR: https://github.com/stellar/awesome-stellar/issues/30 and https://github.com/stellar/awesome-stellar/pull/36
- Change: Replaced a stale OMFIF CBDC resource URL with the current report page.
- Verification: Confirmed the new OMFIF report URL returns HTTP 200 and the old HTTPS thinktank URL returns 404.
- Result: Pull request opened against `stellar/awesome-stellar`.
- Lesson: Link fixes are strongest when they preserve the original resource intent and verify the replacement URL.

### 2026-05-26 - FuelLabs/fuels-rs

- Issue/PR: https://github.com/FuelLabs/fuels-rs/issues/1320 and https://github.com/FuelLabs/fuels-rs/pull/1712
- Change: Added a `U256` docs page and linked it from the Types section.
- Verification: Ran `git diff --check`, confirmed the docs link target exists, and checked the referenced `U256` APIs in source.
- Result: Pull request opened against `FuelLabs/fuels-rs`.
- Lesson: A concise type docs page should cover mapping, construction, generated-binding usage, and serialization behavior.

## Entry template

```markdown
### YYYY-MM-DD - Repository

- Issue/PR:
- Change:
- Verification:
- Result:
- Lesson:
```
