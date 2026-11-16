# Skill Curriculum

Four levels, worked in order, with honest status markers. Status is
updated only when the work exists. A level is not "done" because it was
read about; it is done when the listed work is complete and can be
shown.

Status markers:

- ✅ Done — the work exists and can be shown.
- 🔄 Started — work has begun; the evidence is named.
- ⬜ Not started — no work yet.

Last updated: 2026-11-16.

## Level 1 — Fundamentals

The ground every later level stands on: how Ethereum works, how
Solidity expresses it, and how to use the tools that hold the work.

- [ ] Ethereum fundamentals: accounts, transactions, gas, the EVM
      execution model — ⬜ Not started
- [ ] Solidity syntax and semantics: types, storage layout, function
      visibility, inheritance, events — ⬜ Not started
- [ ] Solidity reference reading: the official documentation's
      security considerations section, read end to end — ⬜ Not started
- [ ] Git and GitHub: repositories, commits, branches, pull requests —
      🔄 Started (GitHub account created 2026-11-16; local git use
      underway; no repositories published yet)
- [ ] Reading and tracing existing contract code without tooling
      assistance — ⬜ Not started
- [ ] Writing, compiling, and deploying a contract to a local chain —
      ⬜ Not started

## Level 2 — Security Analysis

Recognizing vulnerability classes from their causes, not their
symptoms, and reasoning about a contract's invariants.

- [ ] Reentrancy: mechanics, the checks-effects-interactions pattern,
      cross-function and cross-contract variants — 🔄 Started (study
      note drafted from primary sources; lab proof of concept executed
      — see `web3-security-research` and `bug-bounty-reports`)
- [ ] Access-control failures: ownership, roles, initialization,
      proxy and library patterns — 🔄 Started (study note drafted from
      primary sources, including the Parity incidents — see
      `web3-security-research`)
- [ ] Integer and precision issues: overflow behavior pre- and
      post-0.8.0, rounding, division order — ⬜ Not started
- [ ] Oracle and price-manipulation analysis: AMM math, TWAP,
      decentralized oracles — 🔄 Started (analysis drafted from the
      Uniswap v2 whitepaper and incident post-mortems — see
      `defi-security-research`)
- [ ] Signature and replay issues: `ecrecover` pitfalls, EIP-712,
      nonce handling — ⬜ Not started
- [ ] Upgradeability and proxy patterns: delegatecall, storage
      collisions, initialization of implementations — ⬜ Not started
- [ ] Denial-of-service patterns: unbounded loops, gas griefing, push
      vs pull payments — ⬜ Not started
- [ ] SWC registry: read every entry, with at least one worked example
      per class — ⬜ Not started
- [ ] Invariant reasoning: stating a contract's invariants before
      looking for violations — ⬜ Not started
- [ ] Reading real audit reports and post-mortems, with written
      summaries — ⬜ Not started

## Level 3 — Security Tools

Tools that verify what analysis suspects. Each tool counts only when
it has been run against real code and the output understood.

- [ ] Foundry: forge, cast, anvil — writing and running tests,
      fuzzing, forking mainnet state — 🔄 Started (Foundry 1.9.0
      installed; first lab test written and run, passing, 2026-11-16;
      fuzzing and forking not yet attempted)
- [ ] Static analysis: Slither — running it, reading output, triaging
      false positives — ⬜ Not started
- [ ] Symbolic execution / property testing: Echidna or Halmos —
      ⬜ Not started
- [ ] Formal verification concepts: reading a Certora or Kontrol
      specification — ⬜ Not started
- [ ] Transaction tracing and debugging: Tenderly, Phalcon, or
      `cast` traces — ⬜ Not started
- [ ] Testnet deployment and interaction: deploying to Sepolia,
      verifying on Etherscan — ⬜ Not started

## Level 4 — Real Bounty Hunting

Working inside real programs, under real rules. This level starts only
when the earlier levels can support it.

- [ ] Coding bounties: completing a first entry on a coding-bounty
      platform — 🔄 Started (first entry submitted on make.fun as
      @agent-muse, 2026-11-16; result pending; described in general
      terms in the journal entry for that date)
- [ ] Reading a bug bounty program's scope, rules, and severity rubric
      before any testing — ⬜ Not started
- [ ] First scoped review: a full read of an in-scope codebase, with
      written notes, no submission — ⬜ Not started
- [ ] First submission to a bug bounty program — ⬜ Not started
- [ ] First triaged finding — ⬜ Not started
- [ ] First accepted finding — ⬜ Not started
- [ ] First public disclosure, with the program's consent — ⬜ Not started
- [ ] Competitive audit participation (Code4rena, Sherlock, Cantina)
      — ⬜ Not started

## Rules

1. A status changes only when the work exists. Reading about a tool is
   not using it; drafting a note is not finishing a level.
2. Evidence is named in the status line: the file, the test, the
   submission — something checkable.
3. Level 4 work follows program rules exactly: only explicitly
   permitted targets, no out-of-scope testing, no access to user data,
   no disruption of services.
4. The curriculum is revised as learning reveals what it missed. Gaps
   found are added, not hidden.
