# Kashnio public progress

Last updated: 2026-09-05

## Controlled Mainnet

Kashnio operates a fixed three-validator core. All three validators report the
same finalized snapshot and continue to advance finality. Public service health
is derived from this fixed core and finalized quorum; an external participant
is never treated as a Kashnio-operated service dependency.

The active runtime uses Kashnio service names, operating-system accounts,
hostnames, configuration roots, executable roots, state roots, monitoring, and
public domains. The original signed chain identity remains cryptographically
bound inside genesis and finalized history and is not rewritten during a brand
change.

## Verified public services

- Two independently hosted RPC origins agree on finalized identity.
- The canonical persistent indexer follows finalized state and serves the
  Explorer.
- The Explorer, wallet, documentation, website, support, presale-facts, and
  risk pages respond through Kashnio domains.
- The Explorer status page reports RPC, indexer, validator snapshot, quorum,
  finality freshness, and operator notices from live finalized data.
- External monitoring verifies DNS, RPC, snapshot, indexer, Explorer identity,
  finalized quorum, and bounded indexer lag.

## Independent validator boundary

The original three validators are the complete Kashnio-operated service layer.
Any validator admitted later is an independently operated participant. It
starts outside consensus, generates keys locally, imports a guardian-signed
checkpoint, synchronizes, and can become active only through a finalized atomic
lifecycle transition that updates registry and next snapshot together.

An independent participant may stop or delete its host without making Kashnio
RPC, indexer, Explorer, wallet, gateway, or overall service status degraded.
Loss of finalized core quorum must still be reported.

## Releases

- Latest signed native release: `mainnet-v0.2.0-rc8.14`
- Production Ubuntu onboarding release:
  `mainnet-v0.2.0-rc8.11-linux`
- macOS and Windows packages are signed developer and controlled-test builds,
  not the production always-on validator path.

## Remaining external gates

- Independent protocol and runtime security review
- Continued recovery and long-duration load qualification
- A clean live rehearsal of the public independent-validator onboarding flow
- Publication of future compatibility or validator-policy changes before
  activation

Progress statements describe verified evidence only. They are not an
investment promise, independent audit, or guarantee of future value.
