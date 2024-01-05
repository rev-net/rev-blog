---
title: Revnets 1
---

# Revnets 1

_by Jango – originally shared on
[HackMD](https://hackmd.io/uy7QlBAhQeurecDF_ice2g)_

### Contents

- [Juicebox V4](#Bananapus-Juicebox-Network)
- [Revnet Research Network](#Revenue-Model)
- [Defifa Gaming Network](#Defifa-Gaming-Network)
- [Croptop Publishing Network](#Croptop-Publishing-Network)
- [Nance](#Nance)
- [Peel](#Peel)
- [Bannyverse](#Bannyverse)
- [Eden](#Eden)
- [Eth.Limo](#Eth.limo)
- [Pinnable](#Pinnable)
- [Planet](#Planet)
- [EthFS](#Ethfs)
- [Happy Gods](#Happy-Gods)
- [Breadfruit Onchain, LLC](#Breadfruit-Onchain-LLC)
- [Spacetime - MoonDAO's first DePrize](#Spacetime)

### Context

The following are hypothetical networks, all organized on a proposed
experimental $NANA Juicebox protocol fork, running as Revnets across EVM chains.
We are all in planning mode.

Read about revnets here, follow the links to browse various descriptons:
https://revnet.eth.limo.

The work around which each project's networks revolve vary widely, but they will
each run their revenues, investments, and incentives with similar guarentees.

Their implementation on $NANA using a Revnet is meant to streamline their
organizational and legal operations and expectations, and to make them more
accessible to investors and customers.

The people behind all these networks are on board, but have not all yet
finalized their desire to operate their project using Revnets on $NANA in
production. We're all going to play on testnets to try creating revnet
specifications we fully desire to make live for our respective projects. We
don't take fundraising, tokenization, and business models lightly.

Though builder consent is not required – these Revnets can stand besides other
forms of operations and even be fan-led without builder consent – broad
alignment is important, the lack of legitimacy or planned revenue from builders
may diminish an investor's confidence when choosing to support a network.

### Participation

This will be the working document for shaping each of these revnets. Builders
from each network will have edit access to this document and are encouraged to
shape things to their liking, drop links, borrow ideas from one another, and
leave questions for others to help answer.

We'll all be visting this document often to guide and ask questions. Rob, our
lawyer working with $REV, is around to discuss legal risk management strategies
for revnets. Investors are also welcome to drop by to help each revnet shape its
tradeoffs.

Our goal is to use the month of January of 2024 to play with concepts on
testnets, and get ready for production in February.

We'll use this Discord server for day-to-day comms:
https://discord.gg/mRcHm6f82t

### Specifications

Each revnet is specified in scheduled stages. Each stage enforces rules that are
set when the revnet is deployed. For example, a revnet could have one stage last
the first month, and next stage last the next year, and a last stage that lasts
forever after. Each stage must define the following:

| Property            | Description                                                                                                                                                                                      | Example                                                                                                                                                                    | Tension                                                                                                                 |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Initial price       | The number of $TOKENs that'll be issued per 1 unit of a base currency received, at the time the stage begins.                                                                                    | 1,000 $TOKENs / ETH, or <br> 10 $TOKENs / USD                                                                                                                              | None, this is cosmetic only.                                                                                            |
| Price increase rate | The rate at which the price increases.                                                                                                                                                           | 4.2% every 28 days <br> 1% every 24 hours                                                                                                                                  | Faster increases means larger $TOKEN access discrepancies between contributors over time.                               |
| Exit tax intensity  | Influences the amount of funds each $TOKEN can access when turned in.                                                                                                                            | 0.1                                                                                                                                                                        | Value must be between 0 to 1. Higher tax means less access to funds, but remaining $TOKENs benefit more from each exit. |
| Boost               | The amount of $TOKENS that can remain controlled, either with a premint or by reserving a % of issuance for some time.                                                                           | 1,000,000 $TOKENs upfront and 30% of new $TOKENs for 3 years to mymultisig.eth.                                                                                            | Bigger boost means more flexibility, but less predictability or access.                                                 |
| Boost operator      | The address that recieves the premint, and can re-route the boost allocation. <br><br> This is only set for the first stage. The operator can transfer this power, or relinquish it at any time. | If I'm the operator, I can change the 30% of new $TOKENs being routed to mymultisig.eth to be instead 15% routed to a staking rewards contract, and 15% to a burn address. | None. The boost operator can never change the preset boost % or duration, just the allocation.                          |

Read more in-depth descriptions here
https://hackmd.io/_NO0S6VfQnOCBIUDlPS1-g?view#/.

### Revnets

# Juicebox V4 (Bananapus)

_$NANA_

https://bananapus.eth.limo/ https://discord.gg/juicebox

<img src="https://hackmd.io/_uploads/SJyz3yHuT.png" alt="drawing" width="200"/>

## Purpose

Juicebox v4 is a way for networks of treasury-backed token holders (JB projects)
to relate across chains and forks.

##### It will be deployed as an experimental V4 Juicebox Protocol with the following considerations:

- Juicebox V3 fork, fully aligned with $JBX.
- On ETH and OP to start. ARBITRUM, BASE, and any other EVMs soon to follow.
- Native cross-chain project payment bridge, called Suckers, enabling projects
  to get their L1 project paid on various L2s while maintaining correct
  accounting for the treasury-backed tokens.
- Native staking-rewards bridge, called Tentacles, enabling projects to cross
  pollinate with other projects between chains and forks.
- “Funding cycle” => “ruleset”, and other name changes.
- Multiple rulesets can be queued in advance.
- Meta transaction support.
- Remove functionality that hasn’t proved useful (feegauge,
  ballotRedemptionRate).
- Projects will have the option to accept and store funds in ETH, DAI, USDC
  right away, and increasingly more over time.

## Revenue Model

- $NANA takes a 2.5% protocol fee from payouts and redemptions leaving the
  ecosystem across chains.

## $NANA Specifications

The $NANA revnet will play out in 1 stage with the following specifications:

| Property                      | Value                          | Reason                                                                                                                  |
| ----------------------------- | ------------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| Duration                      | Forever                        | No changes ever.                                                                                                        |
| Initial price ceiling         | 1,000,000 $NANA / ETH          | Arbitrary.                                                                                                              |
| Price ceiling's increase rate | 5% every 28 days               | Constant gradual nudge to contribute sooner than later. Arbitrary number.                                               |
| Boost                         | 50% of new \$NANA for 10 years | Sent to dao.jbx.eth, who can decide to use them for $JBX buybacks, growth incentives, or whatever else the DAO decides. |
| Operator                      | dao.jbx.eth                    | Operated by Juicebox DAO ($JBX).                                                                                        |
| Price floor's tax intensity   | 40%                            | Non-trivial tax to access liquidity.                                                                                    |

#### Notes & Questions

- here's how it was before @filipv
  ![image](https://hackmd.io/_uploads/rkE_204uT.png)

# Revnet Research Network

_$REV_ https://discord.gg/nT3XqbzNEr https://t.me/revnet_eth

<img src="https://hackmd.io/_uploads/SJy6TbSAn.png" alt="drawing" width="400"/>

## Purpose

Revnets are treasury-backed tokens that run autonomously with scheduled rules.
They issue tokens when they receive investments, revenue, or donations, and only
release funds from the treasury when someone turns in their tokens. Builders can
reserve a subset of new tokens as they're issued. Like Bitcoin, Revnets run on a
preset token policy that cant be changed. You can use revnets to express new
kinds of resiliant business models and to derisk founder-investor relations for
open source tools/networks.

revnet.eth is the operator of $REV. It is a research hub, dev shop, and
supporter of revnets. The goal of the fundraise is to fund revnet.eth with an
initial balance of $REV. It will use this $REV to develop tools and resources
that make Revnets more accessible, and to fund exciting projects derisked by
their revnets. Ocassionally, revnet.eth will exit from its positions back to the
$REV revnet.

Revnets are implemented as Juicebox projects configured to apply
[retailism](https://jango.eth.limo/9E01E72C-6028-48B7-AD04-F25393307132/).

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Fund revnet.eth with a $REV balance, used to bet on Revnets by funding the
  development of tools and resources that make them better and more accessible.

## Revenue Model

- Invest in derisked revnet-based opportunities.

## $REV Specifications

The $REV revnet will play out in 3 stages with the following specifications:

### Stage 1 | Fundraise

The goal of this stage is to raise $REV to revnet.eth that'll be used to build
revnet-enabling tools like revnet.app, and allocate to promising revnet-based
projects.

| Property                      | Value                                         | Reason                                                                                                                       |
| ----------------------------- | --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Duration                      | 72 days                                       | Arbitrarily a short while to fundraise.                                                                                      |
| Initial price ceiling         | 1,000,000 $REV / ETH                          | Arbitrary.                                                                                                                   |
| Price ceiling's increase rate | 1% every 24 hours                             | Constant nudge to contribute sooner than later. Arbitrary number.                                                            |
| Boost                         | 200,000,000 $REV upfront and 50% of new \$REV | Seed treasury, recognize initial research, development, and grants, fund the porfolio.                                       |
| Boost operator                | The revnet.eth multisig.                      | Currently consists of breadfruit.eth, filipv.eth, codalabs.eth, kmacb.eth, peacenode.eth, and dao.jbx.eth with a 3/6 policy. |
| Price floor's tax intensity   | 0%                                            | Tax-free access to raised funds for the boost to access liquidity.                                                           |

### Stage 2 | Execute

| Property                      | Value                              | Reason                                                                          |
| ----------------------------- | ---------------------------------- | ------------------------------------------------------------------------------- |
| Duration                      | 4 years                            | Arbitrary period to push the thesis with strong growth incentives.              |
| Initial price ceiling         | 10,000 $REV / ETH                  | Arbitrary. Start less than the first stage to incentivize the fundraise stage.  |
| Price ceiling's increase rate | 0.05% every 3 days (100x decrease) | Reduce but maintain the preference for earlier contributions. Arbitrary number. |
| Boost                         | 50% of new \$REV (no change)       | Continues to fund revnet.eth.                                                   |
| Price floor's tax intensity   | 10%                                | Access to funds not taxed very much for continued access to liqudity.           |

### Stage 3 | Reduce

| Property                      | Value            | Reason                                           |
| ----------------------------- | ---------------- | ------------------------------------------------ |
| Duration                      | Forever          | No more changes after this stage.                |
| Price ceiling's increase rate | 10% every 3 days | Tend toward 0 issuance faster. Arbitrary number. |
| Boost                         | 5%               | Reduce the preferential issuance.                |
| Price floor's tax intensity   | 40%              | Exits taxed more. Abitrary number.               |

The $REV network will be on mainnet, but issuance will also be available from
Optimism and Arbitrum.

# Defifa Gaming Network

_$DEFIFA_ https://discord.gg/3puFAeZZkE https://defifa.net

<img src="https://hackmd.io/_uploads/B1T-0WSRn.png" alt="drawing" width="200"/>

## Purpose

Defifa is a special configuration of Juicebox project that is in essence a game.
People mint from a preset number of teams, and then the teams decide how the
game's total pot will be split by agreeing on a scorecard. A socially agreed
upon rubric is proposed from the start -- i.e 60% of the total will go to those
who minted the winner of the next world cup, 30% to second place, 10% to third,
etc -- but the actual spread is a function of the players themselves agreeing on
the what happened, nothing else. The Defifa Gaming Network is a Revnet that
tries to auto incentivize improvements and propegation of Defifa games.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Develop and grow a platform for playing self-refereed prediction games.

## Revenue Model

- $DEFIFA will take a 5% fee from games played on the platform.

## $DEFIFA Specifications

The $DEFIFA mainnet revnet will have the following specification:

| Property                      | Value                                                           |
| ----------------------------- | --------------------------------------------------------------- |
| Initial price ceiling         | X $DEFIFA / ETH                                                 |
| Price ceiling's increase rate | X% every X days                                                 |
| Boost                         | X $DEFIFA upfront and X% of new \$DEFIFA for X years to xxx.eth |
| Boost operator                | xxx.eth                                                         |
| Price floor's tax intensity   | X%                                                              |

The $DEFIFA Optimism revnet will follow the mainnet's issuance schedule, and
will use a Sucker to pull revenues down to mainnet and distribute mainnet
$DEFIFA.

# Croptop Publishing Network

_$CPN_ https://discord.gg/ZSFkRjFkrA https://croptop.eth.limo

<img src="https://hackmd.io/_uploads/B1IMyGrR3.png" alt="drawing" width="400"/>

## Purpose

Croptop sites are self-serve personal websites accessible from .eth addresses,
with content feeds and revenue streams baked in. No wallet or credit card
needed, just a native Mac app. The Croptop Publishing Network is a Revnet that
tries to auto incentivize propegation of content published on Croptop websites.
Juicebox projects can give the Croptop contract permission to post NFTs to their
collections on their behalf, through which posters can add mintable content if
and only if they meet certain criteria the admin sets (price, total supply,
allowlist).

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Develop and grow a peer-to-peer publishing platform with built in revenue
  streams and content feeds.

## Revenue Model

- $CPN takes a 5% fee from mints made through the platform.

## $CPN Specifications

The $CPN mainnet revnet will have the following specification:

| Property                      | Value                                                     |
| ----------------------------- | --------------------------------------------------------- |
| Initial price ceiling         | X $CPN / ETH                                              |
| Price ceiling's increase rate | X% every X days                                           |
| Boost                         | X $CPN upfront and X% of new \$CPN for X years to xxx.eth |
| Boost operator                | xxx.eth                                                   |
| Price floor's tax intensity   | X%                                                        |

The $CPN Optimism revnet will follow the mainnet's issuance schedule, and will
use a Sucker to pull revenues down to mainnet and distribute mainnet $CPN.

# Peel

_$PEEL_ https://discord.gg/fAzKC76xGV https://juicebox.money

<img src="https://hackmd.io/_uploads/B1uN1GBR3.png" alt="drawing" width="400"/>

## Purpose

The Peel community of artisans designs, builds, supports, and hosts commercial
access points to the Juicebox ecosystem of projects, including the cononical
juicebox.money. Inso doing, it advocates for safe and useable consumer
experiences, including those of project owners, project participants, and
ecosystem client developers.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Maintain the juicebox.money site with useful project landing pages that give a
  general sense of what's going on, what the risks are, and how to get involved
  both as a participant and as an admin.
- Distribute useful shared tools, like subgraphs and sdk's, that make spinning
  up new fine-tuned end-to-end commercial-grade experiments easy.
- Help tell projects with their campaign's growth.

## Revenue Model

- $PEEL will sell access to its services and surfaces.

## $PEEL Specifications

The $PEEL mainnet revnet will have the following specification:

| Property                      | Value                                                       |
| ----------------------------- | ----------------------------------------------------------- |
| Initial price ceiling         | X $PEEL / ETH                                               |
| Price ceiling's increase rate | X% every X days                                             |
| Boost                         | X $PEEL upfront and X% of new \$PEEL for X years to xxx.eth |
| Boost operator                | xxx.eth                                                     |
| Price floor's tax intensity   | X%                                                          |

The $PEEL Optimism revnet will follow the mainnet's issuance schedule, and will
use a Sucker to pull revenues down to mainnet and distribute mainnet $PEEL.

# Nance

_$NANCE_ https://discord.gg/acq4JBc5eT https://nance.app

<img src="https://hackmd.io/_uploads/SyPIyfSR3.png" alt="drawing" width="400"/>

## Purpose

Nance is a platform for running cyclic, predictable governance processes for
networks of token holders who need to cordinate around onchain or offchain
actions. Pairs perfectly with communities operating scheduled Juicebox rulesets.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Develop the nance.app platform where communities can engage with their
  governance calendar.
- Work with communities to adapt their pre-existing communications systems to
  accomodate Nance processes and conveniences.

## Revenue Model

- $NANCE will charge a subscription fee to the governance processes it serves.

## $NANCE Specifications

The $NANCE mainnet revnet will have the following specification:

| Property                      | Value                                                         |
| ----------------------------- | ------------------------------------------------------------- |
| Initial price ceiling         | X $NANCE / ETH                                                |
| Price ceiling's increase rate | X% every X days                                               |
| Boost                         | X $NANCE upfront and X% of new \$NANCE for X years to xxx.eth |
| Boost operator                | xxx.eth                                                       |
| Price floor's tax intensity   | X%                                                            |

The $NANCE Optimism revnet will follow the mainnet's issuance schedule, and will
use a Sucker to pull revenues down to mainnet and distribute mainnet $NANCE.

# Bannyverse

_$BANNY_ https://banny.eth.limo/ https://discord.gg/7QCD4XuyTc

<img src="https://hackmd.io/_uploads/H1xnAmzOa.png" alt="drawing" width="200"/>
<img src="https://hackmd.io/_uploads/rkMARQfu6.png" alt="drawing" width="200"/>
<img src="https://hackmd.io/_uploads/r1hl1Ef_T.png" alt="drawing" width="200"/>
<img src="https://hackmd.io/_uploads/r1wJ14fda.png" alt="drawing" width="200"/>

Pilot: https://www.youtube.com/watch?v=BnCNiY19IFE

## Purpose

Bannyverse is the illustrative world of Banny and friends, across screens,
surfaces, and materials.

The banny.eth multisig will extend the existing conception of banny into
story-driven internet content and a story-driven NFT collection.

The multisig is sagekellyn.eth, mieos.eth, dao.jbx.eth, breadfruit.eth,
peri.eth, and lurkmoth.eth.

sagekellyn.eth will art direct and contribute throughout.

lurkmoth.eth will produce an initial series of 8 episodes, dropped every ~2
weeks, with shortform content in between. Watch the pilot linked above to get an
idea.

Alongside, breadfruit.eth peri.eth and mieos.eth are going to unshelf the pixel
banny collection. We will sell 4 options of naked Bannys from the $BANNY revnets
on Optimism and Mainnet, shown above:

Alien: 100 supply per chain, 1 ETH each. Pink: 1000 supply per chain, 0.1 ETH
each. Orange: 10000 supply per chain, 0.01 ETH each. Yellow: unlimited supply
per chain, 0.001 ETH each.

We will then start selling accessories that naked Bannys can buy, with sales
sent to the $BANNY revnet. It might or might not feel similar to the image
below. We will accompany the content storyline, and include seasonal drops in
small batches throughout the years, with occasional knods to currently trending
Juicebox stuff. Like a 10 edition of an ice cube accessory for banny in homage
to cryo, or a space suit as a knod to moondao.

![image](https://hackmd.io/_uploads/rkNWZNMuT.png)

breadfruit.eth is producing the treasury.

So much to play with from this starting point.

#### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Bring Banny to life.

## Revenue Model

- $BANNY sells NFTs, and can benefit from projects that contribute to
  bannyverse's CC0 IP.

The $BANNY revnet will play out in 3 stages with the following specifications:

### Stage 1 | Fundraise

The goal of this stage is to raise $BANNY to banny.eth that'll be used to create
the bannyverse through media, fabrics, and NFTs.

| Property                      | Value                                             | Reason                                                                                                                                                                       |
| ----------------------------- | ------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Duration                      | 28 days                                           | Arbitrarily a short while to fundraise.                                                                                                                                      |
| Initial price ceiling         | 1,000,000 $BANNY / ETH                            | Arbitrary.                                                                                                                                                                   |
| Price ceiling's increase rate | 5% every 24 hours                                 | Constant nudge to contribute sooner than later. Arbitrary number.                                                                                                            |
| Boost                         | 400,000,000 $BANNY upfront and 50% of new \$BANNY | Seed treasury, recognize everyone who has contributed to Banny's legacy thus far, including $JBX, sage, mieos, burtulla, peel, wagmi studios, and maybe some other airdrops. |
| Boost operator                | The banny.eth multisig.                           | They'll govern the boost and evolve governance as needed.                                                                                                                    |
| Price floor's tax intensity   | 0%                                                | Tax-free access to raised funds for the boost to access liquidity.                                                                                                           |

### Stage 2 | Execute

| Property                      | Value                              | Reason                                                                          |
| ----------------------------- | ---------------------------------- | ------------------------------------------------------------------------------- |
| Duration                      | 4 years                            | Arbitrary period to push the bannyverse with strong growth incentives.          |
| Initial price ceiling         | 10,000 $BANNY / ETH                | Arbitrary. Start less than the first stage to incentivize the fundraise stage.  |
| Price ceiling's increase rate | 0.05% every 3 days (100x decrease) | Reduce but maintain the preference for earlier contributions. Arbitrary number. |
| Boost                         | 50% of new \$BANNY (no change)     | Continues to fund revnet.eth.                                                   |
| Price floor's tax intensity   | 10%                                | Access to funds not taxed very much for continued access to liqudity.           |

### Stage 3 | Reduce

| Property                      | Value            | Reason                                           |
| ----------------------------- | ---------------- | ------------------------------------------------ |
| Duration                      | Forever          | No more changes after this stage.                |
| Price ceiling's increase rate | 10% every 3 days | Tend toward 0 issuance faster. Arbitrary number. |
| Boost                         | 5%               | Reduce the preferential issuance.                |
| Price floor's tax intensity   | 40%              | Exits taxed more. Abitrary number.               |

The $BANNY network will be on mainnet, but issuance will also be available from
Optimism and Arbitrum.

# Eden

_$EDEN_ https://discord.gg/9tuBRczQKk https://eden.art

https://cdn.discordapp.com/attachments/898291520975826964/1148703871443681410/prompt2prompt_1693940375_seed_1_.mp4

<img src="https://hackmd.io/_uploads/SJWrSfS03.png" alt="drawing" width="300"/>

## Purpose

Create, remix, and share AI art.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Build out the Eden platform.

## Revenue Model

- $EDEN is a donation button, there's no utility.

## $EDEN Specifications

The $EDEN revnet will play out in 2 stages with the following specifications:

### Stage 1 | Fundraise

The goal of this stage is to raise $EDEN to eden.breadfruit.eth that'll be used
to fund development.

| Property                      | Value                                           | Reason                                                                   |
| ----------------------------- | ----------------------------------------------- | ------------------------------------------------------------------------ |
| Duration                      | 72 days                                         | Arbitrarily a short while to fundraise.                                  |
| Initial price ceiling         | 1,000,000 $EDEN / ETH                           | Arbitrary.                                                               |
| Price ceiling's increase rate | 1% every 24 hours                               | Constant nudge to contribute sooner than later. Arbitrary number.        |
| Boost                         | 400,000,000 $EDEN upfront and 30% of new \$EDEN | Seed treasury, recognize everyone who has contributed to $EDEN thus far. |
| Boost operator                | The eden.breadfruit.eth multisig.               | It'll govern the boost and evolve governance as needed.                  |
| Price floor's tax intensity   | 0%                                              | Tax-free access to raised funds for the boost to access liquidity.       |

### Stage 2 | Persist

| Property                      | Value              | Reason                                                      |
| ----------------------------- | ------------------ | ----------------------------------------------------------- |
| Duration                      | Forever            | No more changes after this stage.                           |
| Price ceiling's increase rate | 0.05% every 3 days | Arbitrary number with small issuance changes.               |
| Boost                         | 90%                | Raise the boost to capture most of the donation afterwards. |
| Price floor's tax intensity   | 40%                | Exits taxed more. Abitrary number.                          |

The $EDEN network will be on mainnet, but issuance will also be available from
Optimism and Arbitrum.

# Eth.limo

_$LIMO_ https://eth.limo

<img src="https://hackmd.io/_uploads/r1z9GiZva.png" alt="drawing" width="300"/>

## Purpose

Proxy service for decentralized sites recorded on ENS.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Maintain and improve the eth.limo proxy.

## Revenue Model

- $LIMO is a donation button, there's no utility.

## $LIMO Specifications

The $LIMO revnet will play out in 2 stages with the following specifications:

### Stage 1 | Fundraise

The goal of this stage is to raise $LIMO to limo.breadfruit.eth that'll be used
to fund development.

| Property                      | Value                                           | Reason                                                             |
| ----------------------------- | ----------------------------------------------- | ------------------------------------------------------------------ |
| Duration                      | 72 days                                         | Arbitrarily a short while to fundraise.                            |
| Initial price ceiling         | 1,000,000 $LIMO / ETH                           | Arbitrary.                                                         |
| Price ceiling's increase rate | 1% every 24 hours                               | Constant nudge to contribute sooner than later. Arbitrary number.  |
| Boost                         | 400,000,000 $LIMO upfront and 30% of new \$LIMO | Recognize everyone who has contributed to $LIMO thus far.          |
| Boost operator                | The limo.breadfruit.eth multisig.               | It'll govern the boost and evolve governance as needed.            |
| Price floor's tax intensity   | 0%                                              | Tax-free access to raised funds for the boost to access liquidity. |

### Stage 2 | Persist

| Property                      | Value              | Reason                                                       |
| ----------------------------- | ------------------ | ------------------------------------------------------------ |
| Duration                      | Forever            | No more changes after this stage.                            |
| Initial price ceiling         | 10,000 $EDEN / ETH | Arbitrary.                                                   |
| Price ceiling's increase rate | 0.05% every 3 days | Arbitrary number with small issuance changes.                |
| Boost                         | 50%                | Raise the boost to capture more of the donations afterwards. |
| Price floor's tax intensity   | 40%                | Exits taxed more. Abitrary number.                           |

The $LIMO network will be on mainnet, but issuance will also be available from
Optimism and Arbitrum.

# Pinnable

_$PNN_ https://pinnable.xyz

<img src="https://hackmd.io/_uploads/SyWMBGHC2.png" alt="drawing" width="500"/>

## Purpose

An NFT-based IPFS pinning service.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Grow its userbase to better share the fixed costs.

## Revenue Model

- $PNN charges for storage.

## $PNN Specifications

The $PNN mainnet revnet will have the following specification:

| Property                      | Value                                                     |
| ----------------------------- | --------------------------------------------------------- |
| Initial price ceiling         | X $PNN / ETH                                              |
| Price ceiling's increase rate | X% every X days                                           |
| Boost                         | X $PNN upfront and X% of new \$PNN for X years to xxx.eth |
| Boost operator                | xxx.eth                                                   |
| Price floor's tax intensity   | X%                                                        |

The $PNN Optimism revnet will follow the mainnet's issuance schedule, and will
use a Sucker to pull revenues down to mainnet and distribute mainnet $PNN.

# Planet

_$PLANET_ https://www.planetable.xyz/

<img src="https://hackmd.io/_uploads/S1u-6KevT.png" alt="drawing" width="300"/>

## Purpose

An IPFS and IPNS based blogging service.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Make decentralized content more resilient and expressive.

## Revenue Model

-

## $PLANET Specifications

The $PLANET mainnet revnet will have the following specification:

| Property                      | Value                                                           |
| ----------------------------- | --------------------------------------------------------------- |
| Initial price ceiling         | X $PLANET / ETH                                                 |
| Price ceiling's increase rate | X% every X days                                                 |
| Boost                         | X $PLANET upfront and X% of new \$PLANET for X years to xxx.eth |
| Boost operator                | xxx.eth                                                         |
| Price floor's tax intensity   | X%                                                              |

The $PLANET Optimism revnet will follow the mainnet's issuance schedule, and
will use a Sucker to pull revenues down to mainnet and distribute mainnet
$PLANET.

## $PLANET Specifications

The $PLANET mainnet revnet will have the following specification:

| Property                      | Value                                                           |
| ----------------------------- | --------------------------------------------------------------- |
| Initial price ceiling         | X $PLANET / ETH                                                 |
| Price ceiling's increase rate | X% every X days                                                 |
| Boost                         | X $PLANET upfront and X% of new \$PLANET for X years to xxx.eth |
| Boost operator                | xxx.eth                                                         |
| Price floor's tax intensity   | X%                                                              |

The $PLANET Optimism revnet will follow the mainnet's issuance schedule, and
will use a Sucker to pull revenues down to mainnet and distribute mainnet
$PLANET.

# EthFS

_$FS_ https://www.ethfs.xyz/

<img src="https://hackmd.io/_uploads/BJKw5tODT.png" alt="drawing" width="300"/>

## Purpose

Upload files of all sizes to be stored onchain for use across smart contracts
and applications.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Make onchain file storage accessible.

## Revenue Model

- $FS is a donation button, there's no utility.

## $FS Specifications

The $FS revnet will play out in 2 stages with the following specifications:

### Stage 1 | Fundraise

The goal of this stage is to raise $FS to fs.breadfruit.eth that'll be used to
fund development.

| Property                      | Value                                      | Reason                                                             |
| ----------------------------- | ------------------------------------------ | ------------------------------------------------------------------ |
| Duration                      | 72 days                                    | Arbitrarily a short while to fundraise.                            |
| Initial price ceiling         | 1,000,000 $FS / ETH                        | Arbitrary.                                                         |
| Price ceiling's increase rate | 1% every 24 hours                          | Constant nudge to contribute sooner than later. Arbitrary number.  |
| Boost                         | 50,000,000 $FS upfront and 20% of new \$FS | Recognize everyone who has contributed to $FS thus far.            |
| Boost operator                | The fs.breadfruit.eth multisig.            | It'll govern the boost and evolve governance as needed.            |
| Price floor's tax intensity   | 0%                                         | Tax-free access to raised funds for the boost to access liquidity. |

### Stage 2 | Persist

| Property                      | Value              | Reason                                                       |
| ----------------------------- | ------------------ | ------------------------------------------------------------ |
| Duration                      | Forever            | No more changes after this stage.                            |
| Initial price ceiling         | 10,000 $FS / ETH   | Arbitrary.                                                   |
| Price ceiling's increase rate | 0.05% every 3 days | Arbitrary number with small issuance changes.                |
| Boost                         | 50%                | Raise the boost to capture more of the donations afterwards. |
| Price floor's tax intensity   | 40%                | Exits taxed more. Abitrary number.                           |

The $FS network will be on mainnet, but issuance will also be available from
Optimism and Arbitrum.

# Happy Gods

_$GODS_ https://discord.gg/zs7nqBes7u

<img src="https://hackmd.io/_uploads/S1zlEzH0n.png" alt="drawing" width="300"/>

## Purpose

Happy Gods is a 128 piece collection by Spanish digital painter Nacho Frades.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Distribute the Happy Gods NFT collection, fund the MoCDA in Spain, and
  contribute to the children's hospital.

## Revenue Model

- Sell art.

## $GODS Specifications

The $GODS mainnet revnet will have the following specification:

| Property                      | Value                                                       |
| ----------------------------- | ----------------------------------------------------------- |
| Initial price ceiling         | X $GODS / ETH                                               |
| Price ceiling's increase rate | X% every X days                                             |
| Boost                         | X $GODS upfront and X% of new \$GODS for X years to xxx.eth |
| Boost operator                | xxx.eth                                                     |
| Price floor's tax intensity   | X%                                                          |

The $GODS Optimism revnet will follow the mainnet's issuance schedule, and will
use a Sucker to pull revenues down to mainnet and distribute mainnet $GODS.

# Breadfruit Onchain, LLC

_$BREAD_

## Purpose

Breadfruit produces projects operating on the Juicebox protocol and the open
crypto internet.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Consult for projects who want to build successful open treasuries.

## Revenue Model

- $BREAD will participate in the treasuries it consults for.

## $BREAD Specifications

The $BREAD mainnet revnet will have the following specification:

| Property                      | Value                                                         |
| ----------------------------- | ------------------------------------------------------------- |
| Initial price ceiling         | X $BREAD / ETH                                                |
| Price ceiling's increase rate | X% every X days                                               |
| Boost                         | X $BREAD upfront and X% of new \$BREAD for X years to xxx.eth |
| Boost operator                | xxx.eth                                                       |
| Price floor's tax intensity   | X%                                                            |

The $BREAD Optimism revnet will follow the mainnet's issuance schedule, and will
use a Sucker to pull revenues down to mainnet and distribute mainnet $BREAD.

# Spacetime

_$SPACETIME_
https://docs.google.com/document/d/1Cgt__KLKSBl4cKfN5Boyjlz0n24XRrqoaeNm3HzjvQU/edit

## Purpose

A timing protocol for objects in cislunar space.

##### This project will be deployed as a project on Juicebox V4 ($NANA) as a Revnet to:

- Be the first instance of a DePrize and create a decentralized time standard
  for space.

## $SPACETIME Specifications

The $SPACETIME mainnet revnet will have the following specification:

| Property                      | Value                                                                 |
| ----------------------------- | --------------------------------------------------------------------- |
| Initial price ceiling         | X $SPACETIME / ETH                                                    |
| Price ceiling's increase rate | X% every X days                                                       |
| Boost                         | X $SPACETIME upfront and X% of new \$SPACETIME for X years to xxx.eth |
| Boost operator                | xxx.eth                                                               |
| Price floor's tax intensity   | X%                                                                    |

The $SPACETIME Optimism revnet will follow the mainnet's issuance schedule, and
will use a Sucker to pull revenues down to mainnet and distribute mainnet
$SPACETIME.
