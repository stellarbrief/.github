# StellarBrief

Small open-source tools for people who run or build on Stellar. Each one answers a question that
comes up around protocol upgrades and security announcements.

**See them work without installing anything:** [stellarbrief.github.io](https://stellarbrief.github.io)
shows real recorded runs that you can replay and re-analyze in your browser, with the source and date of
every result.

| Tool | The question it answers | Status |
| --- | --- | --- |
| [advisory-brief](https://github.com/stellarbrief/advisory-brief) | "What does this advisory or release mean for us?" Plain-language briefs for non-engineers, where each claim cites a quote that code checks against the source text, or is marked unknown. | Web app you run locally. |
| [upgrade-preflight](https://github.com/stellarbrief/upgrade-preflight) | "Will my Soroban contracts behave or cost differently after the next protocol upgrade?" Runs your scenarios on two real local networks at different protocol versions and diffs the results. | CLI and GitHub Action, `v0.1.0`. |
| [upgrade-drill](https://github.com/stellarbrief/upgrade-drill) | "What happens to a validator network during an upgrade vote?" Boots real `stellar-core` containers locally, runs a scripted vote, and reports what each node did. | CLI, `v0.1.0`. Local use only. |

They serve different people in the same upgrade cycle: anyone reading the announcement,
contract developers, and validator operators.

## Where this stands

These projects are new, with one maintainer. Each README says what has been verified by a real
run and what has not, and each has a changelog listing known limits. Nothing here is affiliated
with the Stellar Development Foundation, and none of it is meant for production use.

## Contributing

Each repository has a `CONTRIBUTING.md` with setup steps, the PR flow, and how issues are rated,
and an `ISSUES_BACKLOG.md` of scoped candidate work. Open an issue before starting anything
large. Report security problems through each repository's private vulnerability reporting (see
its `SECURITY.md`), not in a public issue.
