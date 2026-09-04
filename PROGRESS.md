# Kashnio public progress

Last updated: 2026-08-12

## Operational public-testnet foundation

The following public-beta milestones have been completed:

- Signed RC7 Linux x86_64 and ARM64 testnet validator packages have published checksums, Sigstore bundles, release provenance, and operator verification instructions; macOS and Windows operator packages are also published for independent testing.
- Three-validator quorum finalizes matching checkpoints, state roots, and validator snapshots.
- Restart, quorum-loss, partition/rejoin, and state-recovery trials passed within the defined public-beta scope.
- Validator services persist across host restarts and use restricted networking and loopback-only application interfaces.
- Automated validator health checks, off-host backups, and PostgreSQL backups are active.
- The finalized-state indexer synchronizes public RPC state and supports bounded pagination and replacement-indexer comparison.
- The branded explorer serves transactions, finalized checkpoints, accounts, validators, receipts, and network status.
- The self-custody wallet reads live finality, stores accounts in an encrypted local vault, signs locally, supports backup and recovery, and completed a finalized end-to-end testnet transfer.
- Mobile wallet layouts and Progressive Web App behavior have been improved for public beta testing.
- The controlled faucet passed concurrency and allocation qualification and remains publicly disabled.
- Public website, wallet PWA, RPC, indexer, explorer, identity agreement, and finality progression are covered by external monitoring.

## Protocol v2 engineering milestone

Protocol v2 is active on `dag-l1-testnet-2`. Its completed scope includes validator economics, delegation and unbonding, deterministic reward accounting, validator accountability, governance and treasury controls, fungible and non-fungible assets, deterministic WASM contract execution, and the associated protocol, storage, RPC, indexer, SDK, explorer, and wallet integration boundaries.

The three validators run the signed RC7 Protocol v2 node and have repeatedly reported matching checkpoints, state roots, and validator snapshots. The public RPC, indexer, explorer, and wallet expose the live Protocol v2 path, including the finalized KDGTEST test asset. KDGTEST has no monetary value.

## Internal pre-audit checklist

Kashnio completed the project-controlled Protocol v2 pre-audit engineering checklist on 2026-08-12. Completed verification includes:

- RC7 deployment and three-host finality reconciliation
- Reproducible x86_64 and ARM64 release evidence and operator-package qualification
- Live wallet → RPC → validator → indexer → explorer verification
- Public API, SDK, wallet, and explorer consistency checks
- Restart, partition/rejoin, quorum-loss, recovery, equivocation, stale-vote, and clock-skew qualification
- PostgreSQL migration/restore, pagination, and controlled-faucet concurrency qualification
- Validator and indexer monitoring, backup, recovery-vault, and access-closure checks
- Dependency remediation, secret preflight, and deterministic audit-bundle verification

The exact candidate is frozen under `protocol-v2-preaudit-2026-08-12`. Its verified audit-bundle SHA-256 is `6de8f095c8ea7b7a07657f9fa556eaa7c381cfbef845343949af350213fea75a` and its source-tree SHA-256 is `c915c6e1744ebb0132cede500d7137399514f4119075a28ae753957e10af50e0`.

“Internal pre-audit checklist complete” means Kashnio completed its own engineering and evidence gates. It does not mean an independent auditor has reviewed or approved the protocol.

## Current operating boundary

Kashnio is a public testnet beta, not a production or mainnet network.

- Testnet balances have no monetary value.
- The faucet is not publicly available.
- Validator participation is presently controlled while independent-operator onboarding is qualified.
- Public endpoints are subject to testnet maintenance and capacity limits.
- Protocol v2 is active for controlled public-testnet testing; testnet functionality and balances are not production assets.
- Bridges and advanced interoperability remain later gated milestones.
- Internal audit-readiness work does not mean an independent audit has been completed.
- Independent security review remains required before production or mainnet representation.

## Next active work

- Collect longer-duration public load, WebSocket, synchronization, and recovery evidence.
- Complete live onboarding with a truly independent validator operator.
- Finish physical-device wallet testing and independent wallet review.
- Complete independent protocol, economics, runtime, and infrastructure audits and remediation confirmation.
- Specify and prototype the gated M7 interoperability and EVM-compatibility roadmap.
- Freeze approved production economic, governance, legal, and operational policies before any mainnet decision.

Progress statements describe completed evidence only; planned or inactive capabilities are not represented as live.
