# FreedomCore

**Autonomous AI trading systems for crypto perpetuals and on-chain markets.**

FreedomCore builds production trading bots that run themselves. The strategies that drive them are crowned by a multi-LLM swarm that rewrites its own code every cycle, evaluated under honest physics, and only deployed when a new candidate strictly beats the live champion on a fresh out-of-sample window.

The codebase is mature and live with real capital. The strategy IP itself stays in private repositories. The links below are the public surface.

---

## What's live

| Product | What it does | Where it runs |
|---|---|---|
| **MAVERICK** | KuCoin perpetuals trader. Trinity Cascade (three medalist champions running in parallel under a shared risk envelope). | [maverick.freedomcore.io](https://maverick.freedomcore.io/) |
| **SHADOW** | HyperLiquid copy-trading. Cohort-weighted Q-score profiler, scalper-rejecting consensus quorum, 59 wallets across three tiers. | [shadow.freedomcore.io](https://shadow.freedomcore.io/) |
| **ARENA** | Public leaderboard. 75 wallets ranked by Wilson-lower win rate and 6-component Q-score, rebuilt every six hours from SHADOW's profiler database. | [arena.freedomcore.io](https://arena.freedomcore.io/) |
| **QUANTUM** | AI-built portfolios for crypto founders. Static intake, bespoke delivery. | [quantum.freedomcore.io](https://quantum.freedomcore.io/) |

---

## How it works

Five principles you can verify on the live sites:

**1. Honest evaluation.** Every candidate strategy is dual-tested with a 60-second time shift. If its score collapses more than 25% under the brutal pass, it is flagged as future-peeking and zeroed. Lookahead bias does not survive the gate.

**2. Strict beat or hold.** A new candidate must outperform the reigning champion on the same fresh seven-day window. If nothing beats the live system, the system holds. The decision not to evolve is itself intelligence.

**3. Walk-forward validation.** Every survivor must be net positive in each of three rolling two-day sub-windows.

**4. Multi-LLM judicial review.** Three external LLMs review every promotion candidate. Majority crowns one. Disagreement defaults to the incumbent. Council failure never blocks live trading.

**5. Atomic hot-swap.** Live deploys run a 45-second health check. Failure rolls back automatically. No bifurcation between what evaluation saw and what fires on the exchange.

---

## Build cadence

Active development. The swarm runs every cycle. The repositories visible on this profile are the public marketing site, the public ARENA leaderboard, the SHADOW operator tooling, and the infrastructure config. The strategy code is in separate private repositories and stays there.

---

## Stack

Pure NumPy on the hot path. Python and Flask for operator dashboards. SQLite (WAL) for the per-symbol feature store. nginx for the public surface. Solidity for on-chain components. Codex, Gemini, and Claude Opus 4.7 for the swarm and the high-court review chain.

---

## Contact

For partnership, licensing, or buy-side enquiries: [freedomcoreai@gmail.com](mailto:freedomcoreai@gmail.com)

For the live trading bot subscription: [maverick.freedomcore.io/pages/access.html](https://maverick.freedomcore.io/pages/access.html)
