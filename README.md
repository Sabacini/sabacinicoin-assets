# sabacinicoin-assets
Coin_Discription

# Technical Stack

From intent signals to real-world events: Mini App, research mechanics, DAO-style voting, and the infrastructure behind Sabacini.

---

## Project Story

### Phase 0 — Concept & Proof-of-Work

Time first, money later. We started with research, community calls, early design sprints, and a working Telegram Mini App prototype. An open task tracker and public progress logs document the work behind the idea.

### Phase 1 — Mini App MVP (Telegram)

Tap-to-Earn onboarding, basic profiles, RSVP flows, and survey modules.  
Objective: build an active community, measure real interest in IRL events, and filter out bots and low-intent traffic.

### Phase 2 — Scout Token (Research Layer)

A low-price, intent token used inside the Mini App to signal demand (votes, RSVPs, surveys).  
It is strictly a research and filtering tool, not an investment product, and can be implemented as a non-transferable or limited-transfer credit where feasible.

### Phase 3 — DAO Module (Lightweight Governance)

On-chain voting using Sabacini Coin on topics such as preferred regions, event formats, speakers, and partner selection.  
The current smart contract includes a simple proposal + vote system weighted by token balances, with execution performed by the project owner.  
Over time this can evolve into a full Governor + timelock model.

### Phase 4 — Fundraising & Setup

Pre-ICO and ICO of Sabacini Coin.  
Funds from the ICO are allocated to villa acquisition, renovation, yearly operations, events, marketing, and ecosystem development as described in the Whitepaper.  
Legal structuring, due diligence, and Mini App upgrades are tied to clear, milestone-based budgets.

### Phase 5 — Events Hub Launch

Weekly/bi-weekly talks, meetups, and parties in Italy.  
Priority entry via Sabacini Coin balances and NFT Event Passes, with on-site perks (e.g. free breakfasts, unlimited wine & snacks) and partner discounts (hotels, tours, car & yacht rentals).

---

## Technical Stack

### Network (target architecture)

- Primary environment at launch: **BNB Smart Chain** (BEP-20, ERC-20 compatible) for Sabacini Coin.  
- Future-ready for bridging/wrapping to other EVM L2s or TON if community demand and regulation allow.  
- Mini App: Telegram-native front-end; wallets via WalletConnect / TON Connect depending on network integrations.  
- Gas & fees: low-fee chains prioritized to keep interaction costs minimal.

### Smart Contracts (modules)

#### Sabacini Coin (BEP-20 / ERC-20 compatible)

- Fixed total supply minted at deployment (no further minting).  
- Transfer fee with four components: rewards pool, investment pool, marketing, and burn (deflationary).  
- Anti-whale protection via `maxTxAmount`.  
- Fee-exempt list for operational wallets (treasury, marketing, contract).  
- Built-in proposal + voting mechanism (1 address = 1 vote, weight by token balance); execution by owner.  
- Ownership via OpenZeppelin `Ownable`.

#### DAO Governance (future upgrade)

- Migration path to an OpenZeppelin Governor + timelock model once the community size and legal setup justify it.  
- Proposal thresholds, quorum, and voting periods tuned for actual on-chain participation.

#### Event / NFT Passes (ERC-721 / ERC-1155)

- NFT passes for priority entry, member-day perks, and special experiences.  
- Passes do not represent real-estate ownership or profit rights — only access and privileges.

#### Treasury & Milestones (off-chain + multisig)

- Project treasuries (ICO funds, investment pool, marketing funds) kept in multisig wallets.  
- Disbursements tied to DAO-approved milestones and published in open reports.

#### Scout Token (Research Layer)

- Minted or credited via the Mini App at a fixed low price.  
- Used for surveys, RSVPs, and early-stage experiments.  
- Non-investment utility with per-user caps and anti-bot logic.  
- Where implemented on-chain, designed as non-transferable or limited-transfer.

---

### Infrastructure

- **RPC / Nodes:** Ankr and/or reliable public RPC endpoints of the chosen chain.  
- **Explorer:** BscScan for BNB Smart Chain; additional explorers if bridging expands.  
- **Mini App:** Telegram Mini App with Tap-to-Earn, RSVP flows, survey engine, push notifications, and wallet connection.

---

## Security

- **Multisig:** 3-of-5 or higher for core treasuries, with at least one independent signer (advisor or auditor).  
- **Audits:** Third-party security review of Sabacini Coin and key modules before full ICO; follow-up reviews after major upgrades.  
- **Access control:** Ownership and administrative actions restricted; future role-based access via OpenZeppelin patterns as the system evolves.  
- **Operational security:** API rate limiting, bot protection for the Mini App, allowlists for critical operations, and strict key management policies.  
- **Transparency:** Public treasury wallets, quarterly reports, and open budgets linked to milestones.

---

## Stakeholders & Transparent Terms

### Sabacini Coin Holders

Priority entry to events, participation in proposal voting, eligibility for NFT Event Passes and on-site perks.  
No yield promises, no real-estate ownership.

### Event Pass (NFT) Holders

Access tiers for priority entry, member-day benefits, and potential future perks tied to events and partnerships.

### Core Team

Long-term vesting; no token sales from project wallets during the initial lock-up period (e.g. 12 months) as described in the tokenomics.

### Advisors

Legal, real-estate, and crypto experts with vesting schedules and cliffs aligned with long-term contribution.

### Local Partners

Hotels/guesthouses, tours, car & yacht services, and other local providers offering member rates and curated experiences.

### Community Moderators

Telegram/Discord coordination, event facilitation, and first-line support.

### Auditors & Legal

Smart-contract security partners and local property / legal counsel.

---

## Scout Token (Research Layer)

### Purpose

- Measure real intent before heavy spending.  
- Filter bots and low-quality traffic.  
- Size the audience for specific locations, formats, and ticket pricing.

### Use

- Participation in surveys and pilot programs.  
- RSVP for early test events and online sessions.  
- Early demand signals for villa location, event formats, and partnerships.

### Controls

- Per-user and daily caps.  
- Anti-bot and KYC/verification where necessary.  
- Non-transferable or limited-transfer design (where feasible).  
- Monthly public reports on usage and spending.

### Budget cap

Research budget strictly capped (for example, in the range of \$25k–\$50k) with public accounting and transparent burn-down.

---

## User Journey

1. **Open Mini App**  
   Create a profile, use Tap-to-Earn, and (optionally) connect a wallet.

2. **Join Research**  
   Acquire Scout Token at a low fixed price, complete surveys, and RSVP to pilots (with anti-bot and per-user caps).

3. **DAO-Style Voting**  
   Use Sabacini Coin to vote on key topics: preferred regions, event formats, speakers, and partners (according to the on-chain voting rules).

4. **Pre-ICO & ICO**  
   Participate in fundraising rounds that finance legal setup, villa acquisition, renovation, and ecosystem build-out, under transparent allocation rules.

5. **Launch of Events Hub**  
   Attend weekly/bi-weekly events in Italy with priority entry via Sabacini Coin balances and NFT passes, plus on-site perks and partner discounts.
