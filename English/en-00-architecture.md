# AMM Markets Team Architecture

## Goal

AMM Markets is a trading platform and pool-pricing mechanism for LPs. It aims to improve pricing, risk compensation, and execution conditions. It does not custody capital, manage inventory, or manage an LP's complete investment portfolio.

The website platform is separate from the high-frequency on-chain systems. The website does not depend on the high-frequency Ethereum node and never holds user private keys. EOA, Safe, and Safeheron users review and sign transactions in their own wallets.

## Five core hiring roles

These five are proposed **human positions**. Chain-specific Policy Managers and Quant Research are existing **AI agents**, not additional employee positions.

- **AMM Protocol & Pool Policy Lead**: owns Hook mechanisms, production Pool Policy algorithms, and Quant Research; is accountable for algorithm correctness and liveness and supervises the Policy Manager and Quant Research AI agents.
- **Web3 Platform Engineer**: website, wallets, LP workflows, and transaction previews.
- **Blockchain & Market Data Platform Engineer**: historical on-chain/CEX data, the central data platform, and public metrics.
- **Infrastructure, Architecture & Security Engineer**: system architecture, servers, networking, deployment, security, and disaster recovery.
- **Ecosystem, Growth & LP Partnerships Lead**: growth, community, LP acquisition, institutional partnerships, and channels.

## Human leadership and AI agents

```text
AMM Protocol & Pool Policy Lead (human)
├── Quant Research AI agent: baseline fee / price-bound research and validation
└── Chain-specific Policy Manager AI agents: production checks, anomaly analysis,
    and actions within their authorization

Web3 Platform Engineer                 Blockchain & Market Data Platform Engineer
Website, wallets, transaction flows    Historical on-chain/CEX data, central platform
Infrastructure, Architecture & Security Engineer
Runtime environments, deployment, security, disaster recovery
Ecosystem, Growth & LP Partnerships Lead
LPs, institutions, wallets, and ecosystem partnerships
```

AI agent analyses and actions must retain reviewable evidence and follow production testing, review, permission, and release gates. The human Lead remains accountable for tasking, work quality, permission boundaries, and production outcomes.

## Collaboration

- The Protocol & Pool Policy Lead defines protocol logic and algorithm operating standards, reviews Quant Research evidence, and works with chain-specific Policy Managers to maintain production liveness.
- The Web3 Platform Engineer turns protocol capabilities into website, wallet, and transaction-preview flows.
- The Blockchain & Market Data Platform Engineer provides traceable historical and research data. Each production policy manager manages its own collection, reconnection, health checks, and error handling rather than relying on the central platform to operate them.
- The Infrastructure, Architecture & Security Engineer keeps systems isolated, secure, deployable, and recoverable, coordinating failure behavior with the algorithm owner.
- The Ecosystem, Growth & LP Partnerships Lead connects LPs, institutions, wallets, custodians, and ecosystem partners.

Public metrics such as fee income, fee yield, and APR must have an agreed definition and be checked by the data and protocol owners. Growth should never promise investment returns or publish unverified numbers.

## Principles

- Do not use education, school, company brand, or a fixed number of years as hard filters; prioritize demonstrated ability, judgment, and relevant work.
- Protocol security, production algorithm liveness, data correctness, system security, and custody boundaries must each have clear ownership.
- Smart-contract audits, penetration tests, and legal/compliance reviews may be performed by independent specialists.
- The founder/product owner owns product direction, key institutional relationships, and final business trade-offs.
