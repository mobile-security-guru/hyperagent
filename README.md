# hyperagent

Open, forkable edge agent that scores mobile trust boundaries. It runs on Cloudflare Workers, calls no external LLM vendor, and keeps telemetry in your own account.

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/mobile-security-guru/hyperagent)

> **Status: pre-release.** The repo is public and the license is final. The agent core lands in v0.1.0. Watch releases if you want the tag rather than the commits.

## What it does

Mobile controls are easy to state and hard to verify. Identity, account recovery, communications, and sensitive access all move through the phone, and the evidence that they are configured the way policy says lives in half a dozen consoles.

`hyperagent` runs at the edge, scores what it can observe, and emits an attestation you can hand to someone who will ask questions about it.

```
trust boundary index    68 / 100
band                    ELEVATED
emitted                 attestation.json
runtime                 cloudflare worker
```

Sample output. Your numbers will differ.

## Who it is for

Security and IT leads who have to answer for the phone: CISOs, IT directors, and compliance leads in healthcare, financial services, and defense. It is equally useful to any developer who wants a deployable scoring agent they fully control.

## Run it

```bash
git clone https://github.com/mobile-security-guru/hyperagent
cd hyperagent
npm install
npx wrangler dev
```

Deploy with `npx wrangler deploy`, or use the button above for a fresh Cloudflare account. Every binding in `wrangler.jsonc` uses a placeholder name, so nothing points at someone else's account.

## Design decisions

**No vendor LLM key required.** Workers AI is the default so a fresh fork runs without you signing up for anything else.

**Your data stays in your account.** The Worker, the storage bindings, and the emitted attestations all live in the Cloudflare account you deployed into.

**MIT, deliberately.** Fork it, rename it, resell it. That is the intended behavior.

## Sponsors

Sponsorship funds the open core and pays for the modules that follow. Tiers run from $5 to a capped Founding Sponsor tier, and at 50 total sponsors the launch module is relicensed to public MIT for everyone.

[Sponsor Mobile Security Guru](https://github.com/sponsors/mobile-security-guru)

Scoped assessment and engineering work is not part of any sponsor tier. That runs separately as a Mobile Risk Reduction Exercise (MRRE).

## Contributing

Issues and Discussions are open. Read `SECURITY.md` before reporting anything that looks like a vulnerability, and do not open a public issue for it.

## License

MIT. See `LICENSE`.
