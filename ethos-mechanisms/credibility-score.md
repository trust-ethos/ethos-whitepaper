# Credibility Score

**Credibility Scores** quantify credibility indicators.

### Calculation

The Credibility Score algorithm will factor in a variety of weighted indicators. Indicators include relevant on chain actions, such as:

* number of vouchers, mutual vouches, and amount vouched
* mutual vouch duration and defection
* credibility score of vouchers or reviewers
* average rating of your contributions on Ethos
* account ages of attestation

Weights do not need to be linear. For example, having 100 positive reviews may provide 2x more credibility than 10 positive reviews.

Indicators and weights may be added, removed, or adjusted according to the [credibility-consensus.md](../governance/credibility-consensus.md "mention").

### Range

The range of the credibility score is currently 0 to 2800, with several different levels (subject to change)

<table><thead><tr><th width="191.7890625">Range</th><th>Description</th></tr></thead><tbody><tr><td>0 - 799</td><td>Untrusted</td></tr><tr><td>800 - 1199</td><td>Questionable</td></tr><tr><td>1200 - 1399</td><td>Neutral</td></tr><tr><td>1400 - 1599</td><td>Known</td></tr><tr><td>1600 - 1799</td><td>Established</td></tr><tr><td>1800 - 1999</td><td>Reputable</td></tr><tr><td>2000 - 2199</td><td>Exemplary</td></tr><tr><td>2200 - 2399</td><td>Distinguished</td></tr><tr><td>2400 - 2599</td><td>Revered</td></tr><tr><td>2600 - 2800</td><td>Renowned</td></tr></tbody></table>

All wallets and attestations start at the default 1200 score, "neutral."

### Usage

Credibility scores are intended as an "at a glance" quick estimate of credibility across many domains. No single number can represent the complexities of one's reputation among that many groups and interactions. The score is simply a summary of sentiment as measured by social proof.

Different communities' needs may warrant additional weights and calculations. Ethos open protocol allows other dApps to define alternate scores using the same onchain records.

### Under the hood

The credibility score will be calculated using a combination of onchain Ethos data and offchain observations like existing social graphs. Eventually, the algorithm will be committed to the Ethos Smart Contract, with all details publicly verifiable.
