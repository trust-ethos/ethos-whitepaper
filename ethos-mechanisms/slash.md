# Slash

**Slashing** fines unethical behavior.

{% hint style="info" %}
Financial slashing is not currently live in the Ethos. It will be added at a later date.\
The exact parameters of how financial slashing works are subject to change before launch.
{% endhint %}

### Social Validation

In the Ethereum Proof of Stake consensus protocol ([Beacon Chain](https://ethereum.org/en/roadmap/beacon-chain/)), with sufficient staked Ethereum (currently 32Ξ), one may act as a validator. Validators verify the accuracy and security of transactions and receive rewards for their efforts. Validators may act as a "[whistleblower](https://www.blocknative.com/blog/an-ethereum-stakers-guide-to-slashing-other-penalties)" and highlight an inaccurate or insecure transaction for extra validation, with various rewards and fees.

### When to use Slashing

Slashing is intended to call out unethical behavior that the slashee has identified. This can be anything from rug pulling a project to failing to complete a previously agreed upon over-the-counter transaction.

There is no binary definition to when to use slashing, and voters should vote on the ethics of the behavior as opposed to if something is slash-worthy or not. There is no such thing as "throwing a slash out" like you might a trial.

Slashing is not a trial like in traditional judicial systems. It does not put someone in prison, is not used by government agencies, and does not have longstanding impacts to someone's livelihood. This means slashing does not require the same constraints and rigor that a traditional court system would.

### Slashing - Financial

Any Ethos participant may act as a "whistleblower" to accuse another participant of inaccurate claims or unethical behavior. This accusation triggers a 48h lock on staking (and withdrawals) for the accused.

The whistleblower requests human validation by pledging a nominal reward (bond) to validators. Validators vote to indicate if they found the claims valid. Validators are rewarded the same whichever way they vote.

If validators vote in favor of the whistleblower, they reward the whistleblower pledged to validators is reimbursed _from the amount staked by the accused._ This is the "slashing punishment," and it cannot exceed 10% of the total amount staked in Ethos (as of writing)

**This is the&#x20;**_**only**_**&#x20;way in which staked funds may be withdrawn without the explicit approval of the person staking those assets.** It is intended to be rare; most unethical behavior can be reported first by a negative review or unvouching.

Upon being slashed the accused has a 7d grace period before they may be slashed again.

### Slashing - Social

Ethos users can also create "Social Slashings" where instead of actual capital risked, they risk their own social capital in the form of their credibility score.

Whistleblowers request human validation by pledging a blond of their credibility score (subject to min/max based on difference between slasher and slashee's score).

### Slash voting mechanisms

Users must have an Ethos score of at least 1600 to slash someone else. Financial slashing can be used against other Ethos profiles, while Social slashing can be used on both Ethos profiles AND social accounts (like X.com)

Slashes occur over a 48 hour time period. Vote results in-app are blind as to prevent voter bias. Users are welcome to discuss during the voting period but discouraged from revealing their voting preference.

#### Vote weighting

Slashing uses weighted votes based on credibility score. This gives high credibility score participants more weight than new members who have less social proof.

#### Cooldowns & timers

To prevent spam and abuse, multiple cooldown timers are in place, such as

* Maximum number of slashes available at a given point
* A user may only slash one person at a time
* A user may only be slashed once at a time
* Users may not be slashed more than once in a given time frame
