# Attest

**Attestation** ensures people are who they say they are.

In Ethos you attest by recording onchain the other ways you represent yourself (and your reputation) online. This can include digital identities, profiles, and wallets. Attestation is vital to prevent fraud and impersonation.&#x20;

### Price and Costs

Attestation is free; the price is nothing more than the required gas fees.&#x20;

Lying about your identity, however, is the most expensive action you can take on Ethos. Fraudulent attestation warrants Social Validation and Slashing (see: [vouch.md](vouch.md "mention")), which costs both reputation and staked Ethereum.

### Mutually Exclusive

No two Ethos Profiles can attest the same account or wallet.&#x20;

If one of your external accounts are already linked to another Ethos Profile, you may reclaim it automatically, without intervention or social validation. This action will be reflected as evidence on chain, which you can then use to "blow the whistle" on the fraudulent Ethos Profile pretending to be you, and trigger Social Validation.&#x20;

### Account Verification

Attesting external accounts requires demonstrating you have control over that account. Typically this requires emitting a message (tweet, post, etc) or updating a page (profile, commit) from that external account.&#x20;

This does mean that _group accounts_ (like a business's Facebook profile) for which multiple people have access may be easy to accidentally attest from the wrong Ethos profile.&#x20;

Support for various external accounts (Twitter, Facebook, Github, etc) will be added individually; this is not a blanket mechanism for attesting any link.

### Wallet Verification

Attesting a wallet requires signing a request. Most wallet providers make this easy, as this is a standard Ethereum specification ([EIP-712](https://eips.ethereum.org/EIPS/eip-712)). Ethos plans to support wallets for blockchains beyond Ethereum.

An Ethos profile can attest multiple wallets. This allows one to maintain security by keeping assets in different wallets with different keys, yet still represent all the assets within one Ethos profile. Any multi-sig wallets will require sufficient signing keys to sign the Ethos profile request, by definition. Ethos supports custodial and non-custodial wallets.

Ethos can support hardware or air-gapped wallets, though you'll need to know how to hash and sign requests specific to each type of these offline wallets.&#x20;

### Pseudonymity and Permanence

There is no requirement that attestation includes real names or identities. Real names do not confer any advantages to the [Credibility Score](credibility-score.md) calculation.

Attested accounts and wallets are recorded permanently on chain. Be careful. If you maintain separate identifies for operational security or privacy reasons, one slip up is enough to permanently "burn" that pseudonym.&#x20;

### Proof of Humanity

Ethos explicitly does not require [Proof of Humanity](https://worldcoin.org/blog/worldcoin/proof-of-personhood-what-it-is-why-its-needed). Brands, clubs, governments, bots, AI, and any other sentient creatures are able to develop and maintain a reputation, independent of their biological underpinnings.

### **Philosophy**

Reputation stems from communities. A profile on LinkedIn, Tinder, and Reddit will have very different connotations. Ethos should augment, not compete with, social apps like these. &#x20;

Reputation is multifaceted. The same person may have distinct reputations in multiple communities. Public information can still be privacy-sensitive; even if both Tinder and LinkedIn use your real name, few people want them intertwined.&#x20;

Reputation is also much more than identity. Pseudonymity provides benefits towards innovation the same way limited liability corporations do; by not putting "everything on the line," we promote experimentation and risk-taking. Ethos promotes the benefits of pseudonymity while also curtailing the drawbacks.

### Under the hood

Attestation is an open schema that is designed not to solely depend on Ethos infrastructure or smart contract.&#x20;

For linking accounts, an Ethos Oracle will validate an attestation link in a tweet, post, or profile. It will then send a transaction to the Ethos Smart Contract in an open format, list itself as a validator, and sign it.&#x20;

When linking wallets, anyone may submit a attestation payload to the Ethos Smart Contract signed by the wallet itself. The Ethos Oracle will provide a convenience function to sign and submit that payload using public wallet APIs and services (ex: [Metamask](https://docs.metamask.io/wallet/concepts/signing-methods/) signing).





