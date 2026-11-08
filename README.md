# Bybit Heist Trace (Case TR-2025-0221)

A flow-of-funds investigation of three laundering branches from the 21 February 2025 Bybit hack ($1.4–1.5B, attributed by the FBI to North Korea's "TraderTraitor"). Every confirmed hop links to its Ethereum transaction so a reader can verify it.

## Files
- `index.html`: the report as a web page (embed it on your site or host it as-is)
- `Bybit-Heist-Trace-Report.pdf`: 7-page PDF of the same report
- `data/evidence_log.csv`: every hop, with full addresses, amounts, timestamps, transaction hashes and status
- `data/addresses.csv`: 15 addresses for screening (indicators), with roles

## What it shows
| Branch | Phase | Key finding |
|---|---|---|
| A | Conversion | Exploiter 1 → 2 single-use wallets → THORChain in 16 minutes; the deposit memo swaps 257.27 ETH to BTC address 191du9…wZmf |
| B | Liquidation | 98,047.84 ETH of stETH/mETH swap proceeds via ParaSwap, Uniswap and DODO within 71 minutes of the theft |
| C | Layering | Split from Exploiter 5, merged 2,083 ETH from six wallets, 1 ETH test, then 70 days of dormancy before May 2025 outflows |

Also documented: address poisoning against the launderers (about 98% of Exploiter 1's 4,418 transactions are incoming dust from look-alike addresses).

## Skills demonstrated
Blockchain tracing, cross-chain (THORChain memo decoding), laundering typologies, confidence grading, separating verified findings from reported claims, open leads, compliance recommendations, screening indicators.

## Method and limits
Data comes from Etherscan records and public reporting, collected 7 Nov 2026. Etherscan shows only the latest 25 transactions per address, so some activity may not be visible. The Bitcoin leg and three inputs to the merge wallet are listed as open leads. AI assisted with research, decoding and drafting; every confirmed figure ties to a linked transaction.
