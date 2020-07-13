---
gip: 1
title: GIP Purpose and Guidelines
status: IMPLEMENTED
author: Stefan Ionescu (@stefanionescu)
discussions-to: https://discord.gg/bRmTxxW
created: 2020-07-10
updated: 2020-07-13
---

## What is an GIP?

GIP stands for GEB Improvement Proposal. It has been adapted from the EIP (Ethereum Improvement Proposal) and the SIP (Synthetix Improvement Proposal). The purpose of this process is to ensure changes to the GEB framework are transparent and well governed. A GIP is a design document providing information to the Reflexer community about a proposed change to GEB. The author is responsible for building consensus within the community and documenting dissenting opinions.

## GIP Rationale

We intend GIPs to be the primary mechanisms for proposing new features, collecting community input on an issue, and for documenting the design decisions for changes to GEB. Because they are maintained as text files in a versioned repository, their revision history is the historical record of the feature proposal.

It is highly recommended that a single GIP contain a single key proposal or new idea. The more focused the GIP, the more successful it is likely to be.

A GIP must meet certain minimum criteria. It must be a clear and complete description of the proposed enhancement. The enhancement must represent a net improvement.

## GIP Work Flow

Parties involved in the process are the *author*, the [*GIP editors*](#gip-editors), the core team and the Reflexer community.

:warning: Before you begin, vet your idea, this will save you time. Ask the Reflexer community first if an idea is original to avoid wasting time on something that will be rejected based on prior research (searching the Internet does not always do the trick). It also helps to make sure the idea is applicable to the entire community and not just the author. Just because an idea sounds good to the author does not mean it will have the intend effect. The appropriate public forum to gauge interest around your GIP is [the Reflexer Discord].

Your role as the champion is to write the GIP using the style and format described below, shepherd the discussions in the appropriate forums, and build community consensus around the idea. Following is the process that a successful GIP will move along:

```
[ DRAFT ] -> [ LAST CALL ] -> [ APPROVED ] X [ DELAYED ] -> [ IMPLEMENTED ] X [ REJECTED ]
```

Each status change is requested by the GIP author and reviewed by the GIP editors. Use a pull request to update the status. Please include a link to where people should continue discussing your GIP. The GIP editors will process these requests as per the conditions below.

* **Draft** -- Once the champion has asked the Reflexer community whether an idea has any chance of support, they will write a draft GIP as a [pull request]. Consider including an implementation if this will aid people in studying the GIP.

* **Last Call** -- If agreeable, GIP editor will assign the GIP a number (generally the issue or PR number related to the GIP) and merge your pull request. The GIP editor will not unreasonably deny a GIP. Proposed GIPs will be discussed on community calls and in Discord. If there is a reasonable level of consensus around the change on the community call the change will be moved to approved. If the change is contentious the final decision may be delayed until the first GEB is launched on mainnet Ethereum.

* **Approved** -- This GIP has passed community governance and is now being debated by the core team.

* **Delayed** -- This GIP will be re-analyzed after the core team deploys the first GEB on mainnet Ethereum.

* **Implemented** -- This GIP has been implemented and deployed to mainnet.

* **Rejected** -- This GIP has failed to reach community consensus.

## What belongs in a successful GIP?

Each GIP should have the following parts:

- Preamble - RFC 822 style headers containing metadata about the GIP, including the GIP number, a short descriptive title (limited to a maximum of 45 characters), and the author details.
- Simple Summary - “If you can’t explain it simply, you don’t understand it well enough.” Provide a simplified and layman-accessible explanation of the GIP.
- Abstract - a short (~200 word) description of the technical issue being addressed.
- Motivation (*optional*) - The motivation is critical for GIPs that want to change Reflexer. It should clearly explain why the existing specification is inadequate to address the problem that the GIP solves. GIP submissions without sufficient motivation may be rejected outright.
- Specification - The technical specification should describe the syntax and semantics of any new feature.
- Rationale - The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.
- Test Cases - Test cases may be added during the implementation phase but are required before implementation.
- Copyright Waiver - All GIPs must be in the public domain. See the bottom of this GIP for an example copyright waiver.

## GIP Formats and Templates

GIPs should be written in markdown format.

## GIP Header Preamble

Each GIP must begin with an [RFC 822](https://www.ietf.org/rfc/rfc822.txt) style header preamble, preceded and followed by three hyphens (`---`). This header is also termed ["front matter" by Jekyll](https://jekyllrb.com/docs/front-matter/). The headers must appear in the following order. Headers marked with `*` are optional and are described below. All other headers are required.

` gip:` <GIP number> (this is determined by the GIP editor)

` title:` <GIP title>

` author:` <a list of the author's or authors' name(s) and/or username(s), or name(s) and email(s). Details are below.>

` * discussions-to:` \<a url pointing to the official discussion thread\>

` status:` < DRAFT | LAST CALL | APPROVED | DELAYED | IMPLEMENTED | REJECTED >

` created:` <date created on>

` * updated:` <comma separated list of dates>

` * requires:` <GIP number(s)>

` * resolution:` \<a url pointing to the resolution of this GIP\>

Headers that permit lists must separate elements with commas.

Headers requiring dates will always do so in the format of ISO 8601 (yyyy-mm-dd).

#### `author` header

The `author` header optionally lists the names, email addresses or usernames of the authors/owners of the GIP. Those who prefer anonymity may use a username only, or a first name and a username. The format of the author header value must be:

> Random J. User &lt;address@dom.ain&gt;

or

> Random J. User (@username)

if the email address or GitHub username is included, and

> Random J. User

if the email address is not given.

#### `discussions-to` header

While an GIP is in Draft or Last Call status, a `discussions-to` header will indicate the mailing list or URL where the GIP is being discussed.

#### `created` header

The `created` header records the date that the GIP was assigned a number. Both headers should be in yyyy-mm-dd format, e.g. 2001-08-14.

#### `updated` header

The `updated` header records the date(s) when the GIP was updated with "substantial" changes. This header is only valid for GIPs of Draft and Active status.

#### `requires` header

GIPs may have a `requires` header, indicating the GIP numbers that this GIP depends on.

## Auxiliary Files

GIPs may include auxiliary files such as diagrams. Such files must be named GIP-XXXX-Y.ext, where “XXXX” is the GIP number, “Y” is a serial number (starting at 1), and “ext” is replaced by the actual file extension (e.g. “png”).

## GIP Editors

The current GIP editors are

` * Stefan Ionescu (@stefanionescu)`

` * Ameen Soleimani (@ameensol)`

## GIP Editor Responsibilities

For each new GIP that comes in, an editor does the following:

- Read the GIP to check if it is ready: sound and complete. The ideas must make technical sense, even if they don't seem likely to get to final status.
- The title should accurately describe the content.
- Check the GIP for language (spelling, grammar, sentence structure, etc.), markup (Github flavored Markdown) and code style

If the GIP isn't ready, the editor will send it back to the author for revision, with specific instructions.

Once the GIP is ready for the repository, the GIP editor will:

- Assign an GIP number (generally the PR number or, if preferred by the author, the Issue # if there was discussion in the Issues section of this repository about this GIP)

- Merge the corresponding pull request

- Send a message back to the GIP author with the next step.

Many GIPs are written and maintained by developers with write access to the GEB codebase. The GIP editors monitor GIP changes, and correct any structure, grammar, spelling, or markup mistakes they see.

## History

The GIP document was derived heavily from the EIP Ethereum Improvement Proposal and SIP Synthetix Improvement Proposal documents. In many places text was simply copied and modified. Any comments about the GIP document should be directed to the GIP editors.

July 10, 2020: GIP 1 has been drafted and submitted as a PR.

See [the revision history for further details](https://github.com/reflexer-labs/GIPs), which is also available by clicking on the History button in the top right of the GIP.

### Bibliography

[the Reflexer Discord]: https://discord.gg/bRmTxxW
[pull request]: https://github.com/reflexer-labs/GIPs/pulls
[Markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
[EIP]: https://github.com/ethereum/EIPs
[SIP]: https://github.com/Synthetixio/SIPs
[core team]: https://github.com/orgs/reflexer-labs/people

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
