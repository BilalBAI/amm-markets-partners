# AMM Protocol & Pool Policy Lead

## Mission

Own AMM Markets' on-chain trading mechanisms, production Pool Policy algorithms, and quantitative research. The goal is to keep pools tradable within explicit risk boundaries and improve long-term LP economics through verifiable research.

This is a **human leadership role** accountable for the full algorithm lifecycle: research, design, testing, deployment, production operation, and post-incident learning.

## Responsibilities

- Design and maintain Uniswap v4 Hooks, PoolManager-related logic, permissions, and the on-chain semantics of directional fees and price bounds.
- Direct the **Quant Research AI agent** in studying baseline fees, price bounds, trade behavior, LP fee income, inventory, and tail risk; review its data, assumptions, backtests, forward validation, and counterexamples.
- Design and maintain production Pool Policy algorithms, including normal quoting, price recovery, convergence conditions, cooldowns, and safe behavior across market states.
- Own production algorithm **liveness**: detect and resolve prolonged inability to update bounds, pending transactions, blocked nonces, gas constraints, and data failures that stall execution.
- Supervise chain-specific **Policy Manager AI agents** in routine checks, anomaly analysis, and incident recommendations; set consistent operating standards across chains and verify conclusions against on-chain state.
- Define independent data collection and quality gates for each pool. Servers and nodes may be shared, but each production policy manager must manage its own collection, reconnection, health checks, and error handling.
- Establish a verifiable path from research hypotheses and candidate parameters through simulation, testing, review, release, and actual on-chain adoption; retain auditable transaction, nonce, gas, and controller records.
- Define protocol constraints for adding, removing, and moving LP positions and for transaction execution; work with the Web3 Platform Engineer on unsigned transactions and Safe/Safeheron flows.
- Lead production incident reviews and algorithm improvements, verifying that fixes preserve existing risk constraints and do not disrupt other pools.
- Work with the Infrastructure Engineer on monitoring, alerting, isolation, and disaster recovery.
- Use unit and integration tests, historical replay, Foundry, fork tests, fuzzing, and invariant testing to validate contracts and off-chain algorithms; prepare audit materials and production change notes.

## AI agents and accountability

The chain-specific Policy Managers and Quant Researcher are **AI agents assisting this role, not employee positions in this hiring plan**. They may analyze and act within their authorization, but their outputs must retain evidence and remain reviewable. Production changes must still pass testing, review, permission, and release gates.

The human Lead is accountable for agent tasking, work quality, permission boundaries, and production outcomes. Delegation to an AI agent does not remove human accountability for algorithm decisions or incident response.

## Scope and boundaries

- Own protocol mechanisms, the quality of Quant Research, and the correctness and liveness of production Pool Policy algorithms.
- Infrastructure owns servers, nodes, networks, and runtime environments; this role owns algorithm requirements and behavior during infrastructure failures.
- Does not own daily website development, replace independent security audits, sign for LPs or Safeheron, or custody LP funds.
- Material risk trade-offs require appropriate authorization. Liveness or yield goals do not justify silently relaxing safety limits.

## Useful capabilities

- Deep understanding of Uniswap v4, concentrated liquidity, ticks, square-root prices, liquidity, and fee growth.
- Ability to write and review Solidity, Python, and production execution-service code.
- Familiarity with EVM transaction lifecycles, RPC, reorg/finality, nonce, gas, on-chain permissions, and asset flows.
- Ability to design rigorous AMM research and distinguish historical fit, forward evidence, and realized LP economics.
- Experience with production releases, incident response, rollback, and postmortems.
- Ability to supervise AI agents: assign clear tasks, verify evidence, spot faulty conclusions, and control permissions.

## What we value

Production protocol or trading systems, reproducible research and tests, clear incident reviews, and sound judgment across returns, liveness, and risk matter more than degrees or a fixed career timeline.
