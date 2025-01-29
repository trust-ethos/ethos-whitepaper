---
cover: ../.gitbook/assets/Group 1000003181a.png
coverY: 0
---

# Litepaper

### First concepts

#### The Ethos Market

Each market is tied to an Ethos profile, which is connected to an Ethereum wallet. A market is intended to be attached to an identity that users want to speculate on the reputation for; it could be an individual user, a company or corporation, a DAO, or even an autonomous entity.

The amount of markets available will start limited and controlled by Ethos Labs as a means of focusing liquidity into specific markets and giving all users the best possible experience.

#### Trust percentages

Every market has a current Trust/Distrust score based on the current price of trust and distrust votes. This is intended to act as a proxy for how trusted or distrusted someone or something is.

At the start, the market starts at 50:50. Buying trust votes increases the price of trust votes and the overall score. This also lowers the price of distrust votes to provide equilibrium to the market.

{% hint style="info" %}
**A pragmatic example might be:** \
You see someone highly credible like Vitalik at a trust score of 35%.&#x20;

You believe Vitalik is more trustworthy than 35%, so you buy trust votes because you believe his current market price does not correctly reflect his trustworthiness.

You believe you can net a profit because his trust score will go up once the "trust market price" has been realized.
{% endhint %}

It's important to understand that these markets are **perpetual**, and do not resolve. This because trust can never truly be resolved at a point in time

However, you can imagine derivatives markets that could exist in the future resolve at certain points in time, ie. Vitalik will be above 80% before the end of 2025.

### Implementation & liquidity

Ethos Reputation Markets execute on an Automated Market Maker (AMM) smart contract, using a standard Logarithmic Market Scoring Rule (LMSR) algorithm to price two opposite positions. This is the same pricing algorithm used by Polymarket.

As an automated market liquidity is managed algorithmically rather than via traditional bid/ask spreads. Ethos Reputation Markets used a fixed liquidity control per market. These markets will continue to 'swing' with the same amount of volume, no matter how many total assets are locked. This has the following benefits:

* You are never "too late to the party." Your votes have the same impact as the first market participants.
* Markets respond quickly to changing sentiment. It does not require those with the largest holdings to shift positions before the market adapts.
* Nobody is required to add liquidity. There's no liquidity crunch as people exit the market. Despite offering a built in "short-like" position, these contracts cannot be short squeezed.

For future upgrades, the Reputation Market contract implements a graduate function that allows adoption of future algorithms and implementations, with agreement from the market owner.

Note that because Reputation Markets are not prediction markets and do not resolve, they are not "binary options" but lack a formal economic definition; then nearest would be a "binary perpetual."&#x20;

### Contrasts to Ethos.Network

Ethos.network and Ethos.markets work as independent but complementary products. The vast majority of people will have Ethos.network accounts but not a market on Ethos.markets. This is due to some constraints around Ethos.market's reputation market design:

* There is not enough liquidity in the world to support every user having their own Ethos market.
* Ethos.markets ONLY lets people speculate with money, and lacks other social signals like free reviews.
* A reputation market has pure financial upside and downside, and could muddy & conflate social signals of "I don't want to lose money" with "I don't trust this person" - something that's much more clear on Ethos.network

## Acknowledgements & Contributors

This concept was originally from a conversation we had with [@CL207](https://x.com/CL207), originally in late 2023 and then again in September 2024.&#x20;

Both CL and the Ethos team were inspired by what Friend.tech could be ([CL's thesis](https://www.egirlcapital.com/writings/181712053), [our thesis](https://x.com/0x5f_eth/status/1706341407672148477)) but it was missing one key part - you could only buy keys, you couldn't take the sell side. CL casually pitched the idea to us but wasn't sure how to implement it, so we did.&#x20;

He will always be considered an original contributor to the thesis.
