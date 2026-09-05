# Kashnio Control Mainnet

## Identity

| Field | Value |
| --- | --- |
| Chain ID | `kashnio-mainnet` |
| Protocol version | `2` |
| Active validator identities | `3` |
| Latest signed native release | `mainnet-v0.2.0-rc8.14` |
| Production Ubuntu onboarding release | `mainnet-v0.2.0-rc8.11-linux` |
| Native asset | `KDG` |
| Display precision | 9 decimal places |
| Account identity | Ed25519 public key |
| Finality model | Validator-certified checkpoints |

## Public endpoints

| Purpose | Endpoint |
| --- | --- |
| RPC base | `https://rpc.kashnio.com/rpc` |
| Redundant RPC base | `https://rpc2.kashnio.com/rpc` |
| RPC health | `https://rpc.kashnio.com/rpc/health` |
| RPC status | `https://rpc.kashnio.com/rpc/status` |
| Indexer base | `https://indexer.kashnio.com/api/indexer` |
| Routed indexer alias | `https://indexer2.kashnio.com/api/indexer` |
| Explorer | `https://explorer.kashnio.com` |
| Wallet | `https://wallet.kashnio.com` |

Only documented routes are supported. The two RPC origins are independently
hosted. Both indexer hostnames route to the same canonical persistent indexer
and must not be counted as independent storage redundancy.

## Finality

Transaction submission is not finality. A transaction should be represented as
finalized only after its receipt is present in a certified finalized
checkpoint and is visible through the authoritative RPC/indexer data path.

Protocol v2 is reconciled across all three canonical validator hosts using
matching finalized checkpoints, state roots, and validator snapshots. A new
operator starts as an isolated observer candidate and is not a voting validator
until a finalized atomic lifecycle transition updates both registry and next
snapshot.

## Safety

- Never share wallet passwords, private keys, or recovery material.
- Verify that links use the `kashnio.com` domain before interacting.
- Verify the signed release, checksum manifest, chain ID, and guardian-approved
  checkpoint before starting an independent node.
