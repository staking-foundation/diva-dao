# Diva Staking DAO INITIAL COMMUNITY GUIDELINES 

## Section 1. Definition and Purpose

The Diva Staking Decentralized Autonomous Organization (the ‘Diva Staking DAO’) is an unincorporated association of individuals, entities, associations and/or other persons or groups of persons holding the DIVA token AND having completed a process referred to as “delegation”. The Diva Staking DAO is not intended to, and shall not be deemed to, be a legal person or have a legal personality separate from the DAO Members. Without limiting the generality of the foregoing, the DAO is not intended to be, and shall not be deemed to be, a partnership.

The primary objective of the Diva Staking DAO is to curate and maintain the publicly available software resources known as the Diva Staking protocol. It is important to note that the Diva Staking DAO does not engage in administering or managing the Diva Staking protocol in any way. Instead, its mission is focused on enhancing the accessibility, efficiency, and resilience of the blockchain interaction commonly referred to as 'staking' through the utilization of non-proprietary software.

## Section 2. Governance Tokens

Diva Staking DAO governance tokens (the Governance Tokens) means the effectively delegated tokens associated with the Diva Staking protocol and referred to in https://github.com/staking-foundation and designated as Delegated DIVA. D-DIVA. D-Tokens, or any other designation the Diva Staking DAO may find appropriate from time to time.

## Section 3. Excluded Tokens 

DIVA Tokens that have not been revocably delegated, either through self-delegation or delegation to third parties, using the designated governance smart contract of the Diva Staking DAO, are not considered as Diva Staking DAO governance tokens. These tokens do not possess the authority to submit any type of DAO proposal or participate in the voting process for any DAO proposals.

## Section 4. DAO Resolutions.

As per the token amount thresholds outlined in Section 5 below, every holder of Governance Tokens holds the right to submit and participate in the voting of proposals, referred to as 'DAO Proposals.' Once a proposal is duly approved by the Governance Token holders and has not been invalidated by the DAO governance mechanism, it is recognized as a 'DAO Resolution.’

## Section 5. DAO Proposals. 

Proposals may be submitted by any Governance Token holder holding at least 1 Million Governance Tokens subject to any applicable threshold, and/or any frequency restriction or other parameter designated by the Diva Staking DAO through the passage of a Diva Improvement Proposal (as defined below).

There are three types of Proposals:

1.	DCP - Diva Curation Proposals; proposals intended to distribute governance power among communities, sealing strategic partnerships, etc.
2.	DIP - Diva Improvement Proposals; proposals aiming to adapt or modify a configurable feature of the Diva Staking protocol.
3.	DUP - Diva Update Proposals; complex proposals aiming to update core infrastructure and require some code implementation.

## Section 6. DAO Proposals Quorum and Thresholds. 

In order for a Proposal to be valid a quorum of at least 10 Million Governance Tokens is required. 

The thresholds initially set for each kind of proposal are as follows, 

- DCP - more than 50% of favourable votes
- DIP - more than 66% of favourable votes
- DUP- more than 75% of favourable votes

## Section 7. DAO Proposals Procedures

### 7.1. Temperature Check - NDP - New Diva Proposals Process

In order for a proposal to be formally considered by the community an off chain process referred to as a ‘temperature check’ must be followed. Its main objective is to properly evaluate if the proposal intended to be submitted gains enough interest and community support.

The temperature check is done through the DAO offchain community forums by opening a new thread referring to the term “New Diva Proposal +[subject]”

The thread is intended to provide all necessary information and collect feedback to prepare the formal proposal which would later be submitted for its voting and subsequent approval or rejection.

Any member of the community at large may open a thread in the Diva Forum outlining the proposal which needs to be debated or any suggestion which may be deemed as beneficial to the community at large. 

The title of the thread shall include: NDP and a short description of the proposal 

The NDP shall contain at least the following: 

- Short and concise description of the proposal
- Rationale: why the proposal is necessary and what benefit will bring to the community
- Tentative classification as DCP, DIP and DUP
- A community pool to indicate the flag the level of support the proposal may have.

### 7.2. Proposal submission

Proposals can only be submitted by those which have at least 1M D- DIVA delegated and it implies an on-chain transaction.

Proposals can be submitted at https://tally.xyz/gov/diva by selecting “create a new proposal”  

The proposal shall include the following structure: 

- Short name of the proposal 
- Definition as DCP, DIP or DUP 
- DCP Proposals shall include a short description of the proposed action to be taken
- DIP Proposals shall include a risk assessment of the proposed implementation of such proposal and the executable code (Tally provides a list of executable functions which can be implemented) 
- DUP Proposals; this shall include a thorough description of the technical features aimed to be implemented, executable code and test cases. 

Any proposal shall include a copyright waver. Further, any code or material included in any proposal shall be open sourced and released to the public domain without any restriction whatsoever.

### 7.3. Proposals Voting Delay

Once the proposal has been created “on-chain” there is a waiting period (voting delay). During that period token holders can still delegate their tokens (either self delegate or delegate to third parties). Such delegation will affect the necessary quorum for a proposal to become valid as only Delegated DIVA tokens are accounted for any governance purpose. 

Initially the voting delay period is being set to 2 days 

### 7.4. Proposal Voting Period

Once the voting delay period has elapsed all the proposals have a predetermined voting period of 5 days upon submission under which any D-DIVA can vote in favour or object 

After such period has elapsed, considering a valid quorum of 10M D-DIVA has been met and the correspondent voting threshold has been exceeded the proposal shall be considered passed and will become a DAO Resolution

## Section 8. DAO Resolutions

### 8.1. Queueing for Execution and Cooldown Period

Upon successful confirmation that the corresponding threshold and quorums have been met, an on-chain transaction is required to set the approved DAO Resolution in queue for its execution, starting a Cooldown Period through this transaction.

Initially the Cooldown period is being set as 6 days for DCPs and DIPs while DUPs have a cool down period of 10 days. 

During the Cooldown period an approved DAO Resolution still can be disputed and cancelled (see more below) 

### 8.2 Execution 

Once the Cooldown period has elapsed, anybody can execute the transaction to implement a DAO resolution. As the required functions to effectively implement the desired outcome have been previously registered within the proposal, the execution of said transaction does not alter in any manner the terms of the DAO Resolution. 

## Section 9. Disputes

Any DAO Resolution can be challenged before it is executed due security considerations such as governance attacks or fraudulent code implementation. 

In order to challenge a DAO Resolution a Cancellation Proposal must be submitted by a community participant counting with a governance power delegated of at least 1M D-tokens. 

The Proposal shall clearly specify “Cancellation Proposal” and set clearly and consciously what is the harm prevented by the cancellation and other remedies proposed to avoid further damage to the Diva Staking protocol and or community. 

In order to be valid a cancellation proposal requires a quorum of at least 10M tokens and more than 50% of favourable votes. 

The execution of said Cancellation Proposal can be fulfilled 2 hours after its approval.   

