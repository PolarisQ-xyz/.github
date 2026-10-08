# Polaris

Non-custodial, multi-oracle prediction markets on Stellar (Soroban). Binary markets and continuous perpetuals, settled by a Pyth Lazer price verified on-chain and cross-checked against Reflector Network before any funds move — or, when no Lazer access is configured, settled via a second real entrypoint backed by Reflector's live on-chain price directly. Gasless, passkey-secured trading — no seed phrase, no browser extension.

**Live**: [polaris-frontend-delta.vercel.app](https://polaris-frontend-delta.vercel.app)

| Repo | Role |
|---|---|
| [polaris-contracts](https://github.com/PolarisQ-xyz/polaris-contracts) | Rust/Soroban: markets, perpetuals, the LP vault, passkey wallets |
| [polaris-oracle](https://github.com/PolarisQ-xyz/polaris-oracle) | NestJS backend: settlement automation, multi-oracle price relay, sponsored transactions, admin API |
| [polaris-frontend](https://github.com/PolarisQ-xyz/polaris-frontend) | Next.js web app: trading UI, portfolio, embeddable widget, admin dashboard |

Each repo's README documents real bugs found by deliberately trying to break the system after it was "done" — not a changelog of hypotheticals, a record of what actually broke, how it was fixed, and the regression test that proves it. Building in the open, so that record is public.

Open to review, questions, and contributions — see each repo's `CONTRIBUTING.md`.
