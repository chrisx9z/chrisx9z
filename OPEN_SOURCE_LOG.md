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

### 2026-05-26 - linera-io/linera-documentation

- Issue/PR: https://github.com/linera-io/linera-documentation/issues/258 and https://github.com/linera-io/linera-documentation/pull/259
- Change: Documented source-link checks for generated Linera documentation edit URLs.
- Verification: Ran `git diff --check` and confirmed the README includes the expected edit URL example.
- Result: Pull request opened against `linera-io/linera-documentation`.
- Lesson: Documentation deployment repos benefit from explicit source-path checks that prevent contributor-facing links from drifting.

### 2026-05-26 - stellar/js-stellar-base

- Issue/PR: https://github.com/stellar/js-stellar-sdk/issues/584 and https://github.com/stellar/js-stellar-base/pull/967
- Change: Added `getClaimableBalanceIdFromResult` to extract create-claimable-balance IDs from successful transaction result XDRs.
- Verification: Ran `git diff --check`, `node --check src/get_claimable_balance_id.js`, and `node --check test/unit/get_claimable_balance_id_test.js`.
- Result: Pull request opened against `stellar/js-stellar-base`.
- Follow-up: Addressed review feedback by clarifying optional index docs, improving index errors, and covering non-success results.
- Lesson: SDK helpers should accept the object developers already receive after submission while keeping error cases explicit.

### 2026-05-27 - stellar/stellar-etl

- Issue/PR: https://github.com/stellar/stellar-etl/issues/327 and https://github.com/stellar/stellar-etl/pull/428
- Change: Updated JSON-line export filenames and command docs from `.txt` to `.json`.
- Verification: Ran `git diff --check` and confirmed remaining `.txt` references are for the non-JSON ledger range command or tests.
- Result: Pull request opened against `stellar/stellar-etl`.
- Follow-up: Addressed review feedback by documenting that `.json` exports are newline-delimited JSON rows.
- Lesson: File extensions should reflect the payload format so downstream pipelines and users can infer content correctly.

### 2026-05-27 - wevm/zile

- Issue/PR: https://github.com/wevm/zile/issues/46 and https://github.com/wevm/zile/pull/47
- Change: Lazy-loaded the examples command module so `zile new` does not require `typescript`.
- Verification: Ran `git diff --check` and confirmed only `build --check-examples` and `examples:check` import the examples module.
- Result: Pull request opened against `wevm/zile`.
- Lesson: CLI entrypoints should avoid loading optional command dependencies before argument parsing.

### 2026-05-27 - wevm/prool

- Issue/PR: https://github.com/wevm/prool/issues/34 and https://github.com/wevm/prool/pull/78
- Change: Migrated the internal process wrapper from `execa` to `tinyexec` while preserving the tagged-template start callback API.
- Verification: Ran `pnpm install --lockfile-only`, `pnpm install --ignore-scripts`, `pnpm exec tsc --noEmit`, `pnpm exec biome check src/processes/execa.ts package.json .changeset/yellow-rockets-jam.md`, and `git diff --check`.
- Result: Pull request opened against `wevm/prool`.
- Lesson: Dependency-reduction PRs should preserve public callback shape and include compatibility notes for command tokenization.

### 2026-05-27 - stellar/js-stellar-base

- Issue/PR: https://github.com/stellar/js-stellar-base/issues/966 and https://github.com/stellar/js-stellar-base/pull/968
- Change: Added CAP-40 signed payload signer support to revoke signer sponsorship parsing and building.
- Verification: Ran focused mocha coverage for `revokeSignerSponsorship`, source ESLint checks, syntax checks, and `git diff --check`.
- Result: Pull request opened against `stellar/js-stellar-base`.
- Lesson: Parser and builder paths for XDR union arms should stay in parity across related operation helpers.

### 2026-05-27 - stellar/js-stellar-base

- Issue/PR: https://github.com/stellar/js-stellar-base/issues/728 and https://github.com/stellar/js-stellar-base/pull/969
- Change: Added TypeScript operation type literals for each revoke sponsorship subtype and aligned operation interfaces with runtime `operation.type` values.
- Verification: Ran `corepack yarn dtslint --localTs node_modules/typescript/lib types/`, `node --check types/test.ts`, and `git diff --check`.
- Result: Pull request opened against `stellar/js-stellar-base`.
- Lesson: Type definitions should mirror runtime discriminants so downstream clients can switch exhaustively without local workarounds.

### 2026-05-27 - stellar/js-stellar-base

- Issue/PR: https://github.com/stellar/js-stellar-base/issues/789 and https://github.com/stellar/js-stellar-base/pull/970
- Change: Updated amount validation errors to mention the maximum 64-bit signed integer limit and added a `destMin` regression test.
- Verification: Ran focused mocha coverage for `pathPaymentStrictSend`, source ESLint, syntax checks, and `git diff --check`.
- Result: Pull request opened against `stellar/js-stellar-base`.
- Lesson: Validation errors should name boundary conditions when a single generic message can hide the actual cause.

### 2026-05-27 - wevm/prool

- Issue/PR: https://github.com/wevm/prool/issues/44 and https://github.com/wevm/prool/pull/79
- Change: Cleaned up instance start timeout handling so timed-out starts reject catchably, reset to `idle`, and ignore late start resolution.
- Verification: Ran `pnpm exec tsc --noEmit`, focused `Instance.test.ts` coverage, Biome checks, and `git diff --check`.
- Result: Pull request opened against `wevm/prool`.
- Lesson: Timeout wrappers should own cleanup and guard against late async completions changing state after rejection.

### 2026-05-27 - stellar/js-stellar-base

- Issue/PR: https://github.com/stellar/js-stellar-base/issues/347 and https://github.com/stellar/js-stellar-base/pull/971
- Change: Updated `setOptions` flag input types so bitwise bitmap expressions and string flag values work without TypeScript casts.
- Verification: Ran `corepack yarn dtslint --localTs node_modules/typescript/lib types/`, `node --check types/test.ts`, and `git diff --check`.
- Result: Pull request opened against `stellar/js-stellar-base`.
- Lesson: Type declarations for SDK builders should match the runtime input contract, especially for bitmask-style fields.

## Entry template

```markdown
### YYYY-MM-DD - Repository

- Issue/PR:
- Change:
- Verification:
- Result:
- Lesson:
```
