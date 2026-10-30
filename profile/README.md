
# Tensorsoft

**Independent research and open-source tooling for crypto, AI, real-world assets and markets.**

We run our own data pipelines and our own capital. The tools here are the parts of that stack we think others can use: data collectors, perp tooling and LP position management. Built for operators who measure before they trade.

🌐 [tensorsoft.tech](https://tensorsoft.tech) · 📝 [Research & blog](https://tensorsoft.tech/blog) · ✉️ [Contact](https://tensorsoft.tech/contact)

---

## Open-source tools

| Tool | What it does | Status |
|---|---|---|
| `perp-cli` | Command-line tool to query funding rates, open interest and positions across perp DEXs; open, reduce and close positions from the terminal | 🗓️ planned |
| `lp-manager-cli` | Command-line tool to monitor and manage DEX liquidity positions: range status, fees earned, impermanent loss, rebalance alerts | 🗓️ planned |

> These tools run in production inside Tensorsoft today and are being prepared for open-source release. Watch this organization to get notified when each repository goes public.

## Design principles

- **Raw data is kept.** Collectors store raw snapshots append-only. Normalization happens on top, so every number can be traced back to its source.
- **Honest units.** Funding is stored per interval *and* annualized, with the annualization convention written down. An annualized rate is not a realized return.
- **Venue quirks are documented.** Default interest components, funding caps, interval lengths and contract differences are listed per venue instead of hidden in code.
- **Local first.** Everything runs on your own machine or server. No hosted service and no keys sent anywhere you didn't configure.
- **Monitoring included.** Tools expose metrics for Grafana and support alerting, because a position you can't see at 3 a.m. is a risk.

## Research built on these tools

| Study | Date |
|---|---|
| [001 · Perpetual funding rates: a week of divergent signals](https://tensorsoft.tech/blog/perp-funding-rates-7-day-study) | 30 Oct 2026 |

## Contributing

Issues and pull requests are welcome, especially new venue adapters and fixes for venue-specific edge cases. Please open an issue first for larger changes.

## Disclaimer

These tools are provided as is, without warranty. They can place real orders and move real funds when configured to do so. Test with small amounts first. Nothing in this organization is investment advice. Trading perpetuals and providing liquidity carry a significant risk of loss.

---

<sub>© 2026 Tensorsoft Research · Crypto · AI · RWA · Markets</sub>
