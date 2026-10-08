# ChainPilot

_Chat with your wallet: an AI agent that executes Solana transactions from plain language_

## Summary

ChainPilot lets users type or speak natural-language requests like 'swap 1 SOL for USDC' or 'stake my SOL' and an AI agent translates this into real on-chain actions using an existing agent toolkit. It removes the need to understand DeFi UIs or smart contract code, making Solana accessible to total beginners.

## Target users

Crypto beginners and casual Solana users who find DeFi interfaces confusing

## Problem

Most people are intimidated by DeFi interfaces, wallets, and transaction signing, which blocks mainstream adoption.

## Solution

An AI agent built on an existing Solana agent framework interprets chat commands and safely executes transactions with user confirmation.

## MVP features

- Chat interface for wallet actions (swap, send, stake)
- Natural language parsing into transaction intents using LLM
- Transaction preview & confirmation step before signing
- Simple dashboard showing agent action history
- Pre-built integration with Solana Agent Kit for quick MVP

## Chains

Solana

## Tech

Solana Agent Kit, Next.js, OpenAI API, Solana Web3.js, Phantom Wallet Adapter, Node.js

## Category

AI

## Why now

LLM agent frameworks for Solana (like Solana Agent Kit) have matured enough that a small team can build a working conversational wallet in a weekend.

## Roadmap

- Add support for more DeFi protocols (lending, NFT trading)
- Introduce voice input and multilingual support
- Launch a safety/audit layer for high-value transactions
