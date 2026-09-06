# Kashnio Public

Kashnio Public is the official transparency repository for Kashnio development,
Control Mainnet progress, network updates, release verification information, and
community-facing documentation.

This repository intentionally does **not** contain the proprietary Kashnio
protocol, validator, wallet, presale, infrastructure, or deployment source
code.

## Current status

**Stage:** Controlled mainnet operation<br>
**Network:** `kashnio-mainnet`<br>
**Active protocol:** Version 2<br>
**Protocol v2:** Activated across the canonical three-validator set<br>
**Latest signed native release:** `mainnet-v0.2.0-rc8.14`<br>
**Production onboarding release:** Ubuntu `mainnet-v0.2.0-rc8.11-linux`<br>
**Validators:** Three active validator identities<br>
**Internal pre-audit checklist:** Complete<br>
**Independent audit:** Pending<br>
**Open validator admission:** Qualification required; no candidate is counted before finalized atomic activation

Control Mainnet availability must not be interpreted as an independent audit,
production certification, investment guarantee, or unrestricted validator
admission. A downloaded node begins outside consensus and cannot affect quorum.

## Latest update

**Three-host Kashnio runtime verification completed — 2026-09-05**

All three fixed core validators now run under Kashnio service, account,
hostname, configuration, executable, and state-path conventions. A common
finalized sample matched all three validators at height 330,211 and public
finality subsequently advanced beyond height 330,229. The public Explorer
reported every service component operational, with two agreeing RPC origins
and the canonical persistent indexer healthy.

- [Verify live network status](https://explorer.kashnio.com/status)
- [Read the current network boundary](NETWORK.md)

**RC8.14 signed cross-platform release published — 2026-09-03**

RC8.14 provides signed native Linux, macOS, and Windows packages with checksum
and signature evidence. The five-minute production onboarding path remains the
signed RC8.11 Ubuntu release; macOS and Windows are development and controlled-
test builds, not the production always-on validator path.

- [Verify RC8.14 release evidence](https://github.com/Kash661160/Kashnio-Public/releases/tag/mainnet-v0.2.0-rc8.14)
- [Open the production Ubuntu onboarder](https://github.com/Kash661160/Kashnio-Public/releases/tag/mainnet-v0.2.0-rc8.11-linux)

### Previous updates

**Protocol v2 pre-audit engineering milestone completed — 2026-08-12**

Kashnio has activated Protocol v2 on the public testnet and completed its
project-controlled pre-audit engineering checklist. RC7 reconciliation,
three-validator state agreement, public wallet/explorer verification,
reproducible release evidence, SDK/API consistency, recovery, monitoring,
backups, security preflight, and fault qualification are complete within the
documented testnet scope. The candidate is frozen for independent review.

This is an internal engineering-completion milestone—not an independent audit,
production certification, or mainnet approval.

[Read the complete Protocol v2 update →](UPDATES/2026-08-12.md)

- [Development update — 2026-07-30](UPDATES/2026-07-30.md)
- [Signed RC12 validator release](https://github.com/Kash661160/Kashnio-Public/releases/tag/testnet-v0.1.0-rc12)

## Public services

| Service | Address |
| --- | --- |
| Website | https://kashnio.com |
| Wallet | https://wallet.kashnio.com |
| Explorer | https://explorer.kashnio.com |
| Read-only RPC | https://rpc.kashnio.com/rpc |
| Redundant read-only RPC | https://rpc2.kashnio.com/rpc |
| Finalized-state indexer | https://indexer.kashnio.com/api/indexer |
| Routed finalized-state indexer alias | https://indexer2.kashnio.com/api/indexer |

## Documentation

- [Progress and current evidence](PROGRESS.md)
- [Public roadmap](ROADMAP.md)
- [Network information](NETWORK.md)
- [Security reporting](SECURITY.md)
- [License](LICENSE)
- [Copyright and permitted use](COPYRIGHT.md)

## Repository purpose

This repository exists so the public can follow what Kashnio is building,
which milestones are complete, which capabilities are active, and which gates
remain. It is not an open-source distribution and grants no permission to
reproduce the proprietary implementation.

See the [Kashnio Proprietary License](LICENSE) and
[copyright notice](COPYRIGHT.md) before using any repository material.

Copyright © 2026 Kashnio. All rights reserved.
