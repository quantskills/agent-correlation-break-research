# Correlation Break Research Agent

This is a QuantSkills Pandadata research and monitoring agent: `agent-correlation-break-research`.

It is built for researchers, traders, and AI-agent-assisted market review workflows. It does not place orders and does not issue unconditional buy/sell instructions. Its job is to turn real market evidence into readable, reviewable, and reusable research materials.

## What It Helps You Answer

Are the old diversification and correlation assumptions still reliable?

## When To Use It

- You want to decide whether a market state, risk state, or research lead deserves more attention.
- You want Pandadata evidence turned into a report instead of raw tables only.
- You need a watchlist and review checklist for the next observation window.
- You want to hand the result to another researcher or AI agent.

## Primary Watch Focus

跨品种相关性、相关性跨度、强弱联动组。

## How To Read The Output

This repository includes a packaged Pandadata live sample output under `outputs/live/`.

1. Open `outputs/live/report.html` and read the conclusion plus the questions this agent is suited for.
2. Check the three evidence charts: main evidence, supporting evidence, and scorecard metrics.
3. Use `outputs/live/decision_matrix.csv` to separate base, upgrade, downgrade, and insufficient-evidence cases.
4. Use `outputs/live/monitoring_checklist.csv` for the next review window.
5. Use `outputs/live/research_journal_template.md` for review notes and `outputs/live/handoff_card.md` for handoff.

## Materials You Get

| Material | Use |
| --- | --- |
| `outputs/live/report.html` | Start with the conclusion, evidence charts, scenarios, and invalidation conditions. |
| `outputs/live/decision_matrix.csv` | Turns base, upgrade, downgrade, and insufficient-evidence cases into next actions. |
| `outputs/live/monitoring_checklist.csv` | Prioritized watch items for the next review window. |
| `outputs/live/research_journal_template.md` | Template for evidence, counter-evidence, and rerun conditions. |
| `outputs/live/handoff_card.md` | Short handoff for another researcher or AI agent. |
| `outputs/live/data_dictionary.csv` | Tables, fields, and row counts used in the run. |

## Pandadata Methods

- `get_future_dominant_corr`

## Upgrade And Downgrade Clues

- Upgrade watch: 相关性跨度继续扩大，且价格结构也出现风格切换。
- Downgrade watch: 相关性变化来自极短窗口噪声、换合约或数据口径变化。

## Boundary

This is a research and monitoring agent, not an automated trading system. It does not connect to brokers, execute orders, or replace the user's own strategy, risk budget, and execution process.

## License

GNU General Public License v3.0. See [LICENSE](LICENSE).
