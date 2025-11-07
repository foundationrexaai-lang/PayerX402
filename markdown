```markdown
# Payerx402

A foundation repository for Payer X402 — a unified architecture for confidential, compliant, composable on-chain payments.

This repository contains:
- contracts/: Solidity contracts for the X402 Payment Utility Layer, a Shielded Settlement Pool, and a Stealth Address Registry.
- sdk/: TypeScript SDK to create stealth addresses, interact with contracts, and sign payment requests.
- relayer/: Example Sovereign Relayer Network node (Express + TypeScript).
- scripts/: Deployment scripts (Hardhat).
- test/: Unit tests (Hardhat + Mocha/Chai).
- docs/: Architecture notes and next steps.

Quick start (development)
1. Install dependencies
   - `npm install`
2. Compile contracts
   - `npx hardhat compile`
3. Run local node and tests
   - `npx hardhat node`
   - `npx hardhat test`
4. Deploy locally
   - `npx hardhat run --network localhost scripts/deploy.ts`

Notes
- This repo contains placeholder privacy logic for development. Do not use the placeholder cryptography in production.
- Replace the ShieldedPool with a zk-enabled implementation (circom/snarkjs, Halo2, or other) and implement secure stealth address derivation.

License: MIT
```
