# Noctis — Whitepaper

**Draft v0.1 — prepared 2026-09-20**
Status: DRAFT — token name, ticker, and final parameters to be confirmed before launch.

---

## 1. Abstract

Noctis is a community-driven utility token on the Solana blockchain designed around a single, non-negotiable principle: **holders must be rewarded**. Every holder who participates in the Rewards Vault earns a pro-rata share of the reward pool — automatically, transparently, and claimable at any time. No lock-in lotteries, no discretionary payouts.

## 2. Vision

Most tokens ask holders to believe. Noctis asks the protocol to prove it — rewards are enforced by on-chain mechanics, not promises. The goal is a token where holding and staking is, by construction, a yield-bearing position funded by real protocol revenue.

## 3. The Problem

- Typical memecoins and community tokens offer holders nothing but price speculation.
- "Reward" tokens on other chains rely on opaque, off-chain distributions that teams can pause, redirect, or abandon.
- High fees and slow settlement on legacy chains make micro-rewards impractical.

## 4. The Solution

Noctis is issued as an SPL token on Solana (Token-2022 program) and paired with an on-chain **Rewards Vault**:

1. **Stake** — Holders deposit tokens into the Rewards Vault.
2. **Accrue** — Rewards accumulate every epoch, pro-rata to each staker's share of the vault.
3. **Claim** — Stakers claim rewards at any time. No lock-up required (unstaking is always available).

### Where rewards come from

- **Genesis allocation:** 15% of total supply is seeded directly into the Rewards Vault at launch.
- **Protocol fee share:** A transfer fee of **2%** (Token-2022 transfer-fee extension) is levied on secondary trades; **100% of collected fees** flow into the Rewards Vault.
- **Buyback top-ups (roadmap):** A share of any future product revenue is used to market-buy tokens and top up the vault.

This makes rewards structural: as long as there is trading volume, the vault refills itself.

## 5. Token Overview

| Parameter            | Value                                    |
|----------------------|------------------------------------------|
| Name                 | Noctis                     |
| Ticker               | NOCTIS                           |
| Blockchain           | Solana                                   |
| Standard             | SPL Token-2022 (transfer-fee extension)  |
| Total supply         | 1,000,000,000 (1B, fixed — no minting)   |
| Decimals             | 6                                        |
| Mint authority       | Revoked at launch                        |
| Freeze authority     | Revoked at launch                        |
| Transfer fee         | 2% on secondary trades → Rewards Vault   |

## 6. Tokenomics — Distribution

| Allocation        | %   | Amount        | Notes                                        |
|-------------------|-----|---------------|----------------------------------------------|
| Public / Liquidity| 70% | 700,000,000   | LP on Raydium; LP tokens locked/burned       |
| Rewards Vault     | 15% | 150,000,000   | Seeded at launch; topped up by transfer fees |
| Team              | 10% | 100,000,000   | 12-month linear vesting, on-chain            |
| Marketing / CEX   | 5%  | 50,000,000    | Listings, partnerships, community incentives |

- **No presale.** Launch is public and fair via pump.fun bonding curve → Raydium migration, or direct Raydium pool creation.
- **LP lock:** Liquidity provider tokens are locked for a minimum of 12 months (proof published).

## 7. Technology

- **Solana** — sub-second finality and negligible fees make per-epoch micro-rewards economically viable.
- **Token-2022** — transfer-fee extension routes a fixed percentage of every trade to the Rewards Vault without custodial intervention.
- **Rewards Vault program** — a purpose-built Solana program handling staking, epoch accounting, and claims. Code will be published open-source on GitHub and independently audited before mainnet deployment of the vault. (If the vault audit is pending at token launch, staking activates the moment the audited program is deployed — the 15% seed allocation is held in a publicly visible multisig until then.)

## 8. Roadmap

| Phase | Milestone |
|-------|-----------|
| 1 — Launch | Token creation, fair launch, whitepaper + GitHub public, X community live |
| 2 — Liquidity | Raydium pool, LP lock proof published, Birdeye/DexScreener tracking |
| 3 — Verification | Apply: Jupiter strict list, CoinGecko, CoinMarketCap |
| 4 — Rewards Vault | Audit → deploy staking program → vault goes live, 15% seed deposited |
| 5 — Growth | Partnerships, CEX listings, buyback-funded vault top-ups |

## 9. Team & Transparency

- Core team identities and roles published on the project X account and GitHub.
- All treasury and vault wallets publicly labeled.
- No team tokens unlock before month 12; vesting schedule verifiable on-chain.

## 10. Risks & Disclaimer

- Crypto assets are volatile; rewards depend on trading volume and vault funding — **yields are variable and never guaranteed**.
- Smart-contract risk exists even after audit.
- This document is not financial advice and the token is not an investment product offering.
- Regulatory treatment of crypto varies by jurisdiction; participants are responsible for their own compliance.

---

*© 2026 Noctis. Draft for community review — feedback via the project's X account and GitHub issues.*
