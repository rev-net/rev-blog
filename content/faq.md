---
title: FAQs
---

# Frequently Asked Questions

## What are Revnets?

Revnets let anybody fairly launch a token for their company, project, or community, which is backed by a shared treasury.

Instead of using a fixed token supply, Revnets let anyone pay the treasury to make new tokens – but it gets more expensive to make tokens over time, pushing more demand to the market. Token holders can also redeem their tokens to get funds back from the treasury, but earlier redeemers get less, rewarding those who hold their tokens longer.

The price to make new tokens is a "price ceiling" – if the market price goes above it, people will pay the treasury, make new tokens, and sell those back to the market, stabilizing the price. Redeeming tokens is a "price floor" – if the market price goes below it, people will redeem their tokens, get funds back, and buy more tokens back, stabilizing the price. This makes the token price stable and predictable, helping people support the Revnet more confidently.

A Revnet can also set aside some tokens for a group of developers, a community stockpile, and/or anything else. Since new tokens are made continuously, it sets them aside continuously – if 20% is being reserved for a core team, then that team gets 20 tokens for every 100 tokens made.

All of these rules are set up ahead of time and can't be changed, meaning everybody knows what they're getting into before they buy into the treasury. A Revnet token can be used for governance, private chat rooms, in-app purchases, or anything else – all a Revnet does is provide a transparent, stable, and fair financial foundation to build a product, community, or organization on top of.

To learn more about the details, take a look at [Revnets 101](/post/revnets-101/).

## How do the tokens work? Can I use my own token?

Revnets issue ERC-20 tokens, meaning they'll be compatible with Uniswap and other popular tools. They're also `ERC20Votes` tokens, meaning you can use them for onchain governance with platforms like Tally (which uses Governor Bravo).

You can use your own token for a Revnet, but it must implement the [`IJBToken`](https://github.com/Bananapus/juice-contracts-v4/blob/main/src/interfaces/IJBToken.sol) interface.

## How are Revnets made?

Revnets are built on top of [Juicebox v4](https://github.com/Bananapus/juice-contracts-v4), which is a new work-in-progress update to the Juicebox protocol. Juicebox v4 mostly works like [Juicebox v3](https://github.com/jbx-protocol/juice-contracts-v3), which powers [juicebox.money](https://juicebox.money/).

Each Revnet *is* a Juicebox project, but with additional constraints – the project's rules must be a valid Revnet setup, and the rules cannot be changed once the project has been launched. Although the contracts are still changing, you can see the current code on [GitHub](https://github.com/rev-net/revnet-contracts/).

## What networks will Revnets be on?

We plan to launch Revnets on every network where Juicebox v4 is available. We'll be launching on Ethereum mainnet and Optimism first, other OP Stack L2s (like Base) shortly afterwards, and L2s like Polygon, Arbitrum, and Avalanche later on.

## What assets can Revnets raise funds in?

To start, Revnets will be able to accept ETH. We hope to expand this to other ERC-20s over time.

## What is $REV? What is $NANA? How do they relate to $JBX?

Although we're still figuring out the details:

- $REV is the token issued by the *Revnet Research Network* Revnet. This is the Revnet which supports the development of Revnets, as well as related tools and resources.
- $NANA is the token issued by the *Bananapus* Revnet. This is the first project on Juicebox v4, and supports the development of Juicebox v4. This network receives fees from projects on Juicebox v4, including other Revnets.
- $JBX is the token issued by the [JuiceboxDAO](https://juicebox.money/@juicebox) project, which is the first project on Juicebox v3 and receives fees from v3 Juicebox projects. It also governs JuiceboxDAO.

To learn more, read [$JBX, $NANA, and $REV](/post/tokens/).

## What projects are going to use Revnets?

Anyone will be able to make and use Revnets, and we're building an initial cohort of projects that are interested in using Revnets. Although all of this is still subject to change, there's a work-in-progress list on [HackMD](https://hackmd.io/uy7QlBAhQeurecDF_ice2g).

## How can I use Revnets?

We're working on a Revnet dapp, which is available at [revnet.app](https://www.revnet.app/). It's experimental for now, but we hope to polish the contracts and this interface within the next few months.

## Where can I learn more?

Come to our weekly Revnet workshop, each Thursday at 5 PM EST in the [Revnet Discord server](https://discord.com/invite/6Zr7Rtv6Ea).
