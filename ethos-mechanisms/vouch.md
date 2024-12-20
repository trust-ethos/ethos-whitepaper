---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Vouch

**Vouching** indicates a high degree of trust.&#x20;

In Ethos you vouch by staking Ethereum in an Ethos profile, a wallet address, or a social attestation. This fundamental core mechanism is how Ethos captures a network of trusted relationships. It represents the extent to which you are supported by allies and supporters, and thus strongly impacts credibility.

### Financial Stakes

Vouching, unlike [review.md](review.md "mention"), requires a backing asset: staked Ethereum (and in the future, other assets). This forces you to choose how you would allocate your trust and in what amounts and ratios. Does your entire network get equal trust, or would you vouch for some more than others?

The amount of Ethereum staked represents the magnitude of the trust placed in you. Ethos does not differentiate between one person who vouches you with 100Ξ or 100 people who vouch you with one Ethereum. This has many benefits, including that credibility is not a popularity contest; having a single strong supporter can be more impactful than dozens of weaker ties.&#x20;

However, the person you vouch DOES NOT HAVE DIRECT CONTROL over the backing asset. They cannot withdraw, spend, or re-allocate those staked funds.

### Impact on credibility score

In the Ethos webapp, credibility score is earned through vouching over time, as opposed to instantaneously. That credibility is currently earned over a 6 month bond.&#x20;

### Mutual Respect

When you vouch someone and they vouch you back, Ethos notes your mutual stake. This is commonly referred to as a [(3,3) relationship](https://research.tokenmetrics.com/3-comma-3/). Credibility and rewards for both of you are magnified. However, defecting from a mutual stake represents a greater indication that you might be untrustworthy; why would you turn your back on a friend who vouched for you?&#x20;

### Slashing

Slashing provides a mechanism by which unethical behavior may be identified, socially validated, and punished via fines and reduced reputation. Slashing can induce penalties of one's total stake in Ethos. Details in [slash.md](slash.md "mention").&#x20;

### Unvouch

You may withdraw your staked funds at any time by unvouching.&#x20;

You cannot modify the amount staked in a vouch without withdrawing the entire vouch.&#x20;

If you are mutually vouched (3,3) and unvouch, the person who was vouched can mark a vouch as "unhealthy" within 24 hours to signal to the network the vouch ended on poor terms.

### **Philosophy**

A long standing mutually beneficial relationship is the single best indicator of trust.&#x20;

People make mistakes. Penalties should be proportional; not everything is a “completely ruin your reputation” event.&#x20;

However, explicit deceit and defection _for the purposes of financial gain_ should have the potential to prompt strong financial disincentives.&#x20;

In the case where unethical behavior is sufficient to completely destroy one's reputation, all stakers will withdraw their funds and credibility will drop. This is the social equivalent of bankruptcy. Because Ethos is pseudonymous, it is always possible to start a new profile from scratch.&#x20;



