---
code: DCP-01
title: Early Staker Initiative powered by Enzyme vaults
posted_on: 2023-08-14
results: 87.28% YES votes, 9.39% NO votes, 191 addresses, 22.9M votes
url: https://www.tally.xyz/gov/diva/proposal/87485887634082742365047256619524632216107014477059444808141072263652653848832
---

# DCP-01: Early Staker Initiative powered by Enzyme vaults

## Description

This proposal has been curated by @moss @elisafly, @gainzley here, posting from [Avantgarde Treasury](https://avantgarde.finance/). They are the core contributors of [Enzyme](https://enzyme.finance/), formerly Melonport and one of the governance [delegates](https://www.tally.xyz/profile/0xb49f8b8613be240213c1827e2e576044ffec7948?governanceId=eip155:1:0xFb6B7C11a55C57767643F1FF65c34C8693a11A70)for Diva Staking.

As per governance DAO [guidelines](https://docs.staking.foundation/proposals), the proposal is brought by [donkotler.eth](https://www.tally.xyz/profile/0xacbabbb5b96b0e2889c27496fa33e6f26081e1a2?governanceId=eip155:1:0xFb6B7C11a55C57767643F1FF65c34C8693a11A70), who represents 1M+ delegated DIVA tokens and therefore meets the criteria to submit a binding DAO proposal.

### Motivation

Diva DAO, with [4300+ delegated voting holders](https://dune.com/kevinzzz/diva-dao), has initially distributed 100 million DIVA tokens (10% of total supply) to active Ethereum participants.

This initiative seeks to attract TVL and involve a broader audience of future Stakers prior to the mainnet launch. Diva Staking's TVL growth is essential, and this initiative aims to attract support before mainnet release.

A pre-launch TVL initiative - with associated token distribution - for a new protocol like Diva brings a ripple of network effects.

- Stakers know that the protocol and its Liquid Staking Token are widely adopted.
- Stakers get DIVA allocations, which gives them a voice in governance.
- Depositors in the initiative benefit by using proven non-custodial infrastructure.
- Depositors who hold ETH or stETH can support Diva with little or no opportunity cost.
- Operators benefit from being able to plan sufficient capacity ahead of time. Integrations with other DeFi primitives are more likely if there is significant TVL committed. This includes lending, use as collateral, bridging to Layer 2s, etc.

The Ethereum ecosystem benefits by adding diversity to its LST ecosystem, currently dominated by a single provider who holds >85% of LSTs and >30% of all staked ETH, which poses significant systemic risks.

### Summary / TL;DR

The proposal presented the advantages of using the Enzyme platform and for the potential Early Stakers to participate by depositing in one of the 2 vaults in a non-custodial fashion.

- Theinitiative involves ETH or stETH deposits into Enzyme vaults, and a way to account for timing, size and duration of those deposits that will lead to the calculation of DIVA token allocations for each participant. The proposed duration of the initiative is 365 days.
- Depositors will accrue DIVA tokens for every day their (st)ETH is in the vaults.
- Enzyme's time-tested infrastructure, the waiver of protocol fees and other benefits are thoroughly highlighted in [the RFC](https://commonwealth.im/divastaking/discussion/12178-rfc-start-collecting-prelaunch-tvl-with-an-early-staker-program-powered-by-enzyme-vaults) (Infrastructure & Program Design).
- For details on the [proposed T&Cs](https://commonwealth.im/divastaking/discussion/12393-rfc-proposed-terms-conditions-tcs-for-diva-early-stakers-vaults-on-enzyme-incl-token-distribution-criteria-for-program-participants) of the token distribution, please refer to the complementary RFC which will be submitted separately.

### RFC - Tempcheck Status

You can find the RFC on Commonwealth [here](https://commonwealth.im/divastaking/discussion/12178-rfc-start-collecting-prelaunch-tvl-with-an-early-staker-program-powered-by-enzyme-vaults), which was published on July 14th 2023. The non-binding Tempcheck vote has been closed out with 100% YES and 0% NO

### Description of the proposed action

This Diva Curation Proposal (DCP) introduces the creation of an Early Staker Initiative for Diva Staking, to be implemented on Enzyme vaults.

Associated decisions:

- Diva Staking DAO creates 2 vaults on Enzyme: one for ETH and one for stETH
- Avantgarde is set as manager for the Diva vaults with trustless delegation rules
- The Enzyme protocol fee for the 2 Diva vaults is waived (explanation [here](https://commonwealth.im/divastaking/discussion/12178-rfc-start-collecting-prelaunch-tvl-with-an-early-staker-program-powered-by-enzyme-vaults?comment=64260))
- Funds deposited in the 2 vaults are kept idle until Diva Staking mainnet launch
- Avantgarde develops native Enzyme integrations for 2 protocols: Lido (to ensure 1:1 stETH:ETH redemption) and Diva Staking (to ensure 1:1 ETH:divETH staking)

All other aspects of the initiative are not part of this DCP, but are being discussed after the release of the second RFC laying out the [Terms & Conditions](https://commonwealth.im/divastaking/discussion/12393-rfc-proposed-terms-conditions-tcs-for-diva-early-stakers-vaults-on-enzyme-incl-token-distribution-criteria-for-program-participants), including the allocation of DIVA tokens for Avantgarde.

### Technical implementation

The following course of action is proposed:

- Avantgarde multisig (“vault owner”) creates the 2 vaults on behalf of the DAO
- Among initial vault settings, AVG’s multisig (“vault owner”) [assigns delegation](https://docs.enzyme.finance/managers/vaults-for-organisations/delegate-trading) to Avantgarde (“vault delegated manager”)
- Among initial vault settings, Multisig [prevents deposits](https://docs.enzyme.finance/managers/setup/investments) until the official kickoff date.
- Enzyme DAO to waive protocol fees on the new vaults. See explanation on how this will be done [here](https://commonwealth.im/divastaking/discussion/12178-rfc-start-collecting-prelaunch-tvl-with-an-early-staker-program-powered-by-enzyme-vaults?comment=64260). The waiver will be implemented in good faith that the distribution of DIVA tokens for Avantgarde is passed in the second DCP (see also “Notable changes”).
- Avantgarde & Diva DAO announce the official kickoff date across several channels (Commonwealth, Discord, etc.)
- Upon official kickoff date, Avantgarde’s Multisig enables deposits on Enzyme vaults.
- Once the initiative is up & running, Avantgarde proposes the [transfer of ownership](https://docs.enzyme.finance/managers/customise-your-settings/change-owner) from its multisig to the DAO Governor contract within 30 days from the kickoff date.
- During the course of the initiative, Avantgarde will maintain the assets idle as described in the RFC, will implement the needed engineering work for the integration and will facilitate the computation of the token distribution for each participant.

### Avantgarde's role

As described in the RFC, it includes the following elements:

- Smart contract engineering efforts to integrate Diva Staking Protocol
- Smart contract engineering efforts to integrate Lido Staking Protocol to ensure 1:1 redemption of stETH to ETH before staking to Diva.
- Bear the costs associated with the audit of the above integrations Supervision, assistance and facilitation of DIVA token distribution, tracking the onchain activity related to the vault and turning that into the computation of the distribution amounts for each participant.
- Playing a role in facilitating the Enzyme Council’s decision to waive protocol fees (normally 25 bps) for Diva, which can be as high as 250 ETH if the initiative was to max out at 100K ETH.

In general the proposal emphasises alignment, transparency, and community participation in building a sustainable future for the Ethereum ecosystem.

### Notable changes

- Move the approval of the % allocation of DIVA tokens for Avantgarde from the scope of this proposal to the scope of the second complementary [proposal](https://commonwealth.im/divastaking/discussion/12393-rfc-proposed-terms-conditions-tcs-for-diva-early-stakers-vaults-on-enzyme-incl-token-distribution-criteria-for-program-participants) RFC (T&C)
- Based on the same complementary [RFC](https://commonwealth.im/divastaking/discussion/12393-rfc-proposed-terms-conditions-tcs-for-diva-early-stakers-vaults-on-enzyme-incl-token-distribution-criteria-for-program-participants), Avantgarde self-imposes a 6-month additional vesting period (beyond the 365 days) that will lock the DIVA tokens distributed.
- Pending final decision of the Enzyme DAO Council: include an audit competition for the new integrations of Lido & Diva Staking to be run in addition to the audit carried out by Chain Security.

### Notable exclusions

The proposal does not include a third vault with denomination of rETH for the reasons explained [here](https://commonwealth.im/divastaking/discussion/12178-rfc-start-collecting-prelaunch-tvl-with-an-early-staker-program-powered-by-enzyme-vaults?comment=64291). It would be best as a possible extension with a further vote later on so it can be discussed separately. There are also workload implications Avantgarde needs to take into account and plan for.

### Classification

This is a Diva Curation Proposal (DCP), requiring 50% positive votes to be enacted. DCPs are Intended to distribute governance power among communities.

### Copyright waiver

Avantgarde Treasury, as the owner or rights holder of certain creative works, hereby waives specific rights under copyright law in favour of Diva Staking DAO. This waiver pertains to the works described as governance proposals, and includes the rights of reproduction, distribution, public display, and creation of derivative works. This waiver is granted for the purpose of this governance process. Proper attribution to us shall be provided by the recipient whenever the works are used or displayed. This waiver does not extend beyond the rights explicitly stated.
