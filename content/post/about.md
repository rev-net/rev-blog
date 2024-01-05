---
title: About Revnets
---

# About Revnets

_by Filip – originally shared on
[sim.revnet.app](https://sim.revnet.app/about.html)_

Let's say you want to build an open-source alternative to Google Maps. Unless
you want to build it by yourself, you'll need some type of organization.

- Something like an LLC or a C corporation could work, but you would have to
  deal with legal fees, paperwork, and management.[^1] These structures make
  sense for working with investors, but investment can have its downsides: after
  months of outreach and negotiation, you may be left with unfavorable terms or
  lose control of the project down the line. Investors might push you towards
  risky growth strategies, short-term goals, or selling the company.
- You could set up something more experimental like a DAO, but this comes with
  its own challenges – you have to figure out governance and onchain logistics
  before you even get started, and DAOs come with risks like governance
  takeovers that you don't want to worry about.
- You can try to make things work without a formal organization, but a lack of
  pre-determined rules and boundaries can lead to disputes later on. The risk of
  this happening makes people less likely to buy in.

Even if one of these options _did_ work, how would you attract and grow a
network of users to write reviews and label addresses?

We ran into this exact problem when building our own software projects: why
wasn't there a simple way to set up rules in advance, and automatically share
money with a network of supporters as it comes in?

## Our Solution

To solve this, we're building "Revenue Networks" or **Revnets**, which are a new
way to get your project started and fairly share money with your entire network
of investors, workers, and customers. Revnets are designed with a few key
principles:

1. Anyone who supports a Revnet should get some of its revenue, whether they're
   a worker, an investor, or a customer.
2. Revnets are owned by everyone in the network. Everyone interacts with a
   Revnet according to the same rules.
3. Those rules should be set in place when the Revnet is created, and impossible
   to change afterwards. Money can only come into or leave the Revnet as those
   rules allow, making scams and
   [rug pulls](https://www.coindesk.com/learn/what-is-a-rug-pull-how-to-protect-yourself-from-getting-rugged/)
   impossible.
4. Anyone can make a Revnet and use it for whatever they want. Revnets shouldn't
   depend on us or third parties to work.

To accomplish this, we built Revnets using
[smart contracts](https://ethereum.org/en/smart-contracts/) on Ethereum (a smart
contract is a computer programs uploaded to the blockchain). Our smart contracts
don't have an owner and will keep working as long as the Ethereum blockchain is
active.[^2][^3] This means Revnets will keep working, even if we stop supporting
them. Also, Revnets don't depend on legal enforcement – unless the contracts get
hacked, it's impossible for anyone to break a Revnet's rules.

## How Revnets Actually Work

When you make a Revnet, you pick which currency you want it to accept. Since
Revnets are built on Ethereum, ETH is the simplest option.[^4]

To represent a Revnet's ownership (and a claim on some of its revenue), Revnets
use tokens. Tokens are really just numbers stored on a smart contract – you can
just as well think of these as "points", "credits", or "options".

Let's return to our Google Maps alternative. We'll make a Revnet named
**MapNet** which accepts ETH and uses MPN tokens to represent MapNet ownership.

Anyone can pay MapNet with ETH to make new MPN. The price to make new MPN is
also called the **price ceiling**. At first, it costs 1 ETH to create 1 MPN, but
MPN will get more expensive over time, depending on the price ceiling's
_increase frequency_ (how often the price increases) and its _increase amount_
(how much the price increases).

Anyone can destroy their MPN to get back some ETH from MapNet. The amount of ETH
you can get back is also called the **price floor**. In the most basic scenario,
if you have 1% of the total number of MPN tokens and destroy them, you get back
1% of MapNet's ETH.

MapNet can also have a price floor tax, which means you would get back less than
1% of MapNet's ETH. That ETH you didn't get would stay in MapNet, raising the
price floor for everyone else. The price floor also increases as it gets more
expensive to make new MPN (as long as people keep making it). This is why
Revnets are 'up-only' – as long as network activity continues, the price floor
should continue to rise, backing the value of everyone's MPN.

The most you can lose is the gap between the price you bought MPN at and the
price floor. Over time, that gap should shrink, and eventually become profit.

MapNet will make MPN at the price ceiling until a
[Uniswap pool](https://support.uniswap.org/hc/en-us/articles/8829880740109-What-is-a-liquidity-pool-)
(trading market) forms between MPN and ETH. From that point onwards, while MPN's
pool price is between the price ceiling and price floor, MPN will be purchased
and sold in that pool. If MPN's pool price reaches the price ceiling or price
floor, the MPN supply will grow or shrink to meet that demand, keeping the pool
price between the ceiling and floor. This keeps MPN prices stable and
predictable, making people more confident in the token.

To boost early growth, MapNet can set up a **boost**. A boost sends some MPN to
a wallet address called the _boost operator_ for some time after MapNet is
created. For example: "for the first 100 days, when people buy MPN, send 10% of
it to our developer team's wallet".

MapNet can also pre-mint some MPN to that address when MapNet is created. These
tokens can be used as a budget to pay a for early development, but they can also
be used for staking rewards, an airdrop stockpile, or something else.

## Why it Works

- MapNet development needs some heavy lifting up front to get the basics working
  – the boost (and pre-mint) can be used to encourage early work from a team of
  developers.
- Because MPN gets more expensive over time, early MapNet supporters are
  rewarded for taking greater risk, and have more of an incentive to leave
  reviews, label addresses, and use the platform. If it grows, they win too.
- Holding MPN means you own part of MapNet – the more valuable MapNet becomes,
  the more valuable MPN becomes. This makes workers, investors, customers, and
  other MPN holders more likely to support MapNet's growth through referrals and
  word-of-mouth.
- Because of the price floor, the tokens can never lose all of their value. This
  makes Revnets safer to participate in.

But you need to be careful: the rules that control MapNet's price ceiling, price
floor, and the boost are locked in place once MapNet is launched. If your boost
or pre-mint is too large, it might feel unfair and make people less likely to
support the Revnet. If the price increases too quickly, it might cause liquidity
issues later on. To get a sense of how these options play out, experiment with
the [Revnet simulator](/).

Software companies sometimes use investor funding to make their product free, or
cheaper than its alternatives. Once their product has enough users, the company
will raise prices, often leaving users worse off than they were before.

Revnets take a different approach: nothing is free, but customers know exactly
what they're getting into. If the project grows, the network of people that made
that happen is rewarded for it. And if the project fails, losses are limited –
even in a worst-case scenario, people can always get some ETH back by destroying
their MPN.

We think that Revnets will work best for open-source software, decentralized
protocols, social networks, and platforms which rely on user-generated content:
a platform which fairly rewards its users can attract and retain people better
than one which doesn't.

If you want to talk through an idea, message us on
[Discord](https://discord.com/invite/6Zr7Rtv6Ea) or
[Telegram](https://t.me/revnet_eth).

## Further Reading

If you'd like to learn more:

1. Message us on [Discord](https://discord.com/invite/6Zr7Rtv6Ea) or
   [Telegram](https://t.me/revnet_eth). We'd love your input.
2. See our
   [yellow paper](https://raw.githubusercontent.com/rev-net/whitepaper/master/whitepaper/revnet.pdf)
   for an in-depth explanation of the Revnet's mechanisms.
3. The Revnet smart contracts are available on
   [GitHub](https://github.com/rev-net/revnet-contracts).
4. More Revnet writing is available on
   [revnet.eth.limo](https://revnet.eth.limo).

---

Using a revnet could carry significant legal and regulatory risk. Be sure to
consult an experienced legal counsel in your jurisdiction prior to usage.

[^1]:
    Depending on the nature of your project, your Revnet may require a legal
    entity. Talk to a legal expert about the relevant regulations in your
    jurisdiction before using them.

[^2]:
    Operating on Ethereum means users must pay gas fees to interact with
    Revnets. This can be expensive on Etheruem mainnet, but we're planning to deploy
    Revnets on [Layer 2 Networks](https://ethereum.org/en/layer-2/) where gas fees
    will be negligible.

[^3]:
    There could be smart contract exploits, or exploits in the Ethereum
    blockchain itself. Always do your research, and exercise appropriate caution.

[^4]: Revnets can accept and denominate prices in other currencies.

_Thanks to Jango, Mieos, KMac, Sage, Sofia, Hans, Grace, and Owen for reading
drafts of this._
