# Key Custody Chain

## Current State (Single-Node)
* **Master Key:** Locked on-server via `chattr +i` (immutable flag). Cannot be altered or deleted, even by root.
* **Settlement Wallet:** Native Bitcoin wallet with local encrypted keys.
* **Backup:** Physical air-gapped USB (The Ark) containing the encrypted architecture and Master Key.

## Post-Transfer State
* The buyer receives the deployment blueprint and initial keyed instance.
* The buyer's security team initiates a 2-of-3 Multi-Signature (Multisig) custody solution (Mandatory for institutional holding).

## Honest Risk Assessment
The current single-node structure is highly secure against external threat but vulnerable to localized physical failure. The multisig transition is the mandatory primary post-transfer objective.
