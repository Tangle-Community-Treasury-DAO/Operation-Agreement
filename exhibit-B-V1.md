# Exhibit B V1

This document consits of two parts:

- [Procedure A](#exhibit-b---procedure-a-the-shimmer-governance-framework)
- [Procedure B](#exhibit-b---procedure-b-the-shimmer-community-grant-committee)
---
## Exhibit B - Procedure A: The Shimmer Governance Framework

*This is the full specification for all governance processes in the Shimmer network. Detailed rules and procedures are defined here.*
---

## TL:DR

This framework defines the governance process for [selected topics](./governance-scope.md) in the Shimmer network. Changes will be proposed using a three-stage process that can result in a vote by Shimmer token holders. The [governance forum](https://govern.iota.org) hosts the discussions and proposals. This framework defines the detailed rules and standardizes decision-making processes that must be followed to make changes in the network. The specification hosted in this Wiki article was created in a proposal to the Shimmer community. Only the defined final specification is hosted here and the parts 1. Simple Summary, 2. Abstract, 3. Motivation, 6. Implementation have been left out of publishing in the Wiki. The full proposal including these sections can be read [here](https://github.com/iota-community/Shimmer-Governance/blob/main/The%20Shimmer%20Governance%20Framework.md)

## 4. Governance Specification

### 4.1 Proposal Lifecycle

The [Governance forum](https://govern.iota.org), [introduced by the IOTA Foundation](https://blog.iota.org/the-iota-governance-forum/) in May 2022, is the host for our governance process and is used to move a proposal through the three phases of governance:

- Phase 1 - Discussion
- Phase 2 - Temperature check
- Phase 3 - Voting

Once an idea successfully passes phase 2, a vote is initiated in phase 3 using the Firefly voting mechanism based on Shimmer token ownership. This method uses the functionalities of the already developed Firefly Governance and the Hornet [INX participation plugin](/inx-participation/welcome) developed and used first in the [Build vs. Burn](https://blog.iota.org/iota-treasury-vote-how-to-take-part/) vote that happened in June 2022.

**To be accepted and implemented as a vote in Firefly, a governance proposal must successfully pass through the first two phases of the framework that work as a filter mechanism to only allow proposals that fulfill specific criteria to be implemented as a Firefly vote.**

<table>
  <tbody>
    <tr>
      <td>
      </td>
      <td>
        <strong>Phase 1</strong>
      </td>
      <td>
        <strong>Phase 2</strong>
      </td>
      <td>
        <strong>Phase 3</strong>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Consensus mode</strong>
      </td>
      <td>
        <strong>none</strong>
      </td>
      <td>
        <strong>Soft consensus</strong>
      </td>
      <td>
        <strong>Network consensus</strong>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Details</strong>
      </td>
      <td>
        <ul>
          <li>Introducing an idea by posting in the
            <a href="https://govern.iota.org/"> forum </a>
          </li>
          <li>Approval by
            <a href="#governance-forum-moderators"> moderator </a>
          </li>
          <li>The moderator adds the proposal to the phase 1 category</li>
          <li>If the proposal does not meet the guidelines, it goes to the archive</li>
          <li>All specifications and changes to the idea happen in phase 1. This can include several rounds of polling and edits to the original proposal to include input from the community.</li>
          <li>All edits require a new post with a version number</li>
          <li>Receive 50 likes or 50 yes votes in a poll from the community</li>
          <li>If the proposal does not have any engagement over a 30 days duration and does not have the minimum 50 likes / yes votes, it will be archived</li>
          <li>The moderator approves the final version of phase 1 proposal → moves to phase 2</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Post in the forum</li>
          <li>Follows a defined structure of the
            <a href="#412-governance-proposal-template-phase-2--3--emergency-proposal"> governance template </a>
          </li>
          <li>Approval by
            <a href="#governance-forum-moderators"> moderator </a>
          </li>
          <li>Receives a
            <a href="#unique-identifier"> unique identifier number </a>
            by a moderator</li>
          <li>A finalized concept ready to be voted on by the community (during phase 2, the proposal should not be possible to edit anymore)</li>
          <li>Includes a poll to signal soft consensus</li>
          <li>Poll duration 7 days</li>
          <li>Poll must receive a minimum of 100 yes votes to be accepted</li>
          <li>If accepted, it leads to a network-wide vote in Firefly</li>
          <li>Poll must include “Make no changes” option</li>
          <li>It is a non-binding decision</li>
          <li>Can also be conducted as a runoff poll if any
            <a href="#47-counter-proposals"> counter proposals </a>
            qualify</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Announcement post in the forum by a moderator once all requirements are met</li>
          <li>Voting is implemented in Firefly. For the transfer, the exact wording of the question is used without modification in FF. Node operators implemented counting.</li>
          <li>Must include “make no changes” option</li>
          <li>Vote duration 14 days</li>
          <li>Cooldown 7 days before execution</li>
          <li>5% quorum for passing</li>
          <li>Simple majority needed to pass</li>
          <li>Decisions are binding</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Requierements</strong>
      </td>
      <td>
        <ul>
          <li>The post must discuss one of the
            <a href="./governance-scope.md"> parameters that are open for governance </a>
          </li>
          <li>The post must follow the rules set for
            <a href="#guaranteeing-stability---resubmital-delay"> resubmittal delays </a>
          </li>
          <li>Edits require reposting with versioning</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Poll must include “no changes” option</li>
          <li>Follows a defined structure as described in the
            <a href="#412-governance-proposal-template-phase-2--3--emergency-proposal"> proposal template </a>
          </li>
          <li>No edits allowed</li>
          <li>Text that will be used in the Firefly votes is already specified</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Participation event created by the submitter</li>
          <li>Checked by a minimum of two moderators or Admins</li>
          <li>Must include the option “Make no changes” and the same text as the phase 2 poll</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Timeframe</strong>
      </td>
      <td>
        <ul>
          <li>Ideas can be posted on the forum any time and should be discussed as long as needed.</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Poll duration is seven days
          </li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Vote duration 14 days (7 days pre-vote, 7 days counting period)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Decision making to move to next phase</strong>
      </td>
      <td>
        <ul>
          <li>Poll: 50 votes in favor of the proposal in the last version poll</li>
          <li>no poll: The latest published post version received 50 likes.</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Poll must receive a minimum of 100 votes in favor of the proposal</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Firefly vote: simple majority wins</li>
          <li>Must reach 5% quorum of
            <a href="#maximum-achievable-votes"> maximum achieveable votes </a>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Denied
        </strong>
      </td>
      <td>
        <ul>
          <li>Spam</li>
          <li>Does not talk about the
            <a href="./governance-scope.md"> parameters open for governance </a>
          </li>
          <li>Proposal has no engagement over 30 days</li>
          <li>Proposal doesn't reach a minimum of votes/likes</li>
          <li>Proposal conflicts with the 
            <a href="#guaranteeing-stability---resubmital-delay"> resubmittal delay rules </a>
          </li>
          <li>Proposal does not meet the
            <a href="#42-shimmer-governance-framework-guiding-principles"> guiding principles. </a>
          </li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Does not reach the required votes in favor of the proposal in the poll in the seven days</li>
          <li>A counter-proposal reaches community support within 7 days. The proposal then is halted for a runoff.</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Option “Make no changes” reaches the simple majority of votes</li>
          <li>Does not reach 5% quorum of
            <a href="d#maximum-achievable-votes">maximum achievable votes
            </a>
          </li>
          <li>Canceled through an emergency proposal submitted during the 7-day cooldown.</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 4.2 Shimmer Governance Framework Guiding Principles

1. A proposal must be relevant to the Shimmer network and ecosystem.
2. If voted for, the proposal must add positive value and support to the Shimmer ecosystem.
3. All proposals must not segregate individuals, organizations, or communities based on sex, race, color, ethnic or social origin, genetic features, language, religion or belief, political or any other opinion, membership of a national minority, property, birth, disability, age or sexual orientation.
4. The proposal’s intent must not have been submitted within the current [submission season](#48-seasons) and follow the [resubmission delay rules](#guaranteeing-stability---resubmital-delay).
5. The proposal must meet the defined [parameters that are open for governance](./governance-scope.md). All technical proposals relevant to IOTA, Shimmer, and Assembly protocols must be submitted through the standard TIP process.
6. The proposal should not be directed towards using, requesting, or managing the Shimmer Treasury Funds once a Shimmer Community Treasury DAO is established under its own guidelines and rules. Until the Shimmer Community Treasury DAO has been established, this framework can be used to make decisions on the structure and rules of the Treasury DAO. This governance framework can also be used to make decisions on allocating a budget from the Shimmer community Treasury Wallet to the Shimmer Treasury DAO once the Treasury DAO has been established.

### 4.3 Defining the stakeholders of the governance process

#### Governance Forum members

Everybody who successfully registers an account in the [governance forum](https://govern.iota.org/).

#### Governance Proposal submitter (phase 1)

A [Governance Forum member](#governance-forum-members) who posts a governance proposal under the [[Shimmer Governance Proposals] [Phase 1] Discussions](https://govern.iota.org/c/shimmer-governance-proposals/phase-1-discussions/53) category or who submits an [Emergency proposal](#411-phase---3-emergency-proposals) in the governance forum.

To submit a topic in the [Shimmer Governance Proposals](https://govern.iota.org/c/shimmer-governance-proposals/phase-1-discussions/53) section of the forum, the member must have reached the Trust level 1.

This member is responsible for the proposal and needs to make sure that the proposal fulfills all acceptance requirements defined for the different phases of the governance process.

The member is also responsible for all needed coordination with moderators to move a proposal to the next stage or implement it as a vote in phase 3.

A proposal can only move forward at the request of the proposal submitter.

This requires the **proactive involvement** of the proposal submitter. After 30 days of inactivity in the forum (no new comments), a proposal is to be rejected and archived by moderators if it has not met the [acceptance requirements](#proposal-acceptance-requirements-phase-1) to move to the next phase.

The moderators or entities like the IOTA Foundation or Node operators will not automatically take action on a proposal if the original proposal submitter does not request this. If a proposal is not followed up within 30 days, it is considered abandoned by the original submitter and will be closed and archived following the guidelines defined. The topic could then be picked up by someone else and resubmitted as a phase 1 discussion post.

#### Governance Forum voters (phase 2)

Governance Forum members that reached Trust level 1 in the forum are allowed to vote on polls in a [phase 2 proposal](#45-phase-2---temperature-check-phase).

The requirements to achieve Trust level 1 are set as follows:

- Active registered account in the governance forum and,
- has opened a minimum of 3 topics and did read a minimum of 3 topics completely in the forum and,
- has spent a minimum of 25 minutes (aggregated) reading posts in the forum

#### Firefly voters (phase 3)

Everybody who is in control of the minimum amount of Shimmer tokens required to produce one vote. This amount is currently defined as 1000 Glow and follows the [technical specification](https://github.com/iotaledger/inx-participation) for the Hornet INX - participation plugin.

#### Governance Forum Moderators

To enable an effective governance process, some community members need to handle administrative tasks in the governance process, mainly in the governance forum. The community group that works on governance and meets weekly to discuss these topics has selected five community members to fill these positions. The community can propose to remove moderators through the here-defined governance process.

Currently, the following community members are selected as governance forum moderators:
[@Deep_Sea](https://govern.iota.org/u/deep_sea/summary), [@Werner](https://govern.iota.org/u/werner/summary), [@overclocked](https://govern.iota.org/u/overclocked/summary), [@AndyW](https://govern.iota.org/u/andyw/summary)

##### Tasks and responsibilities

- Daily check the forum if new posts are submitted that are requested to become a phase 1, phase 2, or emergency proposal.
- Check every newly submitted post in the [Shimmer Governance Proposals](https://govern.iota.org/c/shimmer-governance-proposals/51) Category if it fulfills the Proposal Acceptance Requirements for [phase 1](#proposal-acceptance-requirements-phase-1), [phase 2](#proposal-acceptance-requirements-phase-2), [phase 3](#proposal-acceptance-requirements-phase-3) or [emergency proposal](#acceptance-requirements-emergency-proposals). This includes checking all provided links in the post for correctness.
- If all requirements are met, approve the posts in the respective Forum subcategory and add the [unique identifier](#unique-identifier) number and the phase tag to the post.
- Keep the [public Notion page](https://shimmergov.notion.site/18af77a6634f4d9d91b7c16d9f294fbd?v=dcd7703eac1e4dd3b5302bf533546cb3) that hosts the unique identifier numbers up to date.
- Run the official [Shimmer Governance Twitter account](https://twitter.com/ShimmerGov) and use it to inform the community about ongoing phase 2 and phase 3 decisions.
- Ensure that phase 2 polls and phase 3 votes are published following the [specified timelines](#49-timing--planning-of-proposals-and-votes)
- Before approving a phase 2 poll into phase 3, ensure that there has been no successful [counter proposal](#47-counter-proposals) submitted.
- If a Phase 2 poll is accepted, inform the community by posting about the poll from the [Shimmer Governance Twitter account](https://twitter.com/ShimmerGov).
- If the requirements are not met, inform the initiator that the proposal misses specific requirements via a private message and keep the proposal unpublished until the requirements for accepting the post are met.
- Support the initiator of a proposal if they lack the technical skills to create the executable participation event that will be uploaded to the nodes for a phase 3 Firefly vote.
- Merge the participation event in the [Github “participation events” repository](#414-hosting-of-the-participation-events-for-governance-votes-on-github) if approval for phase 3 vote has been granted by two moderators or one moderator and one administrator.
- If a phase 2 poll has successfully met all [requirements](#proposal-acceptance-requirements-phase-2) to become a phase 3 Firefly vote, publish an [announcement post](#the-announcement-forum-post-in-phase-3-uses-this-template) under the [Phase 3 vote announcements](https://govern.iota.org/c/shimmer-governance-proposals/phase-3-vote-announcements/54) subcategory following a specific template that includes the unique identifier, the link to the phase 2 discussion, and the time and date when the phase 3 vote begins in Firefly. This announcement post is locked from comments and serves only as information to forum users.
- Publish this announcement post from the Shimmer governance Twitter account.
- Inform one of the IOTA Foundations community managers that a vote in Firefly is planned so that the IF comms department can schedule the social media posts to inform the wider community about the upcoming vote.
- Move finished or declined proposals (phase 1, phase 2, or phase 3) to a separate subcategory [Proposal Archive](https://govern.iota.org/c/shimmer-governance-proposals/proposal-archive/55) in the forum for ended proposals. Proposals moved to the archive will be tagged accordingly [accepted] or [declined].
- If a Firefly vote has been conducted, edit the phase 3 announcement post to include a link to the validated results of the vote published on GitHub.
- Observe the forum and the governance process and propose required adjustments to the [parameters under probation](#specification-parameters-under-probation) after consent in the moderator group has been achieved.
- Prepare the [seasonal vote](#48-seasons) to ratify the new seasonal specification that includes all recently made changes.
- Moderators will manage discussions during the phases to ensure they are not disrespectful and focus on the proposal topic in a positive manner.
- If a participant is aggressive during the discussions and continues to add negative comments within a discussion thread, a minimum of 2 moderators and one admin should discuss and ban a member if decided upon. Guiding principles are described in the forum's [Terms of Service](https://govern.iota.org/t/terms-of-service/4) that regulate all users' activities. They build the foundation for all moderator actions regarding moderation.
- If a submittal is rejected, a moderator or admin will write a brief (one to three sentence) summary stating how the submittal did not follow guiding principles and/or the defined requirements set for submittals.
- The forum moderators will only be granted access to the functionalities required to fulfill the above-described tasks in the forums [Governance] section. This does not provide special access to other administrative functions or the [Research] section of the forum.

#### Governance Forum admins

Employees of the IOTA Foundation which have full access to all functionalities of the Forum. They are responsible for granting moderation rights to the selected [Governance Forum Moderators](#governance-forum-moderators). They can act as Forum moderators if no forum moderator is available to fulfill a required task.
Currently, these IF members are Forum admins: @antonio.nardella @Phylo @anyong @mark.schmidt @Junwei

### 4.4 Phase 1 - Discussion phase

Getting feedback on an idea, adapting it, and including input from others is the primary goal of phase - 1. The Governance forum has a specific category [Shimmer Governance Proposals](https://govern.iota.org/c/shimmer-governance-proposals/51) where this process is hosted. The Discussions phase starts in the [Shimmer Governance Proposals / Phase 1 - Discussion](https://govern.iota.org/c/shimmer-governance-proposals/phase-1-discussions/52) subcategory.

Phase 1 initiates the start of a proposal’s lifecycle. Anyone that has reached [trust level 1](#governance-proposal-submitter-phase-1) in the governance forum can step forward and propose a change to [certain](./governance-scope.md) aspects of the Shimmer network.

The discussion phase must be used to refine the idea to a point where it can be boiled down to either one or two clearly defined options. It may be required that the proposal submitter puts up several polls during the discussion to present a clearly defined and specified concept to the voters in the following phase 2 poll.

All posts in the forum that a trust level 1 member submits are automatically locked from editing 5 minutes after publishing. This means that if a proposal submitter wants to implement some changes in the phase 1 proposal after it has been approved and published by a moderator, the following process needs to be followed (also by members of higher trust levels):

- Close the current topic so that no more comments are possible.
- Submit a new post as a phase 1 Discussion with the same topic title and add Version 2, 3, 4, … to the title
- Directly reference the previous discussion by including a link to the previous post in the new version.
- Follow this process until the proposal submitter is sure that the final version of the proposal has matured and can be formulated as a phase 2 proposal.

The outcome of this process in phase 1 should be a defined and specified proposal ready to be put up for a community poll in phase 2 and implemented in a Firefly vote in phase 3.

To initiate an idea's discussion and decision-making process, a [forum moderator](#governance-forum-moderators) will only allow a post to be published in the [Shimmer Governance Proposals / Phase 1 Discussions](https://govern.iota.org/c/shimmer-governance-proposals/phase-1-discussions/52) subcategory and grant the phase 1 status to a discussion if the topic of the proposal fits one of the [defined Governance parameters](./governance-scope.md) and follows the Shimmer governance framework [guiding principles.](#42-shimmer-governance-framework-guiding-principles)

##### Proposal Acceptance Requirements Phase 1:

- Discussion topic created in the governance forum under the [Governance Proposals / Phase 1 - Discussion](https://govern.iota.org/c/shimmer-governance-proposals/phase-1-discussions/52) subcategory tagged with phase 1
- Duration: topics close automatically after 30 days of inactivity.
- The post must be written in English language
- The post must follow the [Shimmer Governance framework guiding principles](#42-shimmer-governance-framework-guiding-principles).
- A phase 1 topic post needs approval by a moderator and receives the phase 1 tag once it is approved to be published.
- It can only receive a phase 1 tag and become a governance proposal if it discusses one of the parameters [open for community governance](./governance-scope.md), follows the [guiding principles](#42-shimmer-governance-framework-guiding-principles) and does not conflict with the [resubmittal delay rules](#guaranteeing-stability---resubmital-delay).

##### Requirements for a phase 1 proposal to move forward in the process and become a phase 2 temperature check proposal:

- The latest version of the proposal posted by the proposal submitter has either received 50 likes or the latest poll created by the proposal submitter on the latest version of the proposal has received 50 votes in favor of the proposal.

##### Requirements to close a proposal in phase 1

- Topics that have been approved as a phase 1 but have not seen any activity (comments/likes) on the topic for more than 30 days will be automatically closed by the system and then removed from the category and archived by a moderator in the [Proposal archive](https://govern.iota.org/c/shimmer-governance-proposals/proposal-archive/55) category
- The proposal can also be closed and archived at any time by written request of the proposal submitter to a governance forum moderator.

### 4.5 Phase 2 - Temperature check phase

The [Governance Proposal submitter](#governance-proposal-submitter-phase-1) feels confident that the proposal includes everything he or she deems necessary. Hence, a solid and specified proposal has been developed, considering suggestions and refinements raised in phase 1. The proposal is structured using the provided [Governance proposal template](#412-governance-proposal-template-phase-2--3--emergency-proposal) which is implemented as a preconfigured template for all posts in the [Phase 2] - Temperature check subcategory. The submission contains a 7-day lasting Poll conducted by the [Governance Forum voters](#governance-forum-voters-phase-2). If the poll receives enough engagement, it signals support and confidence that the community wants to do a public vote on the manner, which will then be part of the following phase 3.

Phase 2 polls are non-binding decisions and only show sentiment in the community that allows distinguishing if a topic receives enough support to justify a vote in Firefly. All changes to the Shimmer protocol will require a decision by all Shimmer token holders in a phase 3 vote in Firefly.

##### Proposal Acceptance Requirements Phase 2

- A Governance Proposal post was created in the governance forum under the [Shimmer Governance Proposals / Phase 2 - Temperature check](https://govern.iota.org/c/shimmer-governance-proposals/phase-2-temperature-check/53) subcategory and tagged with “phase 2”.
- The proposal links to the phase 1 discussion conducted beforehand. If no phase 1 discussion was conducted, the phase 2 post request will be rejected by the moderators.
- The phase 2 proposal is posted by the same [proposal submitter](#governance-proposal-submitter-phase-1) that had posted the corresponding phase 1 proposal that started the discussion.
- A phase 2 temperature check poll can only begin on specified dates:
  - The first and 3rd Monday of a month before 4 pm UTC and lasts seven days. Moderators ensure that the poll gets published on these days and times.
  - To ensure this, the phase 2 post must be submitted at least 24 hours before the start date of the poll (which is Monday at 4 pm UTC). Proposals that get posted later than 24 hours before the deadline can not be included in the phase 2 period and will have to wait until the next phase 2 period opens (2 weeks later)
- The proposal uses the provided [template](#412-governance-proposal-template-phase-2--3--emergency-proposal) for governance proposals. The proposal template requires all submissions to speak to relevant fields, such as a Simple Summary, Abstract, Motivation, Specification, and Implementation. The template is implemented by default in every post in the [Phase 2] subcategory and shall not be altered besides removing the descriptions in blockquote.
- The text for the participation event is part of the post and contains the exact question and answers. The text is 100% identical to the text used in the poll.
- The proposal receives a [unique identifier](#unique-identifier) from a forum moderator with an increasing number. This identifier will follow the proposal through all stages of the governance process. The Identifier follows the form: SGP - 0000 (SGP stands for Shimmer Governance Proposal). The unique identifier is taken from the [public Notion page](https://shimmergov.notion.site/18af77a6634f4d9d91b7c16d9f294fbd?v=dcd7703eac1e4dd3b5302bf533546cb3).
- The proposal contains a [poll](https://meta.discourse.org/t/how-to-create-polls/77548) created by the [proposal submitter](#governance-proposal-submitter-phase-1). This poll must always include the option “Make no changes”.
- Besides the option “make no changes”, the poll can only contain one or two different other options. So it is either a “Yes / No changes” or an “Option 1 / Option 2 / No changes” vote.
- The text of the whole proposal and poll is not allowed to be edited in phase 2 after the moderators approved it.
- Poll duration must be set to 7 days
- Poll option “limit voting to these groups” must be set to: [trust_level_1 & trust_level_2 & trust_level_3 & trust_level_4]
- Poll option “Show results” must be set to “Always visible.”
- Editing any proposal or poll text is only allowed in the first 5 minutes after publishing the text. The forum settings block further editing of posts.
- If the proposal submitter becomes aware of an error in the text after these initial 5 minutes, he can request that the post gets removed by a moderator by posting a public comment with this request and tagging the @Governance_moderator group under the topic.
- Resubmittal of a corrected proposal version in phase 2 is only possible on the next proposal round (The first or 3rd Monday of a month) and after a moderator approves the corrected post.
- Accepted phase 2 polls will be announced by the official [Shimmer Governance Twitter account](https://twitter.com/ShimmerGov) and reposted by the Shimmer network main account run by the IF.

##### Requirements to win a phase 2 poll in the forum and qualify to process to phase 3

- The Poll must receive a minimum of 100 votes in favor of the proposal.

##### Requirements to close a proposal in phase 2

- If the minimum votes are not reached in the specified time, the phase 2 poll is marked [declined] and archived in the [Proposal archive](https://govern.iota.org/c/shimmer-governance-proposals/proposal-archive/55) category by a moderator
- The proposal can be closed and archived at any time by written request of the proposal submitter to a governance forum moderator.

### 4.6 Phase 3 - Voting

The final decision if we shall change a parameter in the Shimmer network is conducted through a Sybill-protected and transparent network-wide vote asking the whole community of Shimmer token holders to make a decision. All other phases before this vote are just steps to get feedback on community sentiment on an idea and do not have any binding character. But a phase 3 vote in Firefly has protocol-wide consequences and represents a binding decision by the community.

The IOTA community has developed a technical solution for the [BUILD vs. BURN](https://blog.iota.org/iota-treasury-vote-how-to-take-part/) Treasury vote. Firefly and the Hornet nodes are also prepared to conduct these votes in the Shimmer network using the same technology.

The [process](https://github.com/iota-community/treasury/blob/main/specifications/hornet-participation-plugin.md) created for the Build vs. Burn vote already has functionalities implemented to protect the vote from the influence of short-time speculators by using a time-based build-up of voting weight and has proven to be efficient and user-friendly.

For a network-wide vote by all token holders, all required voting preparations must be in place before a phase 3 vote gets announced. These preparations include creating a [participation event](#participation-event) by the proposal submitter (forum moderators can support upon request of the Proposal submitter) that can be implemented into Hornet nodes. This participation event is based on the [specifications](https://github.com/iota-community/treasury/blob/main/specifications/hornet-participation-plugin.md) designed for the Treasury vote.

The participation event needs to be merged by a forum moderator or admin into the respective [Github branch reserved for Shimmer voting participation events](https://github.com/iota-community/Shimmer-governance-participation-events/tree/master/events/vote) before the phase 3 vote can be announced, so that node operators can implement it from this repository.

In this stage, it is required that two forum moderators or one moderator and one admin double-check that all requirements are in place to approve publishing the phase 3 vote announcement. Merging the event in the GitHub repository requires merging rights. These rights can be given to the forum moderators but currently reside with @antonio.nardella and @Phylo.

A forum moderator publishes an [announcement post](#the-announcement-forum-post-in-phase-3-uses-this-template) under the [Phase 3 vote announcement](https://govern.iota.org/c/shimmer-governance-proposals/phase-3-vote-announcements/54) subcategory stating that the proposal has successfully passed the requirements to be implemented as a vote in Firefly. The announcement post includes a link to the phase 2 discussion and states the time and date when the Firefly phase 3 vote begins. This post is “locked” without options to comment and only serves as information to the community.

The same announcement will also be posted on the [Shimmer Governance Twitter account](https://twitter.com/ShimmerGov), which the moderators run.

##### The announcement forum-post in phase 3 uses this template:

_[Phase 3] Shimmer Governance Vote announcement:_

_The proposal [unique identifier and title] has reached soft consensus by the community in the governance forum phase 2 poll [link to the phase 2 poll]. It has fulfilled all requirements to be presented to the community in a governance vote using the Shimmer Firefly Wallet._

_The vote in your Shimmer Firefly Wallet will begin on [date and time in UTC] with a seven-day pre-vote phase during which you can cast your vote before the counting phase begins._

_The seven-day counting period during which you are required to hold your Shimmer tokens in the vote to receive your maximum possible votes will begin on [date and time in UTC]._

_The voting process will end on [date and time in UTC]_

_[Governance vote title] [unique identifier]:_

_Question: [copy text from the participation event]_

_Answer 1: [copy text from the participation event]_

_Answer 2: [Make no changes]_

_Node operators that want to participate in counting this vote can add the participation event to their nodes from this link: [link to the raw event hosted in Github]._

##### Proposal Acceptance Requirements Phase 3

- [Successful phase 2 poll](#requirements-to-win-a-phase-2-poll-in-the-forum-and-qualify-to-process-to-phase-3)
- The Proposal Submitter has created a [participation event](#participation-event) in [Github](https://github.com/iota-community/Shimmer-governance-participation-events) containing the JSON file for the vote, following the [specifications](https://github.com/iota-community/treasury/blob/main/specifications/hornet-participation-plugin.md) described in the IOTA Treasury vote process.
- The name of the participation event file in Github must begin with the [unique identifier](#unique-identifier) of the proposal - given by a forum moderator, followed by the proposal title.
- The text of the participation event in the “additional info” section must contain the URL of the phase 2 post in the governance forum so that voters in Firefly have the direct link to review the proposal and all discussions that did lead to the vote.
- The text of the “vote question” in the participation event must begin with the unique identifier of the proposal following the form
  - SGP - xxxx: _(followed by the Text of the proposal question)_
- One “answer” in the participation event must be “Make no changes.”
- The text of questions and answers is identical to the text used in the phase 2 poll for the question and answers
- Vote Duration: The created participation event used in the vote must contain seven day “commencing” period starting on the milestone that defines Thursday 01:00 pm UTC, directly followed by a 7-day “counting” period.
- Accepted phase 3 votes will be announced by the official [Shimmer Governance Twitter account](https://twitter.com/ShimmerGov) and by the Shimmer network main account, which the IF runs.

##### Requirements to win a phase 3 vote

- The option that wins the phase 3 vote in Firefly must receive a result with a [simple majority](#simple-majority) of votes counted for this option by the hornet nodes participating in the counting. The phase 3 vote must reach a quorum of 5% of the [maximum achievable votes](#maximum-achievable-votes) (based on the [circulating supply](#total-supply--circulating-supply) of Shimmer & the defined counting period in milestones) to be accepted as valid.
- The number of circulating Shimmer tokens used to calculate the vote results is based on the circulating supply of Shimmer at the milestone “counting start.”
- If the simple vote majority achieved in the vote signals the result, “Make no changes”, the proposal will not be accepted and will be considered closed and rejected.

### 4.7 Counter proposals

We may see that some specific topics will receive intensive discussions, and there may be fractions that strongly oppose a proposed change. In that case, a group might want to address the same topic with an entirely different approach. If this is the case, they may create a counter-proposal opposing a discussed proposal. Such a counter proposal must be named as a proposal that aims to counter an already existing proposal by its proposal submitter by calling it “counter-proposal” and adding a link to the proposal it opposes.

A counter-proposal will lead to the situation that a phase 2 poll will need to be conducted with both proposed solutions as voteable options (the original proposal and the counter-proposal) to decide which of the two will be presented to Voters in Firefly.

This means that once a proposal has reached enough support in phase 1 and would move to phase 2, the moderators will need to check if an active counter-proposal is submitted. If no counter-proposal is submitted, the proposal will go through the normal process of phase 2.

If a counter-proposal has been published and submitted, a runoff poll between the proposals will be conducted if the following conditions are met:

##### Conditions for the runoff poll

- The counter-proposal reaches the required 50 likes/votes in Phase1 during the seven-day poll timeframe that the original proposal spends in phase 2. In that case, the runoff poll will be started directly (on the same day) after the initial phase 2 poll has finished successfully (meaning the original proposal has reached 100 votes in favor of the proposal).
- This runoff poll will only contain the original proposal and the runoff proposal(s) as options in the poll and will not include the “Make no changes” option.
- If the counter-proposal fails to receive enough likes until the original proposals phase 2 poll is finished, the counter-proposal has failed, and the original proposal will go the usual way towards phase 3 (if all requirements are met)
- The counter-proposal will be deemed as declined when:
  - It fails to receive 50 votes/likes in phase 1, while the original proposal resides in the seven-day phase 2 poll.
  - It fails to receive more votes in a runoff poll than the original proposal.
  - It fails to receive more than 100 votes in a runoff poll.
- If declined, the topic addressed in the counter-proposal can only be resubmitted following the rules stated under the [resubmittal delay guidelines](#guaranteeing-stability---resubmital-delay).

If the counter proposal qualifies for a runoff poll in phase 2, the moderators will create a special post in the [Phase 2](https://govern.iota.org/c/shimmer-governance-proposals/phase-2-temperature-check/53) category. This post in phase 2 will include all proposals (original as “Proposal 1” and counter-proposals as “Proposal 2”, “Proposal 3,” etc.)

The option that wins this runoff poll with a simple majority of votes and fulfills the set requirement of a minimum of 100 supportive votes will be the winner and move to phase 3.

### 4.8 Seasons

We divide a year into four governance seasons, three months each.

Season's start and end dates will be set as follows:

- **Season 1: 2022/10/01 - 2022/12/31**
- **Season 2: 2023/01/01 - 2023/03/31**
- **Season 3: 2023/04/01 - 2023/06/30**
- **Season 4: 2023/07/07 - 2023/09/30**

Season numbers will further increase following the above schedule.

#### Purpose of the seasons

##### Guaranteeing stability - Resubmital Delay

Once a decision has been made by the community in phase 3, and it has not been subject to any emergency proposal, we deem the decision final and will implement the change. Changes need to have enough time to prove if they have the intended effect; therefore, a direct submittal of a proposal that intends to change the recently made decision must be declined.

- A proposal declined in a phase 3 governance vote cannot be resubmitted in the same season again. This includes all similar proposals that speak to the same topic or follow the same intent as the declined proposal.
- Also, proposals that intend to revert a decision taken in a successful phase 3 vote fall under this category and must follow the same rules.
- Only after the start of a new season a proposal that speaks to the same topic or follows the same intention can be submitted as a phase 1 discussion and has to pass the defined governance process successfully.
- If the proposal topic succeeds through phase 1 and phase 2 but is declined a second time in phase 3 by the community, the waiting time for resubmittal is increased to 2 seasons. Failing this again in the phase 3 vote leads to a 4 season resubmittal delay which is the maximum delay time. This means a topic with the same intent can only be brought up one year later again as a phase 1 proposal if it has been declined three times in a phase 3 vote.
  - **Declined one time: Resubmital Delay 1 Season**
  - **Declined two times: Resubmital Delay 2 Seasons**
  - **Declined three times and more: Resubmital Delay 4 Seasons**

##### Allowing flexible parameter change by soft consensus in phase 2

As we are just starting with governance in the Shimmer network, we believe that specific parameters of this framework need to be open to changes through a process **that does not involve all token holders in every decision** directly. This is why we have defined that the first two seasons will be used as a “probation period”.

During this probation period, forum moderators can change specific parameters by agreeing to the changes in a vote between the moderators with a 2/3rd majority and then proposing the change as a phase 1 discussion. After passing a successful phase 2 poll in the forum, the changes can be implemented without the need to facilitate a phase 3 vote. Only the forum moderators can submit these proposals.

A moderator must update all parameters in the table [parameters under probation](#specification-parameters-under-probation) to become effective.

To avoid confusions and situations where rules seem unclear to the community, we will host seasonal specification votes, where all changes that have been done in the current season or are planned for the next season will need to pass the proposal process, and a phase 3 vote by all token holders to be implemented. If this vote is successful, the changes made before using the probation rules will be officially accepted. Github and the IOTA Wiki will be adjusted to reflect these changes.

This means that the governance moderators can change specific parameters during a season but need confirmation from all voters to establish these changes permanently for the next season.

The proposal that involves all the parameter changes needs to be published **30 days before the end of a season** as a phase 1 discussion posted by a governance moderator in the forum.

The moderators must agree on the proposal before publishing it with a 2/3rd majority vote.

The probation period for parameter soft consensus changes can be extended for additional two seasons in the proposal that establishes the governance specification for season 3.

##### Specification parameters under probation

The following parameters of this framework specification can be adjusted by a moderator proposal and a successful phase 2 poll in the forum:

<table>
  <tbody>
    <tr>
      <td>
        <strong>Parameter</strong>
      </td>
      <td>
        <strong>Current value</strong>
      </td>
    </tr>
    <tr>
      <td>Minimum required proposal likes in phase 1
      </td>
      <td>50 likes
      </td>
    </tr>
    <tr>
      <td>Minimum required positive votes in a poll phase 1
      </td>
      <td>50 votes in favor of a proposal
      </td>
    </tr>
    <tr>
      <td>Minimum required positive votes in a poll phase 2
      </td>
      <td>100 votes in favor of a proposal
      </td>
    </tr>
    <tr>
      <td>Required majority to win in a poll in phase 1
      </td>
      <td>none
      </td>
    </tr>
    <tr>
      <td>Required majority to win in a poll in phase 2
      </td>
      <td>none
      </td>
    </tr>
    <tr>
      <td>Poll duration Phase 2
      </td>
      <td>7 days
      </td>
    </tr>
    <tr>
      <td>Trust level 1 metrics
      </td>
      <td>tl1 requires topics entered: 3
        <p>tl1 requires read posts: 3</p>
        <p>tl1 requires time spent mins: 25 min</p>
      </td>
    </tr>
    <tr>
      <td>Emergency proposal phase 2 poll duration
      </td>
      <td>48 hours
      </td>
    </tr>
    <tr>
      <td>Emergency proposal phase 2 poll required positive votes
      </td>
      <td>200 votes in favor of the proposal
      </td>
    </tr>
    <tr>
      <td>Cooldown duration after phase 3 vote
      </td>
      <td>7 days
      </td>
    </tr>
    <tr>
      <td>Season interval
      </td>
      <td>3 months
      </td>
    </tr>
    <tr>
      <td>Time a phase 2 proposal must be submitted in advance to the moderators to be included in the next phase 2 poll round
      </td>
      <td>24 hours before the next phase 2 round begins (Monday 4 pm UTC)
      </td>
    </tr>
    <tr>
      <td>Automatical closing of topics after inactivity for xx days
      </td>
      <td>30 days
      </td>
    </tr>
    <tr>
      <td>Moderator tasks and responsibilities
      </td>
      <td>As defined in the section 4.3  [Governance Forum Moderators][tasks and responsibilities]
      </td>
    </tr>
  </tbody>
</table>

### 4.9 Timing / Planning of proposals and votes

We have seen in many other projects that it can become challenging for community members to follow a Governance Process and stay up to date with several proposals floating around in different phases.

A good suggestion brought up by the community and used in other DAOs already is implementing fixed and defined "voting days". This should make it possible for those who want to contribute and participate in governance to check on new proposals and execute their voting rights regularly.

**_Remember the timings for the different phases laid out above_**

- A discussion in phase 1 is open-ended and has no defined time limits.
- A temperature check poll in phase 2 lasts seven days.
- After this poll is finished, voting in Firefly needs to be prepared.
- The preparation for this (participation event creation, node preparations) may take two to three days.
- One Moderator approval in the forum is required to move a proposal from phase 1 to phase 2. From phase 2 to phase 3, a minimum of two moderators (or one mod and one admin) must approve, which may also sometimes take a day.

**_Therefore, the following fixed times when phase 2 polls and phase 3 votes begin are set_:**

- A **phase 2 temperature check poll** can only begin on the…
  - **The 1st and 3rd Monday** of a month before 4 pm UTC and will last seven days. A moderator ensures that the poll gets published these days.
- The **network-wide phase 3 votes** of all tokens holders with Firefly starts…
  - **Every 2nd and 4th Thursday** of a month at 1 pm UTC with the “commencing” phase of the participation event. The total duration of phase 3 is 14 days (seven days commencing, seven days counting). The phase 3 announcement post can be published by a moderator after the phase 2 poll has ended successfully and the participation event for the phase 3 vote is created and approved on GitHub.
- Phase 3 votes will be officially announced in a tweet by the Shimmer Twitter account to reach most community members. A Forum admin will forward the information to the IF comms department.

This leads to a simple-to-follow schedule:

- Vote on polls in the Forum happen on the **1st and 3rd Monday of a month.**
- Firefly votes of these proposals happen **on the Thursday following the end of a phase 2 poll.**

### 4.10 Execution of a decision - cooldown period

We need to implement a cool-down phase after a decision in Firefly (phase 3) has been taken. During this period, the execution of the voted changes rests.

There are two important reasons to wait a certain amount of time before we will execute a decision:

- **Ragequitting**: Voters that do not agree with the majority decision must have a reasonable time to leave. If someone cannot agree and does not want to continue being part of the project, this person can sell the owned Shimmer tokens and leave the project before the change they do not agree with will happen.
- **Emergency moves:** In case any formal errors, flaws, or security risks get uncovered during or after a decision.

  An ongoing phase 3 vote that has reached the network-wide Firefly voting cannot be stopped. The event exists in the network, and votes are counted by the nodes already. Experiences in other projects have shown that sometimes errors happen even if everyone acted according to a predefined plan. We cannot take human mistakes out of account.

**Suppose this:** During an ongoing phase 3 vote, the community encounters that the vote would lead to a result whose consequences have been unknown to the voters at the beginning of the voting process. Or a former unknown security risk is discovered that would be implemented if the action proposed in the vote is performed.

In that case, a mechanism should be in place to stop a vote from being executed. I suggest that in such cases, the community can request to initiate a [phase 3 emergency proposal](#411-phase---3-emergency-proposals) to prevent the current voted proposal from being executed.

To implement an emergency move, a certain time delay must exist between the end of a phase 3 vote and the execution of the actions decided in this vote. In such a cooldown period, or already during the ongoing vote, the community can propose [emergency actions](#411-phase---3-emergency-proposals).

This cooldown period is **seven days**.

These seven days act as a security buffer to avoid accidentally implementing decisions that would harm the network and also leave enough time for everyone who cannot accept the decision taken in the vote to leave the network by selling the tokens.

Suppose no emergency proposal that successfully declines the outcome of the previous vote during these seven days is initiated. The decision of a phase 3 vote will be deemed final, binding, and implemented as proposed.

If an emergency proposal has been accepted during the seven-day cooldown period, the execution of the decision is postponed until the result of the emergency proposal is verified.

### 4.11 Phase - 3 Emergency proposals

An emergency proposal must be implemented as a phase 3 vote event within the seven-day cooldown period of the vote decision it seeks to stop. Therefore, such an emergency proposal does not require passing phase 1 and only requires **48 hours of phase 2 poll**.

If this poll reaches the required votes, the emergency proposal can be directly implemented as a phase 3 vote in Firefly.

Two Forum moderators must check if an emergency proposal fulfills the Acceptance Requirements and approve and implement this proposal in phase 2. It is up to the emergency [proposal submitter](#governance-proposal-submitter-phase-1) to inform the Shimmer community and urge them to look into the proposal and participate in the poll.

##### Acceptance Requirements Emergency proposals

- [Emergency proposal] post created in the governance forum tagged with “emergency proposal”. The text describes the motivations of the initiators and the exact reasons why the community should not implement the result of the ongoing vote it aims to cancel.
- The post contains the link to the phase 3 vote announcement of the vote it seeks to cancel.
- Identifies the challenged proposal by the unique identifier of this proposal.
- The emergency proposal is given a unique identifier from a forum moderator with an increasing number. The Identifier follows the form: SEP-0000 (SEP stands for Shimmer Emergency Proposal).
- The emergency [proposal submitter](#governance-proposal-submitter-phase-1) has created a participation event in [Github](ttps://github.com/iota-community/Shimmer-governance-participation-events) containing the precisely defined JSON for the emergency vote following the [specifications](https://github.com/iota-community/treasury/blob/main/specifications/hornet-participation-plugin.md) described in the Treasury vote process.
- The text of the participation event in the “additional info” section must contain the URL of the phase 3 announcement post in the governance forum so that voters in Firefly have the direct link to review all discussions that did lead to the vote.
- The text of the emergency proposal must begin with the unique identifier of the emergency proposal following the form
  - SEP-0000: _(followed by the Text of the proposal question)_
- There are only two voteable options allowed in an emergency proposal:

  - "Accept this emergency proposal! Do not execute proposal (unique identifier)" and
  - “Decline this emergency proposal.”

- The emergency proposal starts as a phase 2 poll with a poll duration of 48 hours.
- This poll must reach 200 votes in favor of the option “Accept this emergency proposal! Do not execute proposal (unique identifier)” to be moved further into a phase 3 vote
- If the poll fails to reach enough votes in favor of the proposal, the emergency proposal is declined and will be archived by a moderator

##### Requirements for a successful emergency move against a proposal

- A result with the simple [majority](https://en.wikipedia.org/wiki/Majority) (50% + 1) of votes counted for the option "Accept this emergency proposal! Do not execute proposal (unique identifier)" is required for an emergency proposal to pass the vote successfully
- To qualify as a binding decision that cancels an already conducted or ongoing vote, an emergency proposal vote must, to be successful, reach higher participation of votes than the winning option of the phase 3 vote. Participation is based on the metric “[average votes per milestone”](#average-votes-per-milestone)

Read some examples about emergency proposal votes in this section [Here are some examples to clarify the principles used:](#here-are-some-examples-to-clarify-the-principles-used-for-the-emergency-proposal)

### 4.12 Governance proposal template (phase 2 & 3 & emergency proposal)

[This is the template](https://docs.google.com/document/d/1EDfwbxR3vxOisdLcZOCriHc3Lxhj5mHd2GTPzt7LWd4/edit?usp=sharing) for proposals in the governance forum. It is required for proposals in phase 2 and phase 3 of the process. The purpose is to provide a unified structure, so proposals follow a predefined form.

#### Unique identifier

- A unique number will follow the proposal through all process stages, starting with phase 2. The Unique identifier follows the standard:
  - SGP - 0000 (**S**himmer **G**overnance **P**roposal), or
  - SEP - 0000 (**S**himmer **E**mergency **P**roposal)
  - The number is assigned by a Forum moderator, increasing the number +1 for every new accepted and published phase 2 proposal
  - All Unique identifiers will be hosted in a [public notion page](https://shimmergov.notion.site/18af77a6634f4d9d91b7c16d9f294fbd?v=dcd7703eac1e4dd3b5302bf533546cb3) hosted by the forum moderators

#### Simple Summary

- You don't understand it well enough if you cannot explain it simply. Provide a simplified and layman-accessible explanation of the suggested change

#### Abstract

- A short (~200 word) description of the issue being addressed. (What is the problem?)

#### Motivation

- Motivation is critical for proposals, especially if they want to change the Governance process. (why do we need this?)

#### Specification

- The specification should describe the syntax and semantics of any new feature. The specification should be detailed enough to allow for it to be reasoned about by the community. (What is the new state of the system parameters after the change?)

#### Rationale

- The rationale clarifies the specification by describing what motivated the design and why the proposer made particular design decisions. It can describe alternate procedures that were considered and related work. The rationale may also provide evidence of the consensus within the community and discuss significant objections or concerns raised during the discussion that lead to the published version of the proposal. (why have the proposed changes been chosen, and how do the proposed changes solve the described problem?)

#### Implementation

- The section should include any implementation dependencies and potential timelines. What is needed to consider the process finalized and implemented? Who needs to act in a specific manner to implement the changes?
- It includes the texts and milestone numbers for a [participation event](#participation-event) used in the phase 3 Firefly vote. The text for “question” and “answer” must be identical to the text used in the poll

#### Vote Name, question, answer, and optionally additional information

- Write down the exact text that the poll question, the answers in the forum poll, and the potential vote in the Firefly wallet should state. Remember that one vote option must be “Make no changes”.
- The text you put here cannot be changed once the phase 2 poll has been approved and published by a moderator in the forum and must be 100% clear, understandable, and syntactically correct. Follow the example below. You can copy it and exchange the example text with your texts.

### 4.13 Hosting of the specification in Github

- This framework will be hosted on the IOTA Wiki Github under [this repository:](https://github.com/iota-wiki/iota-wiki/tree/main/shimmer/learn/Governance).
- Starting with Season 1, the specification agreed on by the voters in the Phase 3 vote will be hosted as the “main” branch of the repository.
- Any changes that happened during a season based on the [parameters under probation](#specification-parameters-under-probation) rules will be added as a pull request.
- Once the voters have accepted the specification for the next season in a phase 3 vote, the community managers will merge the pull request containing the changes into the “main” branch.
- Pull requests should be made by the governance moderators. Reviewers are welcome, and the Community managers will do merges if the vote approves the new specification.
- Every seasonal specification will be saved as individual files in the repository to achieve a persistent history.
- The IOTA / Shimmer Wiki will always display the state of the “main” branch.

### 4.14 Hosting of the participation events for Governance votes on GitHub

All [participation events](#participation-event) for governance votes in the Shimmer network are hosted in the following repository:

- [https://github.com/iota-community/Shimmer-governance-participation-events](https://github.com/iota-community/Shimmer-governance-participation-events)

A [proposal submitter](#governance-proposal-submitter-phase-1) needs to create the participation event for the phase 3 vote of a proposal as a pull request against this repository and add a new file to this folder:

- [https://github.com/iota-community/Shimmer-governance-participation-events/tree/master/events/vote](https://github.com/iota-community/Shimmer-governance-participation-events/tree/master/events/vote)

The participation event needs to be named with the [unique identifier number](#unique-identifier) given by a forum moderator.

Once a proposal has successfully passed the phase 2 poll. A forum moderator will merge the pull request of the participation event into the main branch and announce the phase 3 Firefly vote. Node operators can pick up the event under the provided link (part of the announcement) and add it to their nodes.

## 5. Rationale

#### The reasoning behind the chosen metrics in the proposal process

**Phase 2 poll:**

- Of course, we must know that the forum is not a fully Sybil-protected environment. We have several measures provided by the discourse engine to avoid bots and Sybils entering the forum. Still, sophisticated and knowledgeable users can find ways to avoid those measures and create sybill accounts in the forum. A phase 2 poll is always only a sentiment check in the community and represents a non-binding decision. It is not suitable to make final decisions on a topic. This can only happen in a phase 3 vote in Firefly.

**Counter proposal process:**

- We have discussed several options for this process. Ultimately, we agreed that it is a legit tool to offer the chance for opposing opinions to be heard. We removed the option “make no changes” from the runoff poll because of the following reason:
- The runoff poll will only start if the original proposal has already successfully passed a phase 2 poll (so it received enough supporting votes) - adding the option? Make no changes” into the runoff poll could lead to the situation that the first legit decision (original post won the phase 2 poll) will be canceled if the runoff poll ends with a majority for “make no changes.”
- Removing the option ensures that the Token holders will get the chance to decide on this topic.

**Emergency proposal process:**

**The “Participation” metric**

- The [average number of counted votes](#average-votes-per-milestone) per milestone is the essential metric here because of the nature of the currently used voting system. The number of votes counted increases steadily with the time passed in a vote (every 10 seconds, new votes are added based on used tokens).

- This makes average votes per milestone the only reasonable metric to follow here. It directly measures participation. Therefore shows us if a large number of voters are interested in executing an emergency decision.
- We don't want this emergency rule to enable a small group of voters to overthrow the consensus in the community. So an emergency motion must be the last resort and not easy to execute successfully. But also needs to give a reasonable metric to clearly state that even if the total number of votes reached is lesser (because the timeframe for counting will likely be less), the movement in the community was stronger in favor of the emergency vote.
- Participation is, in our opinion, the best metric to reason about the legitimacy of such an emergency decision. We must accept that an ongoing vote cannot be stopped or reverted.

  So, even if everyone who voted in favor of the uncovered flaw first would stop voting once a flaw is uncovered or change his vote to the option "make no changes", it would be possible that the option which introduces a flaw would still achieve a majority vote and therefore needs to be implemented.

  We will likely see that most votes will not reach very high participation. This is why a passing quorum of 5% for an average vote might be the way to go (it can always be increased if we want). An emergency proposal that brings up a valid argument can likely activate a much bigger group of community members that feel the need to stop this.

- An emergency move against a proposal must prove that the community realized the decisions taken in the vote it aims to cancel were wrong. Therefore only strong participation can show this. It could be thought about defining specific metrics for an emergency proposal to succeed besides having higher participation like
  - Participation must be xx% higher than the participation of the vote it counters
  - Reach a minimum quorum of max. Achievable votes of 10% (compared to 5% in a normal phase 3 vote)
  - A 2/3rd majority of votes could be required instead of an absolute majority.
  - We can visit such ideas in the future

#### Here are some examples to clarify the principles used for the emergency proposal

_Assume that during the ongoing Firefly vote (let's call it Vote A), some people step forward and declare that the execution of the vote will result in a dangerous network configuration and provide some data that they feel is sufficient to prove their claims. Let's observe two different sample scenarios and how the framework would handle them._

#### Scenario 1

A strong movement in the community against Vote A after the issue is discovered. Many voters feel this needs to be stopped and vote accordingly in favor of the emergency proposal with high participation.

**Vote A:**

- SMR circulating supply: 1.000.000 SMR
- counting period chosen: 5000 milestones
- cooldown period: 500 milestones
- maximum achievable votes: 1.000.000 SMR x 5000 milestones = 5.000.000.000 votes
- required quorum to pass the vote successfully (5% of max. achievable votes): 250.000.000 votes
- Result from vote A:
  - Option 1 - 1.750.000.000 votes,
  - Option 2 - 120.000.000 votes.
  - Option 1 would be a valid winner (simple majority and quorum rules passed) and will be executed after seven days of cooldown
  - **Participation in Option 1:**
    - **Average votes per milestone = 350.000 votes/milestone**

**Emergency vote against Vote A:**

- SMR circulating supply: 1.000.000 SMR
- counting period: 5000 milestones
- maximum achievable votes: 1.000.000 SMR x 5000 milestones = 5.000.000.000 votes
- Result from the emergency vote:
  - Option 1 (stop vote A) 3.250.000.000 votes
  - Option 2 (no changes) 1.125.000.000 votes
  - **Participation in Option 1:**
    - **Average votes per milestone = 650.000 votes/milestone**

**Final Result:**

- In the emergency vote, the option to cancel Vote A achieved the majority of votes. Also, it earned higher participation with more average votes per milestone (650.000 > 350.000) than the winning option of vote A.
- **The result of Vote A is therefore invalidated by the emergency vote. It will not be executed because more voters have rejected the result of Vote A in the emergency proposal.**

#### Scenario 2

Some people feel that the issue is a big problem and initiate the emergency proposal. Still, most others do not see it as an issue, dont care, and abstain from participating in the emergency proposal.

**Vote A:**

- SMR circulating supply: 1.000.000 SMR
- counting period: 5000 milestones
- cooldown period: 500 milestones
- maximum achievable votes: 1.000.000 SMR x 5000 milestones = 5.000.000.000 votes
- required quorum to pass the vote successfully (5% of max. achievable votes): 250.000.000 votes
- Result from vote A:
  - Option 1 - 1.750.000.000 votes,
  - Option 2 - 120.000.000 votes.
  - Option 1 has passed the quorum and the simple majority rule. It would be a valid winner and will be executed after seven days of cooldown.
  - **Participation in Option 1:**
    - **Average votes per milestone = 350.000 votes/milestone**

**Emergency vote against Vote A:**

- SMR circulating supply: 1.000.000 SMR
- counting period: 5000 milestones
- maximum achievable votes: 1.000.000 SMR x 1300 milestones = 5.000.000.000 votes
- Result from the emergency vote:
  - Option 1 (stop vote A) 500.000.000 votes
  - Option 2 (no changes) 450.000.000 votes
  - **Participation in Option 1:**
    - **Average votes per milestone = 100.000 votes/milestone**

**Final Result:**

- Option 1 in the emergency vote achieved the majority of votes but did not reach higher participation in average votes per milestone (100.000 &lt; 350.000) than the winning option of vote A
- **The result of Vote A stays valid and will be executed. The emergency proposal has not achieved enough participation to counter the decision in vote A, even if a majority of voters in the emergency proposal have voted in favor of the emergency proposal.**

## 7. Glossary

##### Participation event

A JSON file containing all required information to display a vote in Firefly and used to count the votes in the hornet nodes. It defines specifically

- Unique Identifier of the proposal
- Name of the proposal
- the text of the vote question
- The text of all possible answers
- The milestone when the pre-vote period starts (milestoneIndexCommence)
- The milestone when the counting period starts (milestoneIndexStart)
- The milestone when the counting period ends (milestoneIndexEnd)
- Potential additional information texts if they have been part of the poll texts in phase 2

The exact definition of the participation event can be found here: [https://github.com/iota-community/treasury/blob/main/specifications/hornet-participation-plugin.md](https://github.com/iota-community/treasury/blob/main/specifications/hornet-participation-plugin.md)

An example of how such an event file looks like is the event we used for the BUILD/BURN vote: \
[https://github.com/iotaledger/participation-events/blob/master/events/vote/governance_01.json](https://github.com/iotaledger/participation-events/blob/master/events/vote/governance_01.json)

##### Simple Majority

- For a binary decision, “yes/no” or “Option A/ Option B” it is the option that receives more cast votes than the other option. (51 of 100)
- For a decision with more than two options, it is the option that receives the most casted votes of all available options (100 total cast votes: A = 23, B = 32, C = 45 - where C is the simple majority winner)

##### Maximum achievable votes

- The number of votes that would theoretically be possible to count if
  - 100 % of all circulating tokens would participate in the vote during all milestones that the counting period consists of (milestoneIndexStart until milestoneIndexEnd)
  - Calculated as Total token supply x number of milestones in the counting period
  - The maximum achievable votes are based on the circulating supply of tokens on milestoneIndexStart of the votes counting period.

##### Average votes per milestone

- The number of tokens voting on an option of a vote per milestone
- It is calculated as the number of total votes counted for an option divided by the total amount of milestones the counting period holds.
- Measures participation

##### Total supply / circulating supply

- The number of coins already created, minus any coins that have been burned.

##### Maximum supply

- The number of coins that have ever been created, including coins that have already been burned

## 8. Recommended readings, knowledge library

- [Library of DAO Tools & Governance frameworks](https://www.notion.so/f11f6bb9a4ee4f90855794dfd8d28927?v=a6eb959920f54452a4e2dd13e21e6104)
- [Library of high-level Governance Research papers](https://www.notion.so/bf9572db4a65414a8bfd08909fa31580?v=3d336999fc9a46f582ebfc4500b53de8)
- [Collection of recommended articles and readings around DAO’s](https://www.notion.so/DAO-recommended-articles-bd07c25ef4974f5096a09e6babe82a9a)
- [Collection of DAO & Governance focussed Podcasts and Videos](https://www.notion.so/bf56e6c56dd542f984c1366f807cebd8?v=dbec62901b014d478a5dd6c307d59c0b)
- [IOTA DAO Pioneers learning circle Session Documents](https://github.com/iota-community/DAO-Pioneers#-iota-dao-pioneers-initiative)


---
# Exhibit B - Procedure B: The Shimmer Community Grant Committee

*This is the full specification for all operational processes and ordinary and usual decisions concerning business affairs of the Company while operating the Shimmer Community Grant Committee. Detailed rules and procedures are defined here.*
---

## Shimmer Community Grant Committee - Operation Specification

The Shimmer Community Treasury Grant Committee was established in the Governance Votes [SGP-005](https://govern.iota.org/t/sgp-0005-shimmer-community-treasury-grant-committee/1576), the committee members got selected in [SGP - 001](https://govern.iota.org/t/sgp-0001-shimmer-community-grant-committee-lead-selection/1544/1) and [SGP - 002](https://govern.iota.org/t/sgp-0002-shimmer-community-grant-committee-grant-reviewer-selection/1546) by the Shimmer Token holders.
The Committee received a budget of 27.204.307 SMR for one year of operation from the 181.362.051 SMR large Community Treasury. This article contains the operation specification under which the elected committee members operate and steward the received budget.

## 4. Specification

### _Mission of the Shimmer Community Grant Committee:_

_A community-led committee-based grant program to support the Shimmer network and empower its ecosystem_

### 4.1 The Committee

**The committee will be set up with five members**.

One of them is the **Program Lead**, which, besides reviewing funding requests, takes care of all administrative tasks and reporting and coordinates the committee members' work.

- The Lead also promotes the Program, identifies directions for funding, and has a thought leadership role in guaranteeing the Program's success.
- The Lead is directly involved in grant reviews and decides which team of reviewers should work on a proposal.
- Further, an important part is ongoing coordination with the second ecosystem funding program run by the Tangle Ecosystem Association and the Shimmer Growth Committee to ensure effective alignment in the goals and directions of the community grants program.
- The Lead organizes the regular public meetings of the Grant Committee and takes care of reporting for financial transparency and fund usage.
- The Lead will act as first public contact for anyone that wants to approach the committee besides funding requests.
- The Program Lead will be contracted by Marshal Island DAO LLC (to be set up) which acts as the legal body of the Program and offers limited liability and the needed legal structure to ensure a safe operation.
- To establish this contract the Program Lead is required to have its own legal entity (company, LLC, GmbH, etc) setup in its home juristriction that will engage in the contract with the MIDAO LLC.
- The Lead will be compensated via invoices of max 11200 USDT per month on a 40-hours-per-week basis and will sign a 12-month service provider contract.

**The 4 Grant Reviewers will process funding requests on a part-time basis**.

- The committee operates a 3 of 5 Gnosis multi-signature wallet that requires 3 out of 5 signatures for any operation (like spending funds or adding or removing members).
- The Lead will assign reviewers to work on proposals based on their qualifications, experience, and availability.
- Grant reviewers will operate on a service provider contract basis with the Marshal Island DAO LLC.
- Grant reviewers will be compensated with 50 USD (net) per hour for a maximum of 40 hours per month / 10 hours per week submitted via invoice to the DAO LLC.
- The committee members will select one of the four reviewers as the **Co-Lead**. The Co-Lead acts on behalf of the Committee Lead in cases of sickness, holidays, or leaving. If the Lead resigns, the Co-Lead continues the operation and organizes an election of a new Lead through a community vote.
- If the Programm Lead is unavailable/sick/on leave and the Co-Lead needs to fill this position, the Co-Lead will be compensated for this extra time and can invoice more than 10 hours per week.

**This proposed Grant Program will run for 12 months.** Decisions to continue or end the Program will have to be made one month before the current period ends to enable a graceful shutdown of operations or a transition into the next period. (Costs of operational shutdown need to be secured)
The 12 months period will start on the day when the Firefly vote (Phase 3) results to establish this committee have been community verified and publicly announced.

**The community may replace members** during the Program's period at any time through a governance vote following the process described in the [Shimmer Governance Framework](./the-shimmer-governance-framework.md).

- Need for replacements may occur if committee members find they cannot dedicate sufficient time to the Program. If they ask for a replacement for personal reasons, or if the community has valid concerns about the motivation and professionality of a member or has any proof of fraud, betrayal, or violation of terms.
- Grant reviewers are free to leave the position based on the terms stated in their contract. A 4-week prior notice is required before leaving the committee.
- In case of serious violation of terms of the contract, like a breach of NDA, insider trading, or not disclosed conflict of interest, reviewers will be immediately discarded from the committee position by the committee lead and removed as signers of the multisig wallet.
- Replacement positions will be offered to the runner-up candidates of the committee selection process (Phase 3 results).

### Requirements for Committee members:

- All committee members will do KYC to reveal and verify their identity and sign a legally binding contract (employment or service provider) with the DAO LLC.
- All committee members must reveal any potential conflicts of interest to become committee members. They need to indicate if they currently are or have been in the past part of a team in a DLT project or have other connections or affiliations to projects or groups that could cause a conflict of interest. A conflict of interest policy needs to be accepted and signed.
- To ensure a committee structure that provides different views and makes decisions as unbiased as possible, the maximum number of committee members from a Project Team is limited to **one member per Team**. A Project Team, in this sense, is defined as any organization that causes a conflict of interest by being affiliated as a team member or earning a salary, payment for services, or commission from the project.
- A committee member cannot be involved in evaluating any proposal that would cause a conflict of interest. Other grant reviewers will handle such cases without involving the member that has the conflict. Conflicts of interest are not exclusion criteria for committee members in general; those conflicts need to be disclosed to the Committee Lead. The Program Lead will then exclude the reviewer from the decision-making process for specific grants that would cause a conflict of interest.
- The Programm Lead and the Co-Lead are prohibited from holding any paid position within a Crypto project.
- All members will sign NDAs and Insider Trading disclosures.
- All Committee members are required to operate the Gnosis Multi-Signature Wallet with a Ledger Nano or similar device.

### Selection process for committee members and the Program Lead:

- Please review [the selection process specification](https://govern.iota.org/t/community-grant-committee-selection-proccess-specification/1436) that describes the community-driven selection process
- Phase 1 started on 6 November 22 - you can check the applications here:
  - [Grant Committee Lead applications](https://govern.iota.org/c/shimmer-governance-proposals/shimmer-community-treasury-coommittee-lead-appli/59)
  - [Grant Reviewer Applications](https://govern.iota.org/c/shimmer-governance-proposals/community-treasury-grant-reviewer-applications/58)
- Phase 2 started on 9 December 22 - you can see the Poll and results here:
  - [SGP - 0001 Shimmer Community Grant Committee - Lead selection](https://govern.iota.org/t/sgp-0001-shimmer-community-grant-committee-lead-selection/1544)
  - [SGP - 0002 Shimmer Community Grant Committee Grant Reviewer selection](https://govern.iota.org/t/sgp-0002-shimmer-community-grant-committee-grant-reviewer-selection/1546)

### 4.2 Funding Priorities

#### Funding objectives:

- To increase the utility of the Shimmer network and attract new builders.
- To promote Shimmer and make it more visible and attractive in the DLT space.
- To enable projects to establish successful and profitable business models on Shimmer.

#### Target areas for grant funding:

- Applications and integrations (front-ends, Defi, Gaming, and other applications that use the Shimmer protocol on L1 or L2)
- Incentivizing established successful projects from different ecosystems to deploy their application on the Shimmer network
- Developer tooling
- Open source software development using Shimmer technology
- Analytics tools and dashboards
- Community Education
- Marketing and outreach initiatives
- Code audits
- Events, Community meetups, and hackathons
- Bounties

### Guiding principles for funding decisions:

1. **A proposal must be relevant to the Shimmer network and its ecosystem.**
2. **A proposal that segregates individuals, organizations, or communities based on sex, race, color, ethnic or social origin, genetic features, language, religion or belief, political or any other opinion, membership of a national minority, property, birth, disability, age or sexual orientation.**
3. **The committee will prioritize projects with the highest potential and positive impact on the ecosystem compared to the received funding.**
4. **The proposer or team must be capable of delivering the proposed project. Evaluating this is the responsibility of the committee.**
5. **All funded projects must be open source (under [MIT](https://opensource.org/licenses/MIT), [GNU](https://www.gnu.org/licenses/gpl-3.0.en.html) or [Apache 2.0 license](https://opensource.org/licenses/Apache-2.0)). Projects in development must allow the grant committee to access any private repos for review. These projects will only receive 50% of the proposed budget untill they fully open-sourced their code.**
6. **The requested budget must match industry standards for comparable tasks. If a proposal requests way above fair market value, the committee will dialogue with the team to request adjustments. The committee may either reject such a proposal or cut the funding to settle at fair market value.**
7. **If a project has already received funding from the Tangle Ecosystem association, it cannot receive funding from the Community Treasury for the exact scope of work again. But, the committee can grant additional funding for extensions or further developments of such a project.**
8. **A proposal that creates any conflict of interest from members of the proposing team or committee members must be reported to the committee Lead. Committee members with conflicts of interest cannot process, comment, or vote on a proposal.**
9. **Any attempts of Bribery or offer of future payments, token ownership, or compensations/gifts of any form to committee members will lead to the immediate cancellation of a proposal process. Accepted bribes by committee members will lead to the immediate removal of the members from the committee.**

### 4.3 Application and approval process:

**Easy and quick access to funding** is essential to a successful grant program. Numerous examples in the space have shown that this is one of the most critical reasons teams consider when choosing a network.

### Funding Tiers and requirements:

As long as the market cap of Shimmer is low, we need to take a considerably more secure approach in the early stages. Therefore, we should define a threshold based on the Shimmer market cap, which will lead to the halt of funding, the start of financing with low tiers, and the switch to regular tiers.

- No grants are given out as long as the Market cap of Shimmer is **below 50 Million USD**
- Grants will be given out with **low Tier values** if the market cap of Shimmer is **between 50 and 100 million USD**
- Grants will be given out with the **Regular Tier values** if the market cap of Shimmer is **above 100 million USD**
- **Tier 1 - up to 5.000 USD**: Two reviewers handle the proposal and approve or decline it within two business days after submission. KYC is required for one member of the project teams (the Grant submitter needs to do KYC and be a signer). The reviewers will decide based on the provided data in the application and especially consider if the submitter has a positive history in our community. As soon as funding is approved, the proposal will be funded within two business days after KYC is completed.
- **Tier 2 - Low Tier 5.000 - 25.000 / Regular Tier 5.000 - 50.000 USD**: Two reviewers review the proposal. KYC is required for one member of the project teams (the Grant submitter needs to do KYC and be a signer). Projects considered to be approved can be invited to conduct a 1-hour interview with the reviewers of the proposal. A minimum of two milestones will be defined, and payments will happen based on these milestones. After completing the KYC process, the committee can pay up to 50% of the requested funding upfront.
- **Tier 3: Low Tier 25.000 - 100.000 / Regular Tier 50.000 - 200.000 USD**: Same requirements as the previous tier apply. The Project Team must do KYC (3 members do KYC, including the Grant submitter and Project Team Lead, that will be the signer, and the 3rd Person decided by the Grant Committee Lead). Additionally, applications need approval by the entire grant committee. Projects considered to be approved will be invited to present the idea in an extensive live interview with two grant reviewers and the Program Lead. A minimum of three milestones are defined, and payments happen based on these milestones.

  If the project is accepted, the Program Lead will assign one of the reviewers as a project steward. The steward is responsible for keeping close contact and doing regular (minimum every two weeks) checks with the project team. Milestones are reviewed by the steward and approved by the committee Lead. After completing the KYC process, the Program can pay 30% of the requested funding upfront.

- **Tier 4: Low Tier 100.000 - 250.000 / Regular Tier 200.000 - 500.000 USD:** The entire grants committee will review those applications—same procedure as in Tier 3. The Project Team must do KYC (3 members do KYC, including the Grant submitter and Project Team Lead, that will be the signer and the 3rd Person decided by the Grant Committee Lead). The final decision if the project receives funding will happen in a **vote by all token holders**.
  - Suppose the grants committee supports that the community shall fund a Tier 4 application; it forwards this application to the community as a proposal in the governance forum and asks for approval by the community in a vote by all Shimmer token holders.
  - The proposal in the governance forum will be submitted by the committee lead and includes the project team's full proposal and a detailed statement by the grant committee on why it recommends funding this proposal. Such a proposal will enter the governance process as a Phase 2 Poll in the Governance Forum.

### 4.4 Application and scoring process

The teams must provide the following details in an [**application questionnaire form**](https://www.shimmergov.community/airtable-proposal-form):

**Proposal Title**

**Project Owner Name**

- Applicant Name (Full legal name)

**Project Owner email**

**Wallet address for payments**

- Binance Chain USDT address as long as Shimmer has no native USDT Stable Coin

**About the Team**

- Number of Team Members
- Details per member (write about every Team member. Education and work experience, link to relevant portfolios)
- Legal Status (No status, individual, incorporated)
- Country of the establishment (if legally established)

**About the Project** (Write about your project - idea, use cases, process, goals, and how it helps our ecosystem)

- Project Name
- Project Links
- Project Details (Write details about your project - requirements, deliverables, and milestones - as detailed as possible.)

**Project Goals** (Write about what your team plans to achieve with this project)

- Project Milestone 1,2,3,etc
- Expected Milestone Reward in USDC (How much money would you need to achieve this milestone)

**Funding & Budget Breakdown** (How much money would you need in total, and explain how you would spend this money if your application is accepted)

- Funding Ask in USDC
- Funding Breakdown (Write about how you plan to use the funds in your project, i.e., marketing, developers, etc.)

**Open source:**

- Will you publish the source code of your project under an open-source license (under [MIT](https://opensource.org/licenses/MIT), [GNU](https://www.gnu.org/licenses/gpl-3.0.en.html) or [Apache 2.0 license](https://opensource.org/licenses/Apache-2.0))?

**Previous Funding**

- Has the Team / the project previously received funding from another grant-giving program? If yes, please provide details.
- Has the Team / the project currently applied at other grant-giving programs? If yes, please provide details.

**Other Information:**

- Telegram Handle: (All Team members)
- Discord Handle: (All Team members)
- Whitepaper (if available)
- Pitch deck (if available)
- GitHub repository (if applicable)
- GitHub handles of Team members (if applicable)
- Other social media accounts operated by the team or the team members.

**Category?** (Please put exactly: DeFi, DAOs, NFT, Gaming, Enterprise, Metaverse, Tooling, Infrastructure, Marketing, Outreach, Education, Event, Hackathon, Social, Other)

### **Grant evaluation scoring system:**

**Grant reviewers will use a scoring system to evaluate funding proposals.**

| **Scoring Qualities**                         | **Outstanding (4 points)**                                                                                                                                                     | **Good (3 points)**                                                                                                                                                                              | **O.K (2 points)**                                                                                                                         | **Needs Improvement (1 point)**                                                                                                           | **Missing or Extremely Low Quality (0 points)**                                                          | **Score (out of 4)** |
| --------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------- |
| **Relevance to the Shimmer/IOTA Ecosystem**   | The project is very relevant to the Shimmer/IOTA Ecosystem and exclusively builds on the Shimmer Network. They may currently have an MVP on Shimmer already.                   | The project is relevant to the Shimmer Ecosystem and either builds exclusively on Shimmer or plans to deploy later onto IOTA Mainnet as a second instance.                                       | The project is somewhat relevant to the Shimmer/IOTA Ecosystem, and the Shimmer network is a main network of choice, but not the only one. | The project treats Shimmer as one of many chains and doesn't seem loyal to the Shimmer/IOTA network.                                      | The project shows no signs of Shimmer development or doesn't seem to be faithful to building on Shimmer. |                      |
| **Plan and Funding Model**                    | The team has clear, realistic expectations on their milestones and how the funding will move the team closer to these goals. They follow the expectations of the grant system. | The team has somewhat clear, realistic expectations on their milestones and how the funding will move the team closer to these goals. They somewhat follow the expectations of the grant system. | The team has clear, descriptive expectations of their milestones but are not entirely realistic.                                           | The team has a semblance of expectations for their milestones, but they are unrealistic.                                                  | The team has no clear vision of what funds would be used for.                                            |                      |
| **Execution**                                 | Several critical steps have already been taken toward their project goals. This could be seen in the form of a significant MVP, high traction, etc.                            | Some critical steps have been taken toward their project goals. Their MVP is currently being built with signs or some sort of traction.                                                          | Initial critical steps have been taken (interesting website, socials, etc.), and it seems like a decent project, but extremely early.      | Initial steps taken are poorly executed or sloppy. If there are socials (Twitter, Discord, etc.), their following looks inorganic (fake). | The team has taken no steps to execute their project.                                                    |                      |
| **Verifiability and Quality of the Team**     | Team is doxxed, and we can easily verify backgrounds. The team is also high quality and seems capable, trustworthy, and ready to take action on the project.                   | The Team is somewhat doxxed, and backgrounds are decently easy to verify. They are trustworthy.                                                                                                  | The team is somewhat doxxed, but verifying background information may not be easy. They are more trustworthy than not.                     | The team is somewhat suspicious and hard to verify.                                                                                       | The teams' background and information cannot be verified or is fake.                                     |                      |
| **Overall Quality & Originality of the Idea** | The project is unique and would greatly impact the Shimmer ecosystem.                                                                                                          | The project would significantly impact the Shimmer ecosystem and is decently unique.                                                                                                             | The project would somewhat impact the Shimmer ecosystem as a whole and is somewhat unique.                                                 | The project would have little impact on the Shimmer ecosystem as a whole and is somewhat unique.                                          | The project/idea is a copycat or extremely weak.                                                         |                      |
|                                               |                                                                                                                                                                                |                                                                                                                                                                                                  |                                                                                                                                            |                                                                                                                                           |                                                                                                          | Total: x/20          |

**A project should reach a particular score to be eligible for certain funding Tiers:**

- **Tier 4** (Funding budget 200.000 - 500.000 USD) - required score **minimum 17 of 20**
- **Tier 3** (Funding budget 50.000 - 200.000 USD) - required score **minimum 15 of 20**
- **Tier 1 & 2** (Funding up to 50.000 USD) - required score **minimum 13 of 20**

### Possible Extra Scoring Points:

- Projects offer 0,5% of the projects total token supply to go to the community Treasury: **one extra point can be granted.**
- Projects offer 1% of the projects total token supply to go to the community Treasury: **two extra points can be granted.**
- Projects offer more than 1,5% of the projects total token supply to go to the community Treasury: **three extra points can be granted.**

**This does not imply that automatically such an offer will lead to granting the extra points. Granting these additional points is decided on a case by case basis.**

[**JD Sutton has built a Notion Database for this selection process**](https://airtable.com/shrvZgn3NVsXLTXev/tblAzVWXeTSvUyZI3)

The scoring system is a guideline for reviewers. We understand that it may only sometimes apply to some kinds of projects.

We reserve the ability to place specific projects into different tiers even if point scoring disagrees. Still, this scoring system should apply to the majority of projects.

**The grants committee will present all accepted Tier 1, Tier 2, Tier 3, and Tier 4 applications in a public meeting (weekly or once demand exists) in the IOTA / Shimmer Discord, where the community is invited to ask questions and get insights into the evaluation and decision-making process.**

**All decisions by the grant committee will be published without naming the individual grant committee members who worked on a proposal to avoid becoming vulnerable to potential complaints and attacks from declined projects.**

The committee will host a publicly accessible database (Notion) where all accepted proposals are listed, and all spending can be tracked by the community (including the respective Links to Stablecoin Payouts)
[**Proposed structure example by JD Sutton**](https://www.shimmergov.community/treasury-expenses)

### Complaint process:

Should a project feel it has been treated unjustly by a decision of the grant committee, it should first contact the Programm Lead and try to resolve the issue. If that is not successfull the project can open a complaint thread in the Governance forum and lay out the reasons for the complaint respectfully to the community.
If a Grant Reviewer is also a Governance Forum Moderator, this moderator is excluded from any moderation activities in this specific forum conversation.

### 4.5 The Budget

**Budget for 12 months of operation**

- The Budget for the committee spending during 12 months is 15% of the SMR community Treasury tokens currently held in [this address](https://explorer.shimmer.network/shimmer/addr/smr1qrmakyqt5ezm5k9c0sk39gwfavpktxkjmx0jvh9ejxjq6pr6d39egv2mvuc).
- **15% of this 181.362.051 SMR will be 27.204.307 SMR available for the committee to spend on grants and cover all operational costs.**
- The committee will operate a MultiSig Wallet, supplied with fractions/ monthly allocations of SMR tokens from the community wallet (currently operated by TEA) to the Multisig.
- The committee will pay monthly salary in stablecoin USDT or USDC to the Project Lead and payout compensation to Grant reviewers based on monthly invoices. It will be responsible for handling this efficiently and transparently.
- Six months of salary required for the Project Lead (67200 USD) will be converted from SMR to USDT at the beginning of the program period and again after the first six months of operation.
- The committee will convert the potential max compensation for the grant reviewers (24.000 USD if four reviewers do 10 hours a week) from SMR to USDT quarterly.
- Liquidating those tokens on the exchange shall happen in small amounts controlled by the committee and randomized in time and quantity. (Crypto finance custody potentially an option)
- Once a project has been approved for funding, the committee will convert the amount of Shimmer tokens approved for this project into USDT so that the financing of this project is guaranteed. Market volatility should not impact project funding and Reviewer compensation.
- The needed legal costs and expenses around the setup of the Marshal Island DAO LLC and the potential shutdown costs at the end of the program operations will be covered by the Community Treasury.
- Any excess funds left in the Committee's MultiSig Wallet towards the end of the 12 months will be sent back to the Community Treasury wallet by the committee members in case the community decides not to continue the Program.

### 4.6 The legal entity

The committee members must have a legal status to be aligned with all regulations and operate on safe, legal grounds.

- We propose to start this Grant committee under the umbrella of the Tangle Ecosystem Association until the legal entity in the Mashal Islands has been fully set up. The Tangle Ecosystem Association has agreed to sign service provider contracts with the Committee members to let them start operating as a Grant Committee once the vote has passed.
- Once the legal entity has been fully established, the Committee Lead and the Grant reviewers will sign Service Provider contracts with the Marshal Island DAO LLC and receive legal liability protection from the entity based on these service contracts.
- All committee members will be KyC'd and can be made responsible if any misbehavior occurs based on their contractual terms.

This setup will enable a regulated and lawful grant-giving committee that can be held accountable and operates under a transparent and regulated status.

**Registration & costs**

Setup Fee: 9500 USD
Annual Fee: 5000 USD

### 4.7 Program success metrics

**Measurable criteria:**

- Growth in the number of grants applications received quarter-over-quarter
- Growth in the number of projects, ideas, and events funded
- Growth in community engagement (e.g., increased activity on Discord, Forum, Twitter followers, etc.)
- Growth in Shimmer market capitalization that is driven by applications/projects funded via grants (e.g., increased TVL in the EVM Chain, increased amount of daily/weekly active users, increase in daily active addresses in the Shimmer network and the EVM Chain, increased value transferred due to apps funded by grants)

The committee will provide reports on these metrics every six months.

### 4.8 Changes to this Framework

Once this Framework has been accepted through a public vote by the Shimmer token holders, the process or daily work for the members of the Treasury committee can begin. Even if we now think that we have designed a comprehensive and very well-working set of rules under which the committee members can carry out the grant-giving activities, the committee members may conclude that specific points described in this Framework need changes to operate better and more effectively.
The committee members will be the only ones who can correctly identify the need for such changes. Therefore, we would limit the group of Persons that can propose changes to the specifications described in the document to the five elected Committee members.

- **The following points are open to changes by all community members via the official Shimmer Governance process:**

  - Proposal to replace/remove a Grant Reviewer
  - Proposal to replace/remove the Programm Lead
  - Proposal to terminate and shutdown the Shimmer Community Treasury Grant Committee
  - Proposal to extend the operation period of the Shimmer Community Treasury Grant Committee
  - Proposal to add additional funding to the budget of the Shimmer Community Treasury Grant Committee

- All changes to other points described under **Specification (Point 4.1 - 4.8)** of this document can only be proposed by a member of this Shimmer Community Treasury Committee (Programm Lead and the four elected Grant Reviewers) through a public proposal in the Governance forum following the process laid out in the Shimmer Governance Framework.


