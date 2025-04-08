# ReLeaf – Verifiable Climate Action & Funding DAO

**ReLeaf** is a decentralized protocol on the Solana blockchain that enables individuals and communities to log verifiable environmental actions, earn on-chain reputation, and access funding through a decentralized autonomous organization (DAO) that supports grassroots ecological projects.

---

## Why ReLeaf?

Today’s climate initiatives often lack transparency, coordination, and verifiability. ReLeaf provides a solution by turning real-world environmental efforts into on-chain credentials, enabling communities to propose, fund, and track eco-projects in a decentralized, auditable manner.

---

## Key Features

- **Proof of Action:** Submit geo-tagged, timestamped evidence (photos, metadata) for eco-actions like tree planting, cleanups, or restoration work.
- **Soulbound GreenNFTs:** Non-transferable reputation NFTs are issued upon successful verification of climate action.
- **DAO Governance:** Token or NFT-based voting enables community-driven approval and funding of environmental projects.
- **Milestone-based Disbursal:** Project funds are released in phases tied to progress updates and verified deliverables.

---

## Use Cases

- **Activists** build on-chain climate credentials through verified contributions.
- **Communities** access funding for local, regenerative initiatives.
- **Funders** support transparent, milestone-tracked climate efforts.
- **DAOs** allocate treasury assets towards measurable impact.

---

## Technology Stack

| Layer           | Technologies                          |
|------------------|----------------------------------------|
| Blockchain        | Solana                               |
| Smart Contracts   | Rust, Anchor Framework               |
| NFT Layer         | Metaplex, Soulbound NFT Logic        |
| Frontend          | React, TypeScript, Tailwind CSS      |
| Wallet Support    | Solana Wallet Adapter (Phantom, Backpack) |
| Data Storage      | IPFS / Arweave                       |
| Governance        | PDA-based voting, vesting schedules  |
| Oracles (Optional)| Chainlink Functions (proof validation) |

---

## Architecture Overview

- **GreenNFT Program:** Issues soulbound NFTs after eco-proof is validated.
- **Reputation PDA:** Tracks user participation and contribution levels.
- **Proposal PDA:** Stores project proposals, milestones, and governance data.
- **Vault Program:** Handles treasury disbursal based on verified milestone completions.

---

## Testing Strategy

- Unit tests using Anchor for all smart contract modules
- Integration tests across the full flow (submission → NFT minting → proposal → disbursal)
- Mock oracle testing for media/GPS verification
- Security and governance checks on treasury management logic

---
## Project Timeline

| Week | Deliverable / Milestone                                      |
|------|--------------------------------------------------------------|
| 1    | Project setup, initial repo structure, system architecture design |
| 2    | GreenNFT smart contract development and proof submission interface |
| 3    | DAO governance logic (Proposal PDA, voting logic)            |
| 4    | Vault contract for milestone-based fund disbursal            |
| 5    | Frontend integration with wallet, GreenNFT, and DAO modules  |
| 6    | Oracle setup for proof validation (media, GPS), optional     |
| 7    | Full-stack integration tests, unit tests, QA, documentation  |
| 8    | Final deployment, DAO walkthrough, and capstone presentation |

## Local Setup

```bash
git clone https://github.com/irohanrajput/releaf-turbin3-capstone.git
cd releaf

# Frontend
cd frontend
yarn install
yarn dev

# Solana Programs
cd ../programs
anchor build
anchor test




