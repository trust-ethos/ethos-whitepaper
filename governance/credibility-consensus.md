# Credibility Consensus

For the reasons described in Ethos Governance Principles, the Ethos [credibility-score.md](../ethos-mechanisms/credibility-score.md "mention") is defined by community consensus. During the Early Access period of Ethos, the way to interact with the credibility score is using Contributor XP, which are distributed network contributions to Ethos. This empowers and encourages the primary users of Ethos to be the ones who determine how credibility is measured through our in-house Credibility Score.

Measuring credibility will be inherently difficult, and everyone will have their own differing opinion on how to weight what goes into calculating that credibility. It's important to understand that during the Early Access period, the goal is to push Ethos' credibility model forward _collectively,_ through _consensus._ The initial scoring model is likely to overvalue some parameters, undervalue others, and completely miss parameters the team hasn't yet thought of. The Early Access period allows us to collectively define that as a community and make sure we optimize the scoring system before Ethos progresses to general availability.

With this in mind, during the Early Access period we have two mechanism that will be introduced to govern the credibility score via consensus:

### Weekly Votes

{% hint style="info" %}
Weekly voting is not currently live in the Ethos Network. It will be added at a later date.
{% endhint %}

Every week, Ethos participants will have the opportunity to vote on two things.

* This week's current proposal
* Which proposal should be voted on next week.

Ethos participants will use their points that they are allocated for network activity each week to vote on each of these. A proposal has 3 options - agree, disagree, or abstain and requires 51% approval from voters to be ratified.&#x20;

The leading proposal at the end of the weekly epoch that was voted on will then be put up for vote the following week. Ethos participants will have to choose whether they want to allocate their points to current proposal outcomes vs the ability to vote and participate on future proposals.

Upon the outcome of the current week's proposal, the credibility algorithm will be modified accordingly. In the Early Access phase, this will be done in a centralized manner by the Ethos team, who will manually make the tweaks. This enables full extensibility of the model so that we can introduce new ways to measure credibility as we work together to get the algorithm to true consensus.

### Vote Proposals

Every week during the Early Access period, the Ethos team will author 3 vote proposals for how to modify the current credibility score. Ethos network participants will also be able to create their own vote proposals, which will last over the period of 3 weekly epochs before disappearing.&#x20;

Proposals must have clear definition to the modification of the algorithm, as an example:

* Weight "number of vouchers" by 10% less
* Change the algorithm for "defection score" from nlog(n) to n!&#x20;
* Introduce a new measurement, the value of vouchers that are 1 hop away and weight them along a specified algorithm

Points used to vote for proposals are reset at the end of the weekly epoch and must be recast.

The top proposal is then voted on the next week.



