---
title: "PE4KS London 2026: What the Stable and Capital Summits Actually Settled"
date: 2026-11-23
description: "A 29-video, 11.5-hour digest of PE4KS London (Stable Summit IV and Capital Summit, 17–20 November 2026). On-chain FX funded by reserve income, the collapse of stablecoin distribution economics under MiCA and the GENIUS Act, the Bank of England's systemic stablecoin regime, netting as the binding constraint on atomic settlement, and the finding that 95% of tokenized-product defaults were operational rather than credit."
tags:
  - stablecoins
  - onchain fx
  - tokenization
  - cbdc
  - institutional finance
  - event recap
---

PE4KS ran four summits in parallel in London between 17 and 20 November 2026, under the pitch "the whole of onchain finance in one room. Four peaks, one pass." Twenty-nine videos were published, totalling 11 hours 27 minutes, split between **Stable Summit IV** and **Capital Summit**. This digest reads across all of them for the signals that survived the marketing.

The short version: the conversation moved from *"will institutions come?"* to *"the plumbing is live — what does it cost?"* Three things crystallised. First, on-chain FX is the highest-conviction new use case, and the funding model is **reserve income**, not token incentives. Second, stablecoin distribution economics broke, because regulation now blocks issuers from paying yield to holders, so yield has to be manufactured downstream in vaults. Third, tokenization is no longer the interesting problem — **legal claim, exit liquidity and redeemability** are.

## On-chain FX: reserve income replaces emissions

The keynote that the rest of the day kept referencing came from Curve Finance, arguing that non-USD stablecoin issuers keep burning incentives because they ignore their own balance sheet. Tether and Circle earn roughly four percent a year parking fiat in treasury bills. A sterling, euro or Swiss franc issuer can do exactly the same with local treasuries.

The arithmetic is the point. A one-million-pool GBP/USD market earns around £20,000 a year on each leg — roughly **£40,000 a year to fund liquidity, with no token emissions**. Where a pool must pay three to five percent but the issuer's TVL is only half the pool, the issuer earns about two percent, which is why the practical advice is to **partner with the USD issuer and share reserve income** so both sides can launch a sustainable market. Card payments gave the sharpest spread comparison of the summit: Visa and Mastercard FX runs **200–300 basis points**, on-chain execution runs **4–10 basis points**.

The FX panel pushed back on the incentive model. The Frankencoin association said secondary liquidity is its single largest cost line, above salary, and that crypto market makers run 15–20% watermarks — market making is a privilege, not a right, in traditional markets, and pure extraction in crypto. The TGBP issuer agreed the watermark needs to fall to six to seven percent before on-chain FX thrives. Both flagged that **99% of liquidity in non-USD stablecoins is protocol-owned** and nobody has cracked organic depth.

The best technical observation of the summit was that on-chain two-hop trades routed through USD are *more* efficient than direct off-chain pairs, because capital-in-transit disappears. Traditional FX forces you through a US correspondent bank with nostro/vostro accounts and T+2 settlement; on-chain it is one atomic transaction. The counter-view: about 90% of FX trades route through the dollar today, and the goal is to flip that toward 50% with direct GBP–INR and GBP–GCC pairs.

Commercial numbers came from Circle's stable FX platform, live on the Arc mainnet since 16 September with Visa, Mastercard and DTCC as validators. USDC has processed **$13 trillion** against a **$73 billion** market cap; Circle Payments Network is running **$14.1 billion, up 49% year-on-year**. Consumer app Pulsar reported 70 countries, roughly 10,000 active users, weekly growth near 50%, and rates described as "near Google rates."

## Distribution economics broke, and vaults are the work-around

The clearest thesis of the summit: an issuer keeps the interest on reserves, the distribution platform owns the user. That deal is dead. Under MiCA and UK rules an issuer **cannot pass yield to the end user, directly or indirectly**, which kills the "hold our coin, earn four percent" retail pitch.

Two workarounds were named repeatedly. Partner with a regulated asset manager who manufactures yield on-chain and distribute it through the platform. Or move to external accounts where users self-custody and deploy into vaults themselves. Sizing came from vault infrastructure providers: roughly **10% of all stablecoins are actively generating yield; 90% sit idle**, mostly on smart-contract wallets and exchange custody. Yield is described as the strongest acquisition *and* retention lever, especially in bear markets.

The institutional picture is that at least five teams inside a regulated platform can say no — compliance, security, finance, risk, accounting — and exactly one business person is trying to say yes.

Visa's Open Standard consortium and its OUSD stablecoin is the disruptive attempt at the same problem. Launched 30 September with a market cap just under $1 billion, it charges **no mint or burn fees and shares reserve income across consortium participants**. The contrast drawn on stage: Tether earned **$1.5 billion last quarter**, Circle **$680 million**, of which $300–400 million passed to Coinbase. That is extreme centralisation of reserve income, and Open Standard is explicitly a response to it.

There was unusual scepticism on the panel. Stablecoin market capitalisation is around $300 billion, with growth decelerating from 40–45% in 2025 to 3–4%. Only about **1% of existing stablecoin market capitalisation is payment-related**. In Europe, SEPA already works, so the question "is this a solution looking for a problem?" was put directly to the panel; the answer given was that the bottleneck is the off-ramp, not the rail. Expect consortium consolidation within 6–12 months, and launching a standalone stablecoin outside a consortium was described as "almost impossible" now.

Stablecoin payroll was the most concrete enterprise use case: 300 enterprises, five years of operating, and Europe's first government benefit distribution paid in a euro stablecoin. US payroll is tens of trillions annually, and stablecoin payroll is **1–2% of the flow**. Providers deliberately target contractors to sidestep payroll tax, and reconcile through a settlement layer so CFOs see one source of truth. The next product is funding payroll out of a tokenized money market fund.

## Liquidity, fungibility and the myth of the peg

The most original talk of the summit came from Clear. A stablecoin is not a dollar, it is a *wrapper* — a promise on a dollar carrying its own technological and counterparty risk. In the speaker's words, **"fungibility between stablecoins is more of a marketing argument than a reality."**

Supply has been flat this year while **volume is up roughly tenfold** — the industry is finally measuring flow, not float. Daily price deviation is measured in basis points, not dramatic depegs, though USDC fell 12% during the Silicon Valley Bank failure and a USD token dropped 35% via manipulation. The root cause is structural: **more volume than liquidity**, and the risk/reward of providing liquidity across so many stablecoins is too thin to justify. Nobody had built a way to *trade the spread*. Clear tokenises the gap between market rate and redemption rate so users hold the spread instead of eating it, with losses to spread estimated in the tens of millions of dollars daily.

The institutional liquidity panel landed on one distinction: **primary versus secondary market**. Primary liquidity is tied to the banking system and is legally at-par; access is whitelisted. Depth is not the problem — access is. Tether cleared **$7 billion of redemptions in 48 hours**, Circle billions in 2022, and Sky $500 million. The line from the panel: the depth is there, it is the access that is the issue.

Hard numbers: **99.9%+ of stablecoin TVL is USD-denominated, and the euro is 0.3% of the market.** The killer friction for institutional payments is that OCC-chartered coins do not trade at par against each other, and nothing fixes that without a clearing house. A shared-liquidity-layer model was praised for addressing exactly this.

Insurance is not the answer. Nexus Mutual pricing runs 50–100 basis points, but pays out only after a **depeg below 90 cents for seven consecutive days**. No product exists that guarantees instantaneous at-par redemption — the cost of parking capital against 10 seconds' notice exceeds anyone's willingness to pay.

## Settlement: netting is the whole ballgame

The most technically important exchange of the summit came from the intraday funding panel. Europe moves from T+2 to T+1 in October 2027, and that is the headline. The real constraint is netting.

DTCC netted **$2.2 trillion of transactions down to roughly $33 billion — a 60x reduction**. That is only possible because there is a settlement window enabling batch netting. Remove the window and $2.2 trillion is genuinely $2.2 trillion of cash that has to be moved and recycled, and that money does not exist in the financial system, because the market depends on purchases and sales self-financing one another.

The corollary: velocity of settlement needs velocity of credit. A broker acting as matchbook provides liquidity at zero cost only while it passes assets through. Force it to fund its own balance sheet and it stops providing liquidity.

Other realities named: **60–70% of banks have no wallet infrastructure**; many bank systems lack timestamps supporting hours and minutes; and Deutsche Bank launched its custody product during the summit week, handling 135 currencies. Checkout.com shipped settlement **acceleration** (T+2 to T+0) and a stablecoin settlement rail for weekend settlement, noting that remittance traffic peaks on weekends. Banks' DNA — tens of thousands of regulator reports, forensic dollar-level risk tracking — has to survive translation into atomic settlement, and these institutions cannot afford to fail.

Enterprise adoption framing was candid. SAP Pay renders on-chain balances into a standard bank statement so reconciliation is unchanged, with the transaction hash cascaded into the memo field. The stack was described as sitting past Windows 3.1 but not yet iOS. No enterprise of reasonable size wants self-custody. On tokenized deposits: **$4 trillion versus $240 billion for stablecoins, roughly 15x bigger**, and most of that $240 billion is a "stablecoin sandwich" — mint, move, redeem — where nobody holds a digital asset position.

## The Bank of England laid the clearest regulatory picture

The Bank of England gave the most concrete policy presentation of the summit, and the UK regime is further advanced than any comparable jurisdiction.

| Element | Detail |
|---|---|
| Statutory trusts | Two separate ones — backing assets for coin holders, and a second for wind-down costs |
| Redemption | Direct right, honoured **within 24 hours** |
| Central bank proximity | **30% of backing assets on the central bank balance sheet**, reduced from 40% |
| Liquidity backstop | Facility to repo backing assets in stress |
| Risk tool | Holding limits **dropped** in favour of temporary guardrails — an aggregate issuance cap of **£40 billion** |
| Timeline | Consultation June 2026, responses September, rules finalised end of 2026, FCA gateway closes 28 February 2027, authorisations October 2027 |
| Architecture | FCA on conduct, Bank of England on prudential; Treasury issues the systemic recognition order |

The stated vision is a **multi-money ecosystem** where cash, tokenized deposits, stablecoins and central bank money are interchangeable, with central bank money as the anchor that clears between them.

The deposit tokens panel added the monetary-policy angle, and made the sharpest structural point of the summit. Stablecoins as regulated are *narrow banks* — **no credit creation**. But regulation also forbids paying yield to holders, so holders move into vaults, and vaults lend. Net result: the two-tier system is rebuilt, unbundled — **stablecoins do the money, vaults do the credit creation**. Precedent exists: Sky and Maker ran 10-year US mortgages.

A wholesale CBDC provider argued for economics-led routing: banks will price a trade across central bank money, tokenized deposits and stablecoins purely on capital, liquidity and funding. Stablecoins will migrate to **problematic corridors** — places where nothing else works cheaply.

## "We are mainstream" — the capital markets stack

The Capital Summit panel's framing was that the theoretical era ended, and offered receipts.

- A **Robinhood** vault product on the Morpho stack went from zero to **$1 billion AUM in three months**
- **Morpho** at roughly $7 billion in deposits, Coinbase around $2 billion, crypto-backed loans at 53,000 unique users
- **Fasanara** with $300 million of on-chain fund representations used as productive collateral
- **Xoxo** with 1,500 assets, $1.1 billion AUM, $45 billion volume, live with NASDAQ, London Stock Exchange and Deutsche Börse, with 200 UK and European stocks launched that week
- **Steakhouse** with $5 billion in deposits and 32 employees — the moderator asked whether it was "a bank without capital rules," and the answer was that it is non-custodial and **any depositor can veto adding new collateral**

The recurring caveat: **tokenization does not remove credit risk.** The underlying credit sits off-chain. What changes is accessibility, programmability, composability, and above all collateral financing. The unlock is described not as yield but as cheaper, better, faster financing for assets previously unfinanceable. One number: roughly **$1 trillion of margin loans against stocks at about 10%, against under 5% on-chain**.

Liability was mapped cleanly across three layers: protocol (code, minimal and immutable), vault (risk curator underwrites collateral), integrator (front-end risk layer). DeFi lending is fundamentally a **repo market** — short-term funding that can spike to thousands of percent APY. Project finance, including the pitch to tokenize Chilean copper representing 27% of world output, does not fit that profile. Ten-year tenors against a five-year-old ecosystem is a mismatch.

## Risk: the most important panel of the summit

The room emptied for this session, which is itself a finding. Three methodologies collided.

S&P Global splits risk into two categories: traditional instruments moved on-chain, where the underlying credit drives risk and on-chain is an *operational overlay*, and genuinely novel DeFi market structure. Its new vault fault-risk product is a **relative ranking**, not a point-in-time rating. The honest constraint: thin trading data and short track records, so the method is to define an unwind scenario and compare markets against it.

The specialised rating provider delivered the panel's headline statistic, and it deserves wide circulation:

> **Over 80% of all tokens do not convey any ownership towards the underlying.**
> **95% of all defaults in tokenized products in the last two years were not attributable to a default of the underlying — they were operational and cyber-security risks.**

Their framework is **redeemability risk**: what can go wrong that prevents redeeming in full, in time, per the agreed terms. The case study is a "Frankenstein product" — one token representing a Cayman master fund with two feeder funds under different regulatory frameworks, sharing one liquidity sleeve. Same credit risk, **completely different redeemability risk**. And **60–70% of what is needed to underwrite tokenized products is not publicly available**.

Nexus Mutual's approach is code quality first, then operational security. Smart contract risk has hardened; operational security is now the dominant vector, and public information is no longer sufficient to underwrite it. They monitor every code release, track rapid TVL changes, and are testing AI agents watching unstructured data. Roughly $7 billion covered, fully on-chain balance sheet.

The allocator voice was the sceptic, and worth quoting at length: more data will not make investors better, because in 2008 it was not a failure of information — it was incentives and governance. Risk models should be built on losses, not wins. *"I don't think there has been systemic failure on the blockchain yet… we haven't been tested."* Biggest fear: headline APY of 13–18% being treated as risk-free. And KYC is becoming a honeypot, so push ZK proofs.

The collateral panel made the same point operationally. DTCC's tokenization service went live on 28 October. Falcon Finance accepts three versions of Nvidia as collateral for a synthetic dollar at roughly $2 billion TVL. The discriminator is **legal claim and perfected security interest** — a treasury has to be a treasury, on-chain or off. The protocol's own framing: *"USDT is not a dollar, it's an obligation of Tether."* Exit liquidity is the only question that matters. And the graveyard list is instructive: tokenized real estate ("the asset is highly liquid, nobody wants to buy it"), tokenized private credit with 30-day unwinds, and the historical precedent of BlockFi taking FTT and Serum as collateral, described on stage as absolute suicide.

## The best product spec of the summit

A 120-year-old UK asset manager launched the **first natively issued, FCA-approved tokenized fund**, and it is the blueprint others are reverse-engineering.

**The fund is the token and the token is the fund** — not a wrapper, so counterparty risk is familiar. The **golden source of truth for ownership sits on chain**: transfer it on a Saturday evening and legal ownership transfers on a Saturday evening, in the regulator's eyes. Issued out of BNY's new digital assets platform, with **T+0 redemptions up to 10% of NAV** via a credit facility, which does not exist in traditional funds. Stablecoin in and out, no off-ramp required. NAV published on-chain daily, with an indicative NAV every 15 minutes. The strategy is 50% government and 50% corporate bonds, BBB average, targeting about 2% above cash. A $10 million liquidity sleeve bootstraps the market, because crypto market makers have a 20%-plus cost of cash. Access is professional investors only for now.

The honest admission on scaling: *"I don't know how this scales over time."*

## Staking, block space, and Ethereum's institutional moment

Institutions moved from **26% to 35% of all staked ETH in the first half of 2026**. One operator holds about 6 million ETH, roughly 5% of supply, with 5 million staked — the largest single staking provider in the world.

The framing came from a recent post by Vitalik Buterin arguing that ETH is a store of value if it is money, that fee burning has not been the value driver people expected, and that chasing it conflicts with decentralization. The cleanest investment thesis offered: any asset can be a store of value; ETH's value is **ownership of the most decentralised network with the largest DeFi ecosystem on top**. Ethereum's moat is 50–60 billion in TVL (roughly 6x Solana), 10 years of zero downtime, 70–80% of tokenization, and post-quantum readiness pulled forward to 2027.

The uncomfortable finding came from Japan: institutions' first-choice network is **not Ethereum**, purely because competitors staff that market locally and Ethereum does not. Marketing, not technology. Tokenized stocks running on Solana, Hyperliquid and Robinhood Chain is a live competitive leak, and institutions reportedly start on Ethereum mainnet then move elsewhere once proven.

## Yield forensics: who actually pays you

The best "don't get rich slowly" talk decomposed yield into three buckets: real-world assets (treasuries, companies), crypto market income (borrowers, funding rates, fees), and **promotional rewards** — you can sprint, you can't sprint forever.

The worked example, all from the transcript. A prime USDT strategy pays 3% base and 8% on a particular venue, so the 5% delta is incentives. Borrowing a stablecoin at 4% to buy a token earning 5% collateral rewards and re-pledging is looping — subsidized demand with an unclear funding source for the rewards. A one-tap product advertising 12% APY hides **11x leverage**: $100 plus $1,000 of debt equals $1,100 of assets, $55 profit against $40 borrowing cost, $15 net, which is 15%. **When the borrowing rate reaches 5.5%, APY falls to zero. A 5% collateral depeg at 11x wipes out 55% of equity.** USDC reached 87 cents. Stream Finance, a fund of roughly $400 million, lost **$93 million** in October deleveraging, announced it in November, and was winding down a year later with no distribution to creditors.

The checklist offered: source, structure, capacity, behaviour under stress. Do not evaluate risk by APY.

A Swiss franc CDP protocol showed the disciplined version of the same exercise. Its liquidation mechanism is intentionally slow and oracle-free — the community is the oracle, with a Dutch auction on-chain — which suits RWAs because it works without price feeds or secondary liquidity. **98% of all S&P 500 ETF tokens locked in DeFi sit on this protocol.** A live governance proposal for SpaceX equity as collateral priced the market risk at a 30% reserve against a 19% worst drawdown since IPO, giving a **70% maximum LTV**, plus a **2% risk premium** covering four tail risks: company, issuer, smart contract, governance.

## Agentic payments: the next sandbox, and the first attack surface

The most quotable talk of the summit. The thesis: we will not authorise payments, we will prompt agents. And the agent — reading every email, clicking every link, running 24/7 — **cannot distinguish true from false**.

Researchers tested open-source models against the most prominent protocol in the category and found it **relatively easy to make an agent verify a mandate for one transaction and execute a completely different one.** The missing layers, ranked: limits and caps enforced at the signer level (easiest), identity — **know your agent is more important than know your customer** — liability apportionment across the chain, and verifiable decision logs so chargeback disputes can be settled.

The polemic: decentralization is over. With the Binance hack, roughly $6 billion was wiped from hot wallets and **$3 billion was recovered by centralized stablecoin issuers**. Crypto built the rails and now has a new owner. Agentic payments are the one frontier card networks will not allow, because delegating payment authorization to software breaks their model, so crypto rails get the sandbox first.

Enterprise corroboration came from a multichain issuer naming **agentic** as the fifth use-case vertical after payments, remittance, treasury and settlement, and noting it needs **non-custodial** infrastructure because travel-rule requirements make custodial agent payments painful. The proposed enterprise compromise is hybrid: self-custody up to $1,000–10,000 as a cash desk, custody above that.

## Aave, DeFi's P&L, and the macro hangover

Aave's founder ran the numbers: **$4 trillion in net deposits, $1 trillion in borrow volume, no back office, no settlement team, a few hundred lines of core code.** Kraken's parent bought AAVE on the open market, described on stage as a big bet on on-chain. Aave Labs acquired Avon for fixed-rate lending, aimed squarely at tokenized-asset users.

On the Clarity Act setback: it was not perfect, and could have brought tailwind — the GENIUS Act did exactly that for stablecoins. Its failure activated agencies to be proactive, with SEC guidelines on lending, borrowing, vaults and permissionless securities trading, UK DeFi guidance, and MiCA 2.0.

The allocators were the most honest voices in the room. DeFi was extremely tough through the first half of 2026, with a big pullback in April after the hacks and the 10 October collapse killing liquidity. The hot take: **the meme coin and launchpad casino has hurt crypto more than all of the hacks**, because it disillusioned normal users. Cost of capital: a large Asian allocator will not deploy below mid-teens net on market-neutral, large balance sheets in DeFi need only SOFR plus 20–40 basis points, nimble funds need 12% on USD and above 7% on ETH, and bitcoin-on-bitcoin is 5–6%. The question posed to the room: why put money on chain to do worse than your treasury bills? Roughly **30–50% of large funds lost their AUM**, with capital rotating to AI. On deal flow, one manager said they would cut nine of ten incoming proposals — adverse selection — and prefer high yield with low volatility and pain on redemption periods, because DeFi borrow-rate spikes happen multiple times a year and volatility on both legs is ruinous.

The long arc: crypto was born with native assets, the next five years are securities and tokenized assets, and the 50-year horizon is **funding abundance** — high-capital-expenditure, low-operating-expenditure infrastructure that banks cannot fund under Basel III, which DeFi and tokenization can.

## Bitcoin as macro history

The most idiosyncratic talk swept from Roman denarii through the Joachimsthaler, Potosi's 150,000 inhabitants, the Bank of England raising silver to buy gold in 1694, and Hayek's *Denationalisation of Money* of 1976.

The frame: every economy has an **unquestionable asset** as its cornerstone. Silver, then the dollar, then something. Bitcoin's two intellectual fathers are Hayek and William of Ockham, because Bitcoin is the simplest financial asset in existence, definable in five sentences: digital, unforgeable, peer-to-peer, decentralised governance, 21 million.

The best citation of the summit came from Hal Finney on 30 December 2010: *"Bitcoin cannot scale… The ultimate fate of Bitcoin is to be the asset that serves as a currency reserve for banks that will issue their own digital cash."* Which is, the speaker argued, precisely the treasury-company model — a reserve institution holding the most boring asset on earth, being inventive on the liability side until its liabilities become the world's assets. The oil-refinery analogy: crude meant waterproofing, cement and lighting for 70,000 years, until the fractional tower produced asphalt, diesel, kerosene and gasoline. Financial engineering on Bitcoin is that tower.

## Numbers that matter

| Metric | Value | Source |
|---|---|---|
| Stablecoin market capitalisation | ~$300 billion | Distribution panel |
| Payment-related share of stablecoin cap | ~1% | Open Standard |
| Stablecoins generating yield on-chain | ~10%, 90% idle | Vault infrastructure |
| Stablecoin TVL that is USD-denominated | 99.9%+ | Issuer panel |
| Euro share of stablecoin market | 0.3% | Issuer panel |
| Tokenized deposits vs stablecoin volume | $4tn vs $240bn (15x) | Enterprise panel |
| USDC depeg during SVB | −12% | Clear keynote |
| Tokens conveying **no** ownership of underlying | >80% | Rating agency |
| Tokenized defaults that were operational/cyber, not credit | 95% | Rating agency |
| Underwriting information not publicly available | 60–70% | Rating agency |
| DTCC netting efficiency | $2.2tn → ~$33bn (60x) | Prime broker |
| Robinhood vault on Morpho stack | 0 → $1bn AUM in 3 months | Capital Markets panel |
| Margin loans against stocks | ~$1tn at ~10%; under 5% on-chain | Vault curator |
| BoE backing assets on central bank balance sheet | 30%, from 40% | Bank of England |
| UK systemic stablecoin guardrail | £40bn aggregate cap | Bank of England |
| UK full regime live | October 2027 | Bank of England |
| Card FX cost | 200–300bps vs 4–10bps on-chain | Curve keynote |
| Institutions' share of staked ETH | 26% → 35% in H1 2026 | Staking panel |
| Stream Finance loss | $93m on a ~$400m fund | Asset manager keynote |

## Quotes worth keeping

- *"Market making is a privilege, not a right."* — Frankencoin association
- *"Fungibility between stablecoins is more of a marketing argument than a reality."* — Clear
- *"The depth is there. It's the access that's the issue."* — Risk tokenisation protocol
- *"Current stablecoins in their current existence are just furthering dollar dominance."* — Acceptance network
- *"The moment that window goes away, $2.2tn is $2.2tn of cash that has to be moved. And that money doesn't exist."* — Prime broker
- *"You are recreating a two-tier system: stablecoins do the money, vaults do the credit creation."* — Vault curator
- *"Everyone is a good curator until you're not."* — On-chain asset manager
- *"More data won't make us better investors. In 2008 it wasn't a failure of information — it was incentives and governance."* — Life insurer allocator
- *"We haven't been tested yet."* — Life insurer allocator
- *"Know your agent is more important than know your customer."* — Security firm
- *"The meme coin and launchpad casino has hurt crypto more than all of the hacks."* — Crypto fund manager
- *"Why would you put your money on chain to do worse than your T-bills?"* — Crypto fund manager
- *"Just because you tokenize something, you don't earn the right to be liquid."* — Fund issuer
- *"The ultimate fate of Bitcoin is to be the asset that serves as a currency reserve for banks."* — Hal Finney, 2010

## Overall outlook

PE4KS 2026 marks the point where on-chain finance stopped pitching tokenization as the innovation and started pricing the plumbing. Reserve income is emerging as the honest funding model for non-USD stablecoin liquidity, replacing emissions that no issuer can sustain. Regulation is doing the heavy lifting in both directions — the Bank of England's 30% central bank deposit requirement and £40 billion guardrail give the UK regime the most credible confidence framework anywhere, while MiCA's yield prohibition has permanently redirected distribution economics into vaults and curators.

The uncomfortable findings deserve more attention than the optimistic ones. If over 80% of tokens convey no ownership of an underlying, and 95% of tokenized-product defaults were operational rather than credit, then the industry's risk vocabulary is misaligned with where losses actually occur. If netting is what makes $2.2 trillion of settlement tractable, atomic settlement is not a free upgrade. And if 60–70% of what is needed to underwrite a tokenized product is not publicly available, institutional allocation will stay in the "dip a toe in the water" phase for longer than the headline AUM figures suggest.

Expect the next twelve months to be decided less by price and more by three boring questions: can a stablecoin be redeemed at par on a weekend, does the token carry a legal claim, and who is the counterparty when things break.

---

### Sources

All figures are as stated by speakers on stage and have not been independently verified. Transcripts are auto-generated, so names and numbers carry transcription error. One video, the compliance panel "Compliance Conditions for Institutional Allocation Onchain", has subtitles disabled and is absent from this digest. One keynote, the Curve Finance address, had only Swedish auto-generated captions; the Swedish tail was translated.

Video index — **Stable Summit IV**: [FX Flows](https://youtu.be/yYCgu9Pha-8) · [Stablecoin FX](https://youtu.be/qzwor9CsKCc) · [Curve keynote](https://youtu.be/ytQdxNideVM) · [Stablecoin Yield](https://youtu.be/xeu5GQbSGIA) · [Distribution Economics](https://youtu.be/DrY0qCgrNVw) · [Payroll](https://youtu.be/2ycNb7Wrx0c) · [Liquidity & Capital Efficiency](https://youtu.be/jp95mOuoxgM) · [Enterprise Settlement](https://youtu.be/c45vcm3j-XI) · [Intraday Funding](https://youtu.be/6ygQaKl2wTg) · [Deposit Tokens/CBDC](https://youtu.be/Z_7XbZstMaQ) · [Bank of England keynote](https://youtu.be/PQjEO9kUlrU) · [Clear keynote](https://youtu.be/ozmlpfAV3nE) · [Frankencoin keynote](https://youtu.be/5Ee_r8ToGOg) · [Scottish Banknotes](https://youtu.be/J9owfVC7EoA) · [Axis Eight keynote](https://youtu.be/jKqmrOx_MKg) · [Hacken keynote](https://youtu.be/oHTdYS21cGU) · [Aftermovie](https://youtu.be/z8WqUkmsKg0)

**Capital Summit**: [Capital Markets Stack](https://youtu.be/nr95vLU4jP8) · [Staking Economics](https://youtu.be/w3AFBX5ApbA) · [What After Bitcoin?](https://youtu.be/AwCMaGlIBXg) · [Asset Management & Fund Structures](https://youtu.be/fd4IN1B0gpw) · [First UK-Regulated Fund](https://youtu.be/bDC19a4CahI) · [Nieto Martin-Vares / Wilke](https://youtu.be/54IqEBHQUW0) · [Digital Asset Capital](https://youtu.be/6M5QVOpKKP4) · [TradFi/DeFi Converge](https://youtu.be/aTrumUlCp7A) · [Ratings & Underwriting](https://youtu.be/lFMwdh4rGCw) · [Collateral Terms](https://youtu.be/7_tbcNyaVAk) · [Compliance Conditions](https://youtu.be/hLzq0x25qRo) *(no transcript)*

**Promo**: [Introducing PE4KS](https://youtu.be/fMscN7_lrs4)
