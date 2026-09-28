# Streamora
![Streamora logo](assets/logo.png)

**Programmable payment streams for creators and DAOs on Solana**

## Overview

Streamora lets creators, freelancers, and DAOs set up real-time token streaming payments that unlock continuously instead of in lump sums. Payers can pause, top-up, or attach milestones, while recipients see funds accrue live in their wallet.

## Problem

Lump-sum crypto payments create trust issues and cash-flow mismatches between payers and recipients. Freelancers wait for large delayed payouts, and payers have no way to tie payments to ongoing work or progress.

## Solution

A streaming payment protocol with programmable unlock schedules, milestones, and instant withdrawal of accrued balance. Funds unlock continuously over a defined time window, and recipients can withdraw whatever has accrued at any moment.

## Features (MVP)

- Create a token stream with start/end time and unlock rate
- Recipient can withdraw accrued balance anytime
- Payer can pause, cancel, or top-up an active stream
- Milestone-based unlock requiring recipient proof-of-work upload
- Simple dashboard showing all active streams and balances

## Tech Stack

- **On-chain:** Anchor, Rust (Solana program)
- **Frontend:** React, TypeScript
- **Payments/UX:** Solana Pay, Wallet Adapter

## How It Works

Streamora combines an on-chain Anchor program with a React dashboard.

```
[Payer Wallet] --create/top-up/pause--> [Anchor Stream Program] --accrual--> [Recipient Wallet]
 |
 [Milestone Proof Upload]
 |
 [Unlock Trigger]
```

1. Payer creates a stream, specifying token, start/end time, and rate.
2. The Anchor program tracks accrued balance based on elapsed time.
3. Recipient can withdraw any accrued (unlocked) balance at any point.
4. Payer can pause, cancel, or top-up the stream while it's active.
5. For milestone streams, the recipient uploads proof-of-work before the next unlock is released.
6. The React dashboard reads on-chain state to show all active streams and balances in real time.

## Roadmap

- Add fiat off-ramp integration for recipients
- Support NFT-gated streams for token-gated communities
- Launch payroll product for crypto-native startups

## Pitch

- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team

- [Name] - Role - [GitHub/Twitter]
- [Name] - Role - [GitHub/Twitter]
- [Name] - Role - [GitHub/Twitter]

*Built for the Colosseum hackathon.*

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)
