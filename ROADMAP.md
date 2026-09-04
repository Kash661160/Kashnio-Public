# Kashnio public roadmap

The roadmap is evidence-driven. Dates are not promised until the relevant technical, operational, security, economic, legal, and governance gates are satisfied.

## Phase 1 — Foundation

**Status: completed for public-beta scope**

- Deterministic Layer-1 protocol foundation
- Canonical transactions and Ed25519 identities
- DAG execution and checkpoint finality
- Persistent node state and recovery boundaries
- Wallet PWA and explorer foundation
- Signed multi-architecture release pipeline

## Phase 2 — Distributed public testnet

**Status: active public beta**

- Three-validator quorum
- Public RPC, finalized-state indexer, wallet, and explorer
- Signed RC7 Linux x86_64 and ARM64 operator packages, with macOS and Windows test packages
- Restart, partition/rejoin, quorum-loss, and recovery qualification
- Monitoring, bounded public access, and off-host backups
- Controlled faucet qualification
- Public progress and network reporting

**Remaining gates:** longer-duration public load and WebSocket evidence, independent-operator expansion, and continued service-stability observations.

## Phase 3 — Developer and operator expansion

**Status: active and gated**

- Public validator package and verification instructions published
- RPC, SDK, pagination, history, subscription, and fee-estimation stabilization in progress
- Independent-operator acceptance and expanded independently operated infrastructure pending
- Additional integration documentation and examples planned
- Physical-device wallet qualification and independent wallet review pending

## Phase 4 — Protocol expansion

**Status: active on public testnet; internal pre-audit engineering checklist complete**

The completed Protocol v2 engineering scope covers:

- Validator economics, delegation, unbonding, rewards, and slashing accounting
- Governance, treasury, and snapshot-bound voting
- Fungible and non-fungible asset foundations
- Deterministic WASM contract execution
- Protocol v2 RPC, indexer, SDK, explorer, and wallet integration surfaces
- Versioned state commitments, migration boundaries, and activation controls
- Signed RC7 activation across the three-validator public testnet
- Matching live checkpoints, state roots, and validator snapshots
- Frozen project-controlled pre-audit candidate and verified evidence bundle

Protocol v2 is active for public-testnet testing. Kashnio's internal engineering checklist, security preflight, fault qualification, recovery verification, and release reconciliation are complete for the frozen pre-audit candidate. This project-controlled completion does not replace independent security or economic review and does not authorize mainnet.

## Phase 5 — M7 interoperability and EVM compatibility

**Status: planned; research and specification gated**

M7 is the planned interoperability milestone. Its proposed scope includes:

- Versioned interoperability and proof-verifier interfaces
- Bounded cross-network message and asset-verification foundations
- An EVM-compatibility layer for familiar Ethereum tooling and application migration
- Deterministic mapping for EVM transactions, accounts, logs, receipts, gas, and finality
- Wallet and developer-tool compatibility, including standard EVM JSON-RPC workflows where technically and safely supportable
- Cross-runtime state commitments, upgrade controls, replay protection, and failure isolation
- Dedicated adversarial testing and independent review before any public activation

Kashnio has not represented M7, an EVM runtime, an EVM bridge, or Ethereum-tool compatibility as live. Architecture, compatibility level, trust assumptions, and activation parameters must be specified and reviewed before implementation is treated as production work.

## Phase 6 — Production and mainnet

**Status: not launched; gates remain closed**

Mainnet requires, at minimum:

- Independent protocol, wallet, runtime, economics, and infrastructure security audits
- Confirmed remediation and retesting
- Long-duration public-testnet evidence
- Independent validator participation
- Frozen production protocol, economic, governance, and operational parameters
- Production legal and regulatory review
- Mature incident response and disaster recovery
- Reproducible production genesis ceremony
- Explicit Kashnio launch authorization

Public-testnet progress does not satisfy or bypass these mainnet gates.
