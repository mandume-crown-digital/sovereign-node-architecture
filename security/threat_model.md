# Security & Threat Model

## Blast-Radius Isolation
The node is isolated. A compromise of the web server does not grant access to the settlement wallet, which is stored with independent encryption and is not internet-facing.

## Correlated Vulnerabilities
* **Cloud Provider Risk:** The current reliance on a single cloud provider is a correlated risk. Post-transfer, the acquiring entity is advised to deploy the node across multiple geographic regions.
* **Custom Code Audit:** The `dpo_initiate.php` gateway is custom-coded. The acquiring entity's auditors should review the script for edge-case vulnerabilities (e.g., transaction concurrency) prior to scaling. We state this plainly: custom code requires custom audit.

## Patching Regime
Monthly kernel updates and immediate zero-day patches for Nginx/PHP. The `chattr +i` protocol prevents unauthorized script injection, but all root-level access must be monitored.
