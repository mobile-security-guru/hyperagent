# hyperagent

Point your own AI agent at these folders and at your own files. It works out which actions in your organization run through a phone, who is allowed to take them, and what proves it today. We never receive your data.

> **v0.1.0.** Method folders for three seats. No code runs here; your agent does the work.

## Start here

Pick your seat and paste its prompt into the agent you already use:

- [CISO](kit/ciso/PROMPT.md)
- [IT Director](kit/it-director/PROMPT.md)
- [Compliance](kit/compliance/PROMPT.md)

See [a sample result](examples/ciso-sample-output.md) (fictitious organization).

## How it works

1. Your agent reads the folders in this repo: the questions, the evidence each answer needs, and the templates to write it down.
2. Your agent reads your own exports inside your own environment. Nothing in this repo sends anything anywhere, and you can read every file to confirm it. [`AGENTS.md`](AGENTS.md) holds the privacy rules your agent follows first.
3. You get a table: each action that runs through a phone, who is authorized to take it, the record that proves it, and **UNKNOWN** wherever no record does. Then a plan to close those gaps with tools you already own.

Your agent's own provider still processes what you give it, under your agreement with them. We are not a party to that and receive none of it.

## Who it is for

One folder per seat, each with its own questions and paste-ready prompt:

- **CISO:** Conditional Access policies, MDM inventory, recent identity incidents
- **IT Director:** MDM inventory, carrier invoices, help-desk tickets for new phones, resets and number changes
- **Compliance:** mobile policy, access reviews, audit evidence requests

## Sponsors

Sponsorship funds new method folders. Tiers start at $25 a month.

[Sponsor Mobile Security Guru](https://github.com/sponsors/mobile-security-guru)

When you hit an UNKNOWN you cannot close on your own, that work runs separately as a Mobile Risk Reduction Exercise (MRRE). No sponsor tier includes it.

## Contributing

Issues and Discussions are open. Read `SECURITY.md` before reporting anything that looks like a vulnerability, and do not open a public issue for it.

## License

MIT. See `LICENSE`.
