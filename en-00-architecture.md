# AMM Markets Team Architecture

## Goal

AMM Markets is a trading platform and pool-pricing mechanism for LPs. It aims to improve pricing, risk compensation, and execution conditions. It does not custody capital, manage inventory, or manage an LP's complete investment portfolio.

The website platform is separate from the high-frequency on-chain systems. The website does not depend on the high-frequency Ethereum node and never holds user private keys. EOA, Safe, and Safeheron users review and sign transactions in their own wallets.

## Five core roles

```text
AMM Protocol & Research Lead
        │  Hooks, fees, price bounds, AMM research
        ▼
Web3 Platform Engineer ─────── Blockchain & Market Data Platform Engineer
Website, wallets, transactions       On-chain/CEX data, central data platform
        │                              │
        └───────────┬──────────────────┘
                    ▼
Infrastructure, Architecture & Security Engineer
System architecture, servers, network, deployment, security, DR

Ecosystem, Growth & LP Partnerships Lead
External growth, community, LP acquisition, institutions, channels
```

## Collaboration

- The Protocol & Research Lead defines protocol logic, fee mechanisms, and AMM research.
- The Web3 Platform Engineer turns protocol capabilities into website, wallet, and transaction-preview flows.
- The Blockchain & Market Data Platform Engineer provides traceable on-chain and off-chain data.
- The Infrastructure, Architecture & Security Engineer keeps the systems isolated, secure, deployable, and recoverable.
- The Ecosystem, Growth & LP Partnerships Lead connects LPs, institutions, wallets, custodians, and ecosystem partners.

Public metrics such as fee income, fee yield, and APR must have an agreed definition and be checked by the data and protocol owners. Growth should never promise investment returns or publish unverified numbers.

## Principles

- Do not use education, school, company brand, or a fixed number of years as hard filters; prioritize demonstrated ability, judgment, and relevant work.
- Protocol security, data correctness, system security, and custody boundaries must each have clear ownership.
- Smart-contract audits, penetration tests, and legal/compliance reviews may be performed by independent specialists.
- The founder/product owner owns product direction, key institutional relationships, and final business trade-offs.
