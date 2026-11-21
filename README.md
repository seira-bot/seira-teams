# Seira teams

Community team templates for [Seira](https://seira.bot). Each template sets up a small team of bots for one outcome.

Seira reads [`catalog.json`](catalog.json) from this repository. You can also copy a playbook to any other agent product.

## Teams

| Team | Outcome | Bots | Markdown |
| --- | --- | ---: | --- |
| [SEO Growth Team](teams/seo-growth) | Prioritize search work most likely to grow qualified traffic | 4 | [Open](packages/seo-growth.md) |
| [Engineering Team](teams/engineering) | Take a software change from intent to a verified release | 4 | [Open](packages/engineering.md) |
| [100x Marketing Team](teams/100x-marketing) | Launch a focused campaign and make a stop-or-scale decision | 4 | [Open](packages/100x-marketing.md) |
| [Reddit Lead Miner](teams/reddit-lead-miner) | Find qualified Reddit leads with source evidence | 2 | [Open](packages/reddit-lead-miner.md) |
| [Competitor Watch](teams/competitor-watch) | Turn material competitor changes into a decision brief | 2 | [Open](packages/competitor-watch.md) |
| [Inbox Follow-up](teams/inbox-follow-up) | Recover sales conversations where your team owes the next step | 2 | [Open](packages/inbox-follow-up.md) |

## Use a playbook

1. Choose a team in Seira, or open its Markdown file here.
2. Seira installs the team for you. For another product, give the Markdown to its Chief of Staff.
3. Ask the Chief of Staff to activate the team.

Seira creates the bots, rooms, playbooks, connector intent, and paused routines. Suggested routines always start paused.

A playbook lists required connections. It never contains credentials, conversations, approvals, memory, local paths, or secrets.

## Repository structure

- [`teams/`](teams) holds one folder for each team, with its skills and manifest.
- [`packages/`](packages) holds the one-file Markdown playbooks.
- [`catalog.json`](catalog.json) indexes the teams.
- [`schema/`](schema) holds the JSON schema of the team manifest.
- [`FORMAT.md`](FORMAT.md) describes the file formats.

Run `npm install` and then `npm test`. The test builds `catalog.json`, `packages/<slug>.md`, and `team.seirateam.json`, and then checks them. Do not edit those generated files by hand.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before you propose a team. This repository does not accept secrets, binary bundles, or executable scripts.

## License

MIT
