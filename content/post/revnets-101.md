title: Revnets 101

# Revnets 101

_by Jango – originally shared on
[HackMD](https://hackmd.io/_NO0S6VfQnOCBIUDlPS1-g)_

Revnets help you establish financial rules for your open source project, without
governance, ops, or management overhead.

Revnets are useful for:

- **Builders** who pour their time and resources into open source things they
  believe in.
- **Investors** who are looking to support open source projects with a clear
  understanding of risks and opportunities.
- **Networks and communities** using and contributing to open source endeavors.

## Parameters

A revnet is defined in sequential stages.

Each stage specifies the following parameters:

- Duration
- Price
- Boost
- Exit tax
- Buyback pool

A revnet also specifies a Boost operator and optionally a Boost premint once at
the time it is deployed.

## Duration

The amount of time a stage lasts for before the next stage takes effect.

A revnet's last stage remains in effect forever.

## Initial price

The number of $TOKENs that’ll be issued per 1 unit of a base currency received,
at the time the stage begins.

## Price increase rate

The rate at which the price increases.

The price increases predictably during each stage, allowing open, fair, and
predictable entries for anyone interested.

## Examples

- 1,000,000 $TOKENs per 1 ETH contributed, increasing 5% every 30 days.

- 1 $TOKEN per 1 USD worth of ETH contributed, 1% every 24 hours.

- 1 $TOKEN per 1 USDC contributed, no increases.

## Price Visualization

Revnet with a price starting at 1 $TOKEN per ETH contributed, increasing 5%
every 24 hours.

```
0.81450625 $TOKENs per ETH                            ----->
                                                      ↑
0.857375 $TOKENs per ETH                        ----->
                                                ↑
0.857375 $TOKENs per ETH                  ----->
                                          ↑
0.9025 $TOKENs per ETH              ----->
                                    ↑
0.95 $TOKENs per ETH          ----->
                              ↑
1 $TOKEN per ETH        ----->
                        0   24h   48h   72h   96h   120h
```

## Boost

The percent of newly issued $TOKENs that will be routed to a predefined
destination determined by the boost operator. The remainder is always routed to
the payer.

The boost also consists of an optional one-time premint to the boost operator at
the time the revnet is deployed.

## Examples

- 1,000 $TOKENs preminted 20% boost operated by your-multisig.eth to fund an
  initial treasury.
- 100% boost operated by your-onchain-gov.eth if all token issuance should be
  withheld.
- 0% boost for no priviledged issuance.
- 50% boost routed to a staking rewards pool, with no operator that can change
  this allocation.

## Boost Visualization

Revnet with a price of 1,000 $TOKENs per ETH contributed and a boost of 50%.

```
               --->  500 $TOKENs issued to the payer.
1 ETH paid ---|
               --->  500 $TOKENs issued to the boost.
```

## Boost Operator

The address that can change the destination of subsequent boost $TOKENs within
the predetermined percent.

The Boost operator can transfer this role to another operator at any time, or
revoke the role altogether to ensure the boost allocation no longer changes.

## Examples

- your-multisig.eth starts as the operator to have more flexibility over
  budgets, later transfered to your-onchain-gov.eth for more decentralized
  control, later rescinded so no changes can be made.

## Exit tax

$TOKENs are the only way to access a revnet's funds.

The exit tax intensity determines what percentage of funds that $TOKENs can then
access at any point in time, benefiting the remaining $TOKENs who can now each
be turned in for a larger share.

The intensity can range from 0 to 1, 0 being no tax.

```
                       total-funds                           intensity
access-per-$TOKEN = -----------------  * ((1-intensity) + --------------- )
                      $TOKEN-supply                        $TOKEN-supply
```

## Examples

With a total of 10 outstanding $TOKENs and 1 ETH in the revnet, 1 $TOKEN (10% of
supply) can access:

- 0 intensity => access 0.1 ETH (10% of the funds)

- 0.1 => 0.091 ETH (9.1% of the funds)

- 0.5 => 0.055 ETH (5.5% of the funds)

- 1 => 0.01 ETH (1% of the funds)

## Exit tax visualization

Revnet with an exit tax intensity of 0.5, a total of 10 outstanding $TOKENs, and
1 ETH in the revnet to start.

```
0.0736 ETH per next $TOKEN                             ------>
                                                       ↑
0.06729 ETH per next $TOKEN                       ---->
                                                  ↑
0.062346 ETH per next $TOKEN          ----------->
                                      ↑
0.0583 ETH per next $TOKEN       ---->
                                 ↑
0.055 ETH per next $TOKEN     -->
                               exit exit         exit exit   exit
```

## Buyback pool

If there exists liquidity in an AMM that offers a $TOKEN / ETH price better than
what the revnet offers for new mints, inbound revenues will be fulfilled by the
AMM instead of issuing new $TOKEN.

This buyback pressure fills the space between the ever-increasing price ceiling
from the issuance price and ever-increasing price floor from exits.

![image](https://hackmd.io/_uploads/H1KD2UE_a.png)

## Stages

A revnet is deployed with a sequence of stages specified up front.

Stages allow for timeboxed rules to incentivize participation.

## Example

**Stage 1 (fundraise)**: 72 days, 1 $TOKEN per ETH increasing 1% every 24 hours,
100 $TOKENs upfront and 50% boost to your-multisig.eth, 10% exit tax intensity.

**Stage 2 (execute)**: Forever after, 0.01 $TOKENs per ETH increasing 1% every 3
days, no more boost, 50% exit tax intensity.
