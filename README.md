# ChainPilot
![ChainPilot logo](assets/logo.png)

**Chat with your wallet: an AI agent that executes Solana transactions from plain language**

## Overview
ChainPilot is a conversational interface for the Solana blockchain. Instead of navigating DeFi dashboards, connecting menus, and confirming cryptic transactions, users simply type or speak what they want, like "swap 1 SOL for USDC" or "stake my SOL", and an AI agent turns that request into a real, user-confirmed on-chain transaction.

## Problem
Most people are intimidated by DeFi interfaces, wallets, and transaction signing. This complexity is one of the biggest blockers to mainstream Solana adoption, especially for crypto beginners and casual users.

## Solution
ChainPilot combines an LLM with the Solana Agent Kit to interpret plain-language chat commands, construct the corresponding transaction, show the user a clear preview, and only execute it after explicit confirmation and wallet signature.

## Features (MVP)
- Chat interface for wallet actions: swap, send, stake
- Natural language parsing into transaction intents using an LLM
- Transaction preview and confirmation step before signing
- Simple dashboard showing agent action history
- Pre-built integration with Solana Agent Kit for a fast MVP

## Tech Stack
- Solana Agent Kit
- Next.js
- OpenAI API
- Solana Web3.js
- Phantom Wallet Adapter
- Node.js

## How It Works

```
User (chat/voice)
      |
      v
Next.js chat UI -----> OpenAI API (parse intent)
      |                         |
      |                         v
      |                 Structured transaction intent
      |                         |
      v                         v
          Solana Agent Kit (build tx via Web3.js)
                      |
                      v
          Transaction preview shown to user
                      |
                      v
       User confirms + signs via Phantom Wallet
                      |
                      v
            Transaction submitted to Solana
                      |
                      v
        Action history dashboard updated
```

On-chain, ChainPilot does not introduce a custom program; it uses the Solana Agent Kit to compose standard instructions (token swaps, SPL/SOL transfers, staking) that are signed and submitted through the user's own wallet.

## Roadmap
- Add support for more DeFi protocols (lending, NFT trading)
- Introduce voice input and multilingual support
- Launch a safety/audit layer for high-value transactions

## Pitch
See our one-pager at [docs/pitch.pdf](docs/pitch.pdf) and the spoken pitch script at [docs/pitch-script.md](docs/pitch-script.md).

## Team
- [Name] — Role (placeholder)
- [Name] — Role (placeholder)
- [Name] — Role (placeholder)

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://cakeman0259-png.github.io/chainpilot/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.
