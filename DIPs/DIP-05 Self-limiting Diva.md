# Self-limiting Diva

## Abstract

The staking ecosystem is still young, and Diva will be offering the lowest bond available to potential Node Operators in the Liquid Staking Derivative market. 

It’s not outside the realm of possibility that Diva’s new product offering is a “killer app” in this space and Diva could be set to take a large amount of market share. 

With that in mind, I propose that Diva should self limit.

## Motivation

Danny Ryan has identified some [key thresholds](https://notes.ethereum.org/@djrtwo/risks-of-lsd) and their consequences:
- above 33% - an LST can prevent finalization
- above 50% - an LST can censor
- above 66% - an LST can achieve finalization

For further context, Danny elaborated on his views in [this interview with Evan Van Ness](https://www.youtube.com/watch?v=Y0ddkSa1ZuI&t=2s).

Empirically, the liquid staking market has centralizing dynamics; this is an externality that the free market is unable to express - a classic tragedy of the commons. 

One way liquid staking protocols can mitigate this risk is by committing to self-limiting to 22% of staked ETH - a threshold that both mitigates Danny Ryan's concerns listed above, while also allowing staking protocols enough breathing room to be competitive on the open market. 

Anthony Sassano and Eric Conoar also have [a great discussion about the risks here.](https://www.youtube.com/watch?v=hQO2rHQze-4&t=1137s)

[Superphiz’s rationale for limiting to 22%](https://twitter.com/superphiz/status/1525224461380747268?s=20) are:
- It requires at least four parties to affect finalization.
- We can lose one provider at 22% and not miss a step on the network.
- It is capture-resistant so third parties are comfortable building on the network.

A few other protocols have committed to self-limiting:
- Rocket Pool has passed a DAO resolution to [self-limit to a maximum of 33%](https://github.com/rocket-pool/RPIPs/blob/main/RPIPs/RPIP-17.md)
- Stakewise has [stated on Twitter](https://twitter.com/stakewise_io/status/1525225299146944513?s=20) that they would self limit to 22%
- Vitalik suggests [self-limiting via increasing its protocol fee](https://twitter.com/VitalikButerin/status/1525301234516652032?s=20)

Even though Diva is still nascent, Diva deciding to self-limit would indicate to the wider Ethereum community that Diva puts Ethereum’s health before itself.

## Specification

**Diva Staking will take measures to avoid greater than 22% of the ETH deposited on the beacon chain being deposited through the Diva protocol.**

- This may imply a number of actions, such as stopping the creation of validators, or any other feasible measure which can be reasonably implemented by the community to accomplish the above outlined aim.

**One such action could be for Diva to stop the creation of validators, should Diva reach that threshold, but for Diva to continue minting divETH tokens.**

This will dilute divETH's staking APR, creating an economic incentive to stake with other liquid staking providers , while also preventing Diva from crossing that same threshold. This will have the added benefit of making integrations with other protocols, and especially immutable protocols, simple and less prone to failure.

## This Proposal, if passed, represents the DAO's Intent

This specification represents the community's intent and is not a direct call for a code implementation. The Diva DAO acknowledges and respects the operational boundaries and legal considerations of Diva BVI. The DAO understands that Diva BVI retains its autonomy and is not subordinate to the DAO's intents. Our aim is to convey the collective values of our community, fully recognizing that the final implementation decisions rest with Diva BVI and its associated entities.

## Classification

Low risk, no executable smart contract code.

## Copyright waiver

Copyright and related rights waived via CC0 1.0 (https://creativecommons.org/publicdomain/zero/1.0/)
