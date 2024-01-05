---
title: Modeling Retailism
---

# Modeling Retailism

_by Jango – originally shared on
[jango.eth.limo](https://jango.eth.limo/?id=B762F3CC-AEFE-4DE0-B08C-7C16400AF718)_

Retailist networks are deterministic, meaning all networks configured the same
way will have the same trajectory.

Each network is defined by fixed rules that change in fixed ways over a fixed
time frame known as a “generation”.

## Rules

Configuring a retailist network requires making three choices, and allows for
five additional optional choices:

##### Currency (optional)

_In which currency will the network store its value? ETH is used by default._

##### Initial issuance rate (optional)

_At the network’s onset, how many $TOKENs will be issued when it receives 1 ETH?
The default is 1._

##### Generation duration (required)

_How long is a generation? Everyone who joins the network during a generation
will receive the same amount of its $TOKENs when they pay ETH._

##### Generational tax rate (required)

_By what percent will the network's $TOKEN issuance rate be reduced between
generations?_

##### Exit tax rate (required)

- _How much less does a $TOKEN holder receive when accessing the network’s ETH
  immediately before any another $TOKEN holder does?_
- _This is specified as a percent that’ll be input into the formula
  `t / s * ((1-r) + r / s)`, where `t` is the network’s ETH balance, `s` is the
  total $TOKEN supply, and `r` is the tax rate. 0% suggests no tax, 100%
  suggests $TOKEN holders can never access the treasury because they’re taxed
  entirely._

##### Deploy tax (optional)

_The amount of $TOKENs to mint at the time of deployment for the deployer._

##### Boost duration (optional)

_The amount of time to apply a boost for, which pre-allocates a percentage of
newly issued tokens to some beneficiary as the network receives ETH._

##### Boost rate (optional)

_The percentage of newly issued $TOKENs to pre-allocate when the network
receives ETH during the boost period._

## Tensions

As it unfolds, each network will have a generation-over-generation growth rate
which describes how much ETH a network receives over time, and an exit rate
which describes what percentage of $TOKEN holders leave during each generation.

Tensions arise when considering how a network’s rules will affect these two
tendencies:

- networks with longer generations or a flatter generational tax rate leave room
  for more equal access over time to entice newcomers, but may lack energy from
  incumbent participants whose contributions are less recognized.
- networks with a larger exit tax reward more committed network participants,
  but may dissuade someone from making a commitment to the network in the first
  place since they’ll have less freedom to leave.
- networks with a deploy tax or boost can acknowledge the non-financial forms of
  participation which are often the subjects around which they revolve, but may
  also create governance burdens and spoil fair launch narratives.

Each network should consider its own unique circumstances when navigating these
trade-offs, keeping in mind that each new $TOKEN holder will eventually become
an elder one.

## Playground

Play around with these levers in this
[spreadsheet](https://docs.google.com/spreadsheets/d/1LC_zc2pfL4uUFLASz_OHf4wb7fFQyW1DDj31N6iOM9o/edit#gid=861230243).
Adjust the rules and set a few projections at the top to see how the outcome
changes.

- the first graph shows the amount of ETH each $TOKEN can be redeemed for at any
  point in time. Notice how this number can only go up or stay still, depending
  on how much motion (new entries, new exists) there is in the network.
- the second graph shows the amount of ETH that guarentees to back the last
  $TOKEN left in the network after everyone else has exited, at any point in
  time.
- the third graph shows the percent rebate that all payments into the network
  over time would yield if the $TOKENs the payment produced were immediately
  redeemed. Notice how the amount converges on a percentage, approaching from
  the bottom as preminted $TOKENs get diluted or from the top if no preminted
  $TOKENs are specified.
- the last shows the total value of all the $TOKENs allocated to boosting over
  time, if none were redeemed. Notice how even after boosting stops, the
  potential value of the allocated $TOKENs continues to rise as their redemption
  value rises.
- the table gives all context and calculations from which the graphs are
  derived. It shows how the network's dynamics change over time given the
  provided projections.

#### Related Links

- [Intro to Retailism](https://jango.eth.limo/9E01E72C-6028-48B7-AD04-F25393307132)
- [A Retailistic View on CAC and LTV](https://jango.eth.limo/572BD957-0331-4977-8B2D-35F84D693276)
