---
title: About Revnets
---

# About Revnets

_by Jango – originally shared on
[revnet.eth.limo](https://revnet.eth.limo/about/)_

Revnets are revenue-backed networks of friends, investors, builders, donors,
fee-paying consumers, and anons around the world without need for governance,
management, permission, or any coordination.

Revnets are great for managing revenues and funding for open source projects and
internet networks by:

- Derisking bets for investors.
- Providing custom initial boost periods for builders.
- Rewarding today's retail consumers with tomorrow's network growth.

[Read the pitch to open source](https://revnet.eth.limo/4211056F-95FA-4459-9D53-ABC9E72ABB73/)

- Play with revnet simulations -> [sim.revnet.app](https://sim.revnet.app)
- Deploy your revnet -> [revnet.app](https://revnet.app)
- Ask questions or help others -> [t.me/revnet_eth](https://t.me/revnet_eth)
- Read the yellowpaper ->
  [revnet.pdf](https://github.com/rev-net/revnet-writing/blob/master/whitepaper/revnet.pdf)
- Learn through examples ->
  [sim.revnet.app/about](https://sim.revnet.app/about.html)

## Thesis

### Networks should own their own growth

Investors, builders, artists, storytellers, fans, donors, and fee-paying retail
consumers are all participants who help sustain a network and should all benefit
from revenue growth.

### Incentives should be clear to everyone, from startup to scale

Financially empowering both elders and newcomers within a framework of open,
voluntary participation supports a network's evolution by transparently
reflecting everyone's risks and contributions over time.

### Rent seeking should be inefficient

Given our world of uncertainty and opportunism, networks best sustain fruitful
participation when equipped with a reliable immunity instinct that efficiently
protects and rewards productivity.

## How it works

In practice, revnets implement Retailism:

_(The following is adapted from original
[Retailism](https://jango.eth.limo/9E01E72C-6028-48B7-AD04-F25393307132/) post)_

### What is Retailism

A business framework where wealth is exchanged programmatically over time from
newer participants to elder ones, and where investors and customers are treated
as alike participants. The “bag”, or the debt, is passed incrementally,
predictably, and ceremonially from one generation of voluntary participants to
the next, without need to orient towards retail extraction. Nothing is free, but
things reliably tend to become more and more free as a network grows over time.

### Why do we want it

Retailism is neither corporate capitalism, which defines generations through the
passing of a bag along Series A, B, and C investors, eventually selling to
retail who continues this cycle of amplifying narratives that pump and dump
bags. Nor is it corporate non-profitism or donationism, which obfuscate risks
and incentives altogether.

These are both increasingly fragile forms of production within internet-native
markets since their requisite delineation between capital and labor becomes
fuzzy – does an AI assist you or do you assist it? Does your crypto currency
work for you or do you work for it? Do your social networks serve you or do you
serve them? Hard to say, on the internet the act of investing and consuming are
often intertwined, and tail-risks of a network's failure are spread throughout
it.

Retailism hints at a progression of the status quo that can outcompete within a
broader capitalist marketplace of -isms by empowering the producer-consumer.

### Who is it for

Devs and communities will choose a Retailist business structure when they prefer
their outcome to be oriented towards maximizing the network's self-propagation
while minimizing the growth potential of any party with privileged access and
exploitable liabilites. They'll understand their work to have value while also
understanding a network's preference to work for itself once instigated.

### Why now

The Retailism framework is too fragile to exist if a rent-seeking fiduciary
facilitating the handling of money and the generational handoffs is required. It
can only outcompete as an encoded contract between network participants enforced
by a blockchain, a recent breakthrough.

It is now possible to encode this without any new code at all through onchain
protocols like Juicebox.

### How exactly does it work

For each network, the framework depends on only three variables:

#### 1. Ceiling increase rate

- _How much does the maximum cost to enter the network increase from one
  generation to the next, and how often are generations?_
- _This is encodable from the Juicebox protocol by kicking off the treasury with
  a $TOKEN issuance rate, and using a discount rate with funding cycles to
  consistently decrease the issuance rate of $TOKEN forever forward, tending
  toward zero in quantized chunks._

#### 2. Floor tax intensity

- _How much does the minimum value reclaimed from leaving the network increase
  each time?_
- _This is encodable from the Juicebox protocol using a redemption rate, leaving
  those $TOKEN holders who stick around with proportionally more as others
  redeem their $TOKENs for a chunk of the treasury._

#### 3. Boost

- _How will the startup work be valued? How much boosting should the network
  start with, favoring whom, and for how long?_
- _This is encodable from the Juicebox protocol using a premint of $TOKENS, and
  a reserved rate to devs and $TOKEN stakers effective until a future date when
  it is auto-removed via a scheduled funding cycle reconfiguration._

Once in motion, a network's revenue and investments should all be routed to its
revnet, the only way to access its $TOKENs.

If a liquidity pool with a better price than the current issuance rate exists,
inbound payments are routed to it instead. The issuance rate dampens upward
hyperbolic price manipulation of this pool by setting a price ceiling, and the
redemption rate dampens downward manipulation by setting a price floor that
increases with each subsequent redemption. These ensure participants a window of
opportunity for each generation, with a frame that can only progress upward over
time.

### More

[A Retailistic View on CAC and LTV](https://jango.eth.limo/572BD957-0331-4977-8B2D-35F84D693276)

[Modeling Retailism](https://jango.eth.limo/B762F3CC-AEFE-4DE0-B08C-7C16400AF718/)

[Retailism for Devs, Investors, and Customers](https://jango.eth.limo/3EB05292-0376-4B7D-AFCF-042B70673C3D/)

[Observations: Network dynamics similar between atoms, cells, organisms, groups, dance parties](https://jango.eth.limo/CF40F5D2-7BFE-43A3-9C15-1C6547FBD15C/)

## Implementation

Revnets and $REV are expressed using the
[$NANA fork](https://bananapus.eth.limo) of the Juicebox V3 Protocol and Uniswap
Protocol, on Mainnet, Optimism, and any number of other L2s.

## $REV Specifications

The Revnet Research Network (RRN) will develop tools for people to grow revnets
across the internet, including at [revnet.app](https://revnet.app) where new
revnets can be deployed and accessed. It will work with the JuiceboxDAO
community to deploy a forked Juicebox Protocol that runs as a $JBX-operated
revnet ([$NANA](https://bananapus.eth.limo/)), and will itself fund the
development of tools it builds through a revnet that issues $REV.

The $REV revnet will have the following specification:

| Property                      | Value                                                            |
| ----------------------------- | ---------------------------------------------------------------- |
| Initial price ceiling         | 1,000 $REV / ETH                                                 |
| Price ceiling's increase rate | 2.5% every 28 days                                               |
| Boost                         | 30,000 $REV upfront and 20% new $REV for 3 years to RRN multisig |
| Price floor's tax intensity   | 10%                                                              |

Once deployed, revnets cannot change their specification.

## Revnets - Season 1

See https://hackmd.io/@jango/revnets-1
