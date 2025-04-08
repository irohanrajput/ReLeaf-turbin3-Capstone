# 🌿 ReLeaf – Verifiable Climate Action & Funding DAO

**ReLeaf** is a decentralized protocol on **Solana** that empowers individuals and communities to take meaningful climate action, verify their impact, and access funding through a DAO that supports grassroots environmental projects.

---

## 🌍 Why ReLeaf?

🌱 Climate impact should be **verifiable**, **transparent**, and **rewarding**.  
🛠️ ReLeaf turns **eco-actions** into on-chain **reputation** and unlocks **community-driven funding** for local nature projects.

---

## 🔎 Core Features

- ✅ **Proof of Action**: Submit evidence (photos, GPS, metadata) to record cleanups, plantings, and eco-work on-chain
- 🪪 **Soulbound GreenNFTs**: Earn non-transferable reputation NFTs for verified actions
- 🗳️ **ReLeaf DAO**: Propose and vote on grassroots projects needing funding
- 💸 **Milestone-based Disbursal**: Funds released in stages as projects prove real-world progress

---

## 🧭 Use Cases

- **Activists** log verified eco-efforts and build on-chain credibility
- **Communities** propose and get funding for rewilding, cleanups, tree planting
- **DAO members** vote using on-chain eco-reputation
- **Funders** can support verified local impact with full transparency

---

## ⚙️ Tech Stack

| Layer | Tech |
|-------|------|
| Blockchain | Solana |
| Smart Contracts | Rust + Anchor |
| NFT Layer | Metaplex + Soulbound Logic |
| Frontend | React + TypeScript + TailwindCSS |
| Wallets | Solana Wallet Adapter (Phantom, Backpack) |
| Storage | IPFS / Arweave for proof data |
| Governance | PDA-based voting, milestones, and vesting |
| Oracles (Optional) | Chainlink Functions for media/GPS validation |

---

## 🧠 Architecture

- **GreenNFT Program**: Mints soulbound NFTs after eco-proof is submitted
- **Reputation PDA**: Tracks users’ eco-contributions and voting weight
- **Proposal PDA**: Stores proposals, milestones, and DAO votes
- **Vault Program**: Disburses funds based on verified milestone completion

---

## 🧪 Testing Strategy

- Anchor unit tests for each program module
- Integration testing of full flow: proof → NFT → proposal → disbursal
- Mock oracle testing for proof validation
- Security and vesting checks on treasury program

---

## 🧑‍💻 Developer Setup (Coming Soon)

```bash
git clone https://github.com/yourhandle/releaf.git
cd releaf

# Frontend
cd frontend
pnpm install
pnpm dev

# Programs
cd ../programs
anchor build
anchor test
