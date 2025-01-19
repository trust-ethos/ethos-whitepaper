# Bug Bounty

## Guidelines

### **Ethical Standards**

**The Ethos bug bounty aligns with our mission to reward ethical behavior. Although we outline guidelines and rules, the ultimate consideration in our bug bounty program will be: did you behave ethically?**&#x20;

**We cannot foresee every possibility, and although security researchers are the best at breaking rules, we reserve the right to deny or reduce participation or benefits due to ethical concerns.**

Specifically:

* Adhere to ethical standards and legal guidelines. Any actions that compromise the integrity, privacy, or availability of systems beyond what is necessary for testing are strictly prohibited.
* No harm: Ensure that your testing does not negatively impact users or infrastructure.
* Do not threaten, blackmail, dox, or otherwise create a negative environment for Ethos staff or users.
* Do not communicate with the Ethos staff or users outside of designated vulnerability reporting channels.
* Bug bounty reward edibility is ultimately up to the discretion of Ethos staff and any bug bounty management services.&#x20;

### **Scope and Testing Environment**

**Web Services**

* When possible, conduct tests in test environments only.
* Denial of Service attacks are prohibited against app.ethos.network.
* Avoid testing with external dependencies and third-party systems not controlled by Ethos, such as:
  * Twitter / X
  * Cloudflare
  * Intercom
  * Alchemy
  * Moralis
* Notify Ethos staff if you will be conducting tests that may lead to increased load. If your tests increase infrastructure costs or cause Ethos to hit API rate limits, then this is sufficient reason to disqualify any bug bounty rewards.&#x20;

| Service | Production ❌      | Test Environment ✅        |
| ------- | ----------------- | ------------------------- |
| web     | app.ethos.network | testnet.ethos.network     |
| echo    | api.ethos.network | api.testnet.ethos.network |

**Smart Contracts**

* Replicating tests on public mainnet is prohibited. All testing should be conducted on local forks of either testnet or mainnet. If necessary, notify the Ethos team before testing on base sepolia.

### **Responsible Disclosure**

* Do not publicly disclose vulnerabilities before they are resolved.
* Do not discuss (publicly or otherwise) any aspect of a submitted vulnerability before resolution.
* Use private, official reporting channels to submit your findings. Ie, Ethos public discord does not qualify.
* Never exploit a vulnerability or threaten to do so.
* Do not attempt to rescue funds without explicit written consent.
* Publicly known bugs or bugs reported in a previous audit are not eligible.
* Do not try to cajole Ethos regarding severity or payment.
* You may publish details about your submission after resolution or a maximum of 30 days.

## Report a Vulnerability

| Scope           | Managed By | Submit Via                                                                                                                   |
| --------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Web Services    | Ethos Labs | email [support@ethos.network](mailto:support@ethos.network)                                                                  |
| Smart Contracts | Sherlock   | [https://audits.sherlock.xyz/bug-bounties/pre/15?t=submission](https://audits.sherlock.xyz/bug-bounties/pre/15?t=submission) |

Address urgent issues or questions to: [support@ethos.network ](mailto:support@ethos.network)

Submissions must include:

* Clear explanation of the vulnerability
* Reproduction instructions or working Proof of Concept (PoC)
* Impact assessment on users and platform
* One vulnerability per report
* English language only

## Rewards and Disputes

### Web Services

| Severity                                      | Maximum Rewards       |
| --------------------------------------------- | --------------------- |
| <mark style="color:red;">Critical</mark>      | $1,000 USD            |
| <mark style="color:orange;">High</mark>       | $500 USD              |
| <mark style="color:yellow;">Medium</mark>     | $50 USD               |
| <mark style="color:purple;">Low / Info</mark> | Positive Ethos Review |

Severity and resolution are strictly determined by the Ethos team. Payment can be made in either FIAT or USDC/USDT.

### Smart Contracts

Smart Contract rewards and disputes are managed by Sherlock

{% embed url="https://audits.sherlock.xyz/bug-bounties/pre/15" %}

Disputes addressed by Sherlock may not be re-escalated to the Ethos team.

## Eligibility and Scoring

### Web Services

Critical severity findings include:

* Disclosure of Ethos application Attestation signature private keys
* Trigger transactions, intercept, drain, withdraw, or otherwise impact user funds

High severity findings include:

* Redirect users to invalid Ethereum addresses prior to submitting a transaction
* Cause users to attest invalid social media or external accounts, or take over existing attestations (without compromising the underlying account)
* Force users to vouch for you or others

Medium severity findings include:

* Claim XP for social media accounts you do not control
* Force others to claim your referral links
* Force users to review you or others

Low / Info severity findings include:

* Anything that impacts the generation or calculation of score or XP

### Smart Contracts

Smart contract eligibility and severity scoring will be strictly managed by Sherlock.

[https://audits.sherlock.xyz/bug-bounties/pre/15](https://audits.sherlock.xyz/bug-bounties/pre/15)

The following issues are considered 'known' and ineligible for rewards.

<details>

<summary>Known Issues</summary>

* Descriptive error messages (e.g. stack traces, application or server errors).
* Fingerprinting / banner disclosure on common/public services.
* Clickjacking and issues only exploitable through clickjacking.
* Logout Cross-Site Request Forgery (logout CSRF).
* Presence of application or web browser ‘autocomplete’ or ‘save password’ functionality.
* Lack of Secure/HTTPOnly flags on non-sensitive Cookies.
* Lack of "security speed bump" when leaving the site.
* Weak Captcha / Captcha bypass.
* Login or Forgot Password page brute force and account lockout not enforced.
* Username enumeration.
* Missing HTTP security headers, specifically ([https://owasp.org/www-project-secure-headers/](https://owasp.org/www-project-secure-headers/)), e.g.
  * Strict-Transport-Security.
  * X-Frame-Options.
  * X-XSS-Protection.
  * X-Content-Type-Options.
  * Content-Security-Policy, X-Content-Security-Policy, X-WebKit-CSP.
  * Content-Security-Policy-Report-Only.
  * Cache-Control and Pragma
* HTTP/DNS cache poisoning.
* SSL/TLS Issues, e.g.
  * SSL Attacks such as BEAST, BREACH, Renegotiation attack.
  * SSL Forward secrecy not enabled.
  * SSL weak/insecure cipher suites.
* Self-XSS reports will not be accepted.
  * Similarly, any XSS where local access is required (i.e. User-Agent Header injection) will not be accepted. The only exception will be if you can show a working off-path MiTM attack that will allow for the XSS to trigger.
* Vulnerabilities that are limited to unsupported browsers will not be accepted (i.e. "this exploit only works in IE6/IE7").&#x20;
* Known vulnerabilities in used libraries unless you can prove exploitability.
* Missing or incorrect SPF records of any kind.
* Missing or incorrect DMARC records of any kind.
* Source code disclosure vulnerabilities.
* Information disclosure of non-confidential information
* The ability to upload/download viruses or malicious files to the platform.
* Email bombing
* Request Flooding
* Lack of rate limiting

</details>

## Safe Harbor

Ethos will adhere to "safe harbor" protections; we will not pursue legal action against known ethical security researchers ("whitehats") attempting to defend Ethos against active exploitation. To qualify for safe harbor protections, notify Ethos of your intent and what attack you are defending against by notifying us at [support@ethos.network](mailto:support@ethos.network) and we will confirm safe harbor status.&#x20;

Note: without written acknowledgement from Ethos staff, safe harbor is not guaranteed.

Ethos requires that you return 90% of recovered funds within 24 hours to qualify for Safe Harbor protections. Recovered funds may be transferred to [0x9C98258da66Ed095948CE4774e541C9FE978e946](https://etherscan.io/address/0x9c98258da66ed095948ce4774e541c9fe978e946)&#x20;



