# Solana Token Explorer and Safety Checker

Search Solana tokens, see price, volume and liquidity, then click any row to run an instant safety check.

**Live demo:** https://froggy-coder0.github.io/token-tool/

## Why this exists

Thousands of new tokens launch on Solana every day, and many are scams. Most beginners only look at the price. This tool makes basic red flags easy to see in under a minute.

## Features

- Search tokens by name, symbol or address
- Market data: price, 24h change, volume, liquidity and age
- Sortable table that refreshes every 30 seconds
- One-click safety check with a simple risk score (green, yellow, red)
- Plain-language explanation for every check
- No wallet, no login, no install

## What the safety check looks at

- Mint authority (can the creator print new tokens?)
- Freeze authority (can the creator freeze your tokens?)
- Top 10 holder concentration
- Liquidity
- Token age

## Limitations

This is a basic check, not investment advice. It looks at only a few public signals and cannot catch every scam. Some results can be misleading, for example pump.fun tokens may show high holder concentration because of the bonding curve account. Always do your own research.

## Tech stack

HTML, CSS and JavaScript (no framework), Solana RPC, DexScreener API, hosted on GitHub Pages.

## Data sources

Market data from DexScreener. On-chain data from the Solana RPC.

## Ideas for the future

- Price charts
- Watchlist
- More chains (Ethereum, Base)
