# Streamora

_Programmable payment streams for creators and DAOs on Solana_

## Summary

Streamora lets creators, freelancers, and DAOs set up real-time token streaming payments that unlock continuously instead of in lump sums. Payers can pause, top-up, or attach milestones, while recipients see funds accrue live in their wallet.

## Target users

Freelancers, DAOs, subscription businesses, and payroll teams

## Problem

Lump-sum crypto payments create trust issues and cash-flow mismatches between payers and recipients.

## Solution

A streaming payment protocol with programmable unlock schedules, milestones, and instant withdrawal of accrued balance.

## MVP features

- Create a token stream with start/end time and rate
- Recipient can withdraw accrued balance anytime
- Payer can pause, cancel, or top-up an active stream
- Milestone-based unlock requiring recipient proof-of-work upload
- Simple dashboard showing all active streams and balances

## Chains

Solana

## Tech

Anchor, Rust, React, TypeScript, Solana Pay, Wallet Adapter

## Category

Payments

## Why now

Real-time payment streaming is a proven primitive (Sablier, Superfluid) but underbuilt on Solana despite its low fees making micro-streams practical.

## Roadmap

- Add fiat off-ramp integration for recipients
- Support NFT-gated streams for token-gated communities
- Launch payroll product for crypto-native startups
