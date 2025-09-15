# Credibility Score

**Credibility Scores** quantify credibility indicators.

### Calculation

The Credibility Score algorithm will factor in a variety of weighted indicators. Indicators include relevant on chain actions, such as:

* number of vouchers, mutual vouches, and amount vouched
* mutual vouch duration and defection&#x20;
* credibility score of vouchers or reviewers
* average rating of your contributions on Ethos
* account ages of attestation

Weights do not need to be linear. For example, having 100 positive reviews may provide 2x more credibility than 10 positive reviews.&#x20;

Indicators and weights may be added, removed, or adjusted according to the [credibility-consensus.md](../governance/credibility-consensus.md "mention").

### Range

The range of the credibility score is currently 0 to 2800, with several different levels (subject to change)

0-799 - untrusted

800 -1199 - questionable

1200 - 1399 neutral

1400 - 1599 known 

1600 - 1799 established

1700 - 1999 - reputable

2000 - 2199 - exemplary 

2200 - 2399 - distinguished

2400 - 2599 - revered 

2600 - 2800 - renowned 

All wallets and attestations start at the default 1200 score, "neutral."

### Usage

Credibility scores are intended as an "at a glance" quick estimate of credibility across many domains. No single number can represent the complexities of one's reputation among that many groups and interactions. The score is simply a summary of sentiment as measured by social proof.

Different communities' needs may warrant additional weights and calculations. Ethos open protocol allows other dApps to define alternate scores using the same onchain records.

### Under the hood

The credibility score will be calculated using a combination of onchain Ethos data and offchain observations like existing social graphs. Eventually, the algorithm will be committed to the Ethos Smart Contract, with all details publicly verifiable.&#x20;
