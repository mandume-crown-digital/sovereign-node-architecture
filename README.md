# The Sovereign Node — Architecture & Transfer

**Status:** Operational
**Settlement Rail:** Native Bitcoin (bc1q)
**Classification:** Strategic Asset Transfer

## Overview
The Sovereign Node is a self-hosted, closed-loop digital infrastructure node. It is designed to operate independently of legacy banking and third-party SaaS gatekeepers. It is delivered as a transferable blueprint and a fully keyed, live instance.

## Core Stack
* **Web/App Layer:** Hardened LEMP Stack (Linux, Nginx, MySQL, PHP)
* **Oracle Component:** Self-hosted proprietary architecture for deterministic delivery and token-gated access
* **Delivery Engine (CIWS):** Automated dispatch integrated via API
* **Settlement Rail:** Native Bitcoin (bc1q) via custom PHP gateway (`dpo_initiate.php`). No third-party processors. No chargeback vectors.

## Repository Contents
* [`/runbook`](./runbook/deployment.md) - The 5-step deployment protocol for the acquiring entity.
* [`/security`](./security/threat_model.md) - The blast-radius isolation and correlated vulnerability analysis.
* [`/custody`](./custody/key_chain.md) - The current single-node custody state and the mandatory multisig transition plan.

## Transfer Status
This architecture is being offered for a Private Sovereign License or Exclusive Acquisition. For the full 5-page dossier, contact the Operator:
**Email:** ryanhauala@outlook.com
