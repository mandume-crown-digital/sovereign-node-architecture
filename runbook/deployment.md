# Deployment Runbook

The architecture is delivered as a turnkey blueprint. Maintenance and operations shift entirely to the acquiring entity upon handoff.

## Provision
1. Spin up the required hardware (bare metal or Virtual Private Cloud).
2. Ensure the environment meets the minimum specifications for the hardened LEMP stack.

## Harden
1. Apply the provided iptables and ufw configurations (Ports 22, 80, 443 only).
2. Disable root SSH login. Enforce key-only authentication.
3. Install Fail2ban for intrusion prevention.

## Deploy
1. Extract the architecture package.
2. Deploy Nginx server blocks and PHP-FPM pools.
3. Provision the isolated database.

## Verify
1. Run the CIWS diagnostic.
2. Test the bc1q routing script against a testnet or micro-transaction.

## Handoff
1. The Operator transfers domain DNS and revokes all previous SSH keys.
2. The buyer assumes total root control.
