# Projects & SDK Protocol Compatibility

## Table of contents

- [Abstract](#abstract)
- [Protocol Version Compatibilities](#protocol-version-compatibilities)
  - [Icon Status Attribution](#icon-status-attribution)
  - [Elephant: Protocol v0.5.?.?](#)
  - [Dragon: Protocol v0.4.?.?](#)
  - [Cow: Protocol v0.3.0.2](#cow-protocol-v0302)
- [Projects Status Updates](#projects-status-update)
- [Tests](#tests)
- [References](#references)
- [History](#history)

## Abstract

This document aims to group technical features of Milestones in the Catapult Protocol Development project and assess/update status reports about specific Software Development Kits compatibility.

This document may be moved to a nemtech repository in case it is deemed necessary. For the time being the document should provide with an easy aggregation of all features addressed in the protocol project during milestones development and should provide a clear compatibility table for individual protocol features / or changes.

## Protocol Version Compatibilities

### Icon Status Attribution

Following table describes the status attributions for each of the icons that will be used in the protocol features compatibility tables:

| Icon | Status |
| :-: | :-: |
| :question: | Investigation/Research is currently in progress. |
| :white_check_mark: | Feature is available. |
| :o: | Work in Progress (WIP) |
| :stop_sign: | Feature is not available. |

### Elephant: Protocol v0.5.?.?

| feature | server@0.4.?.? | rest@? | sdk-js@? | sdk-java@? | sdk-python@? | sdk-unity@? | sdk-php@? |
| :-: |:-: | :-: | :-: | :-: | :-: | :-: | :-: |
| mosaic levy | :question:  | :stop_sign:  | :stop_sign:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |
| metadata key-value| :question:  | :stop_sign:  | :stop_sign:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |

### Dragon: [Protocol v0.4.?.?](https://github.com/nemtech/catapult-server/milestone/5)

| feature | server@0.4.?.? | rest@? | sdk-js@? | sdk-java@? | sdk-python@? | sdk-unity@? | sdk-php@? |
| :-: |:-: | :-: | :-: | :-: | :-: | :-: | :-: |
| hashlock with alias | :question:  | :stop_sign:  | :stop_sign:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |
| optin cosigners | :question:  | :white_check_mark:  | :white_check_mark:  | :stop_sign:  | :white_check_mark: | :stop_sign: | :stop_sign: |
| lightning network | :question:  | :stop_sign:  | :stop_sign:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |
| consensus PoS+ | :question:  | :stop_sign:  | :stop_sign:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |
| new harvesting | :question:  | :stop_sign:  | :stop_sign:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |

### Cow: [Protocol v0.3.0.2](https://github.com/nemtech/catapult-server/milestone/3)

| feature | [server@0.3.0.2](https://github.com/nemtech/catapult-server/releases/tag/v0.3.0.2) | [rest@0.7.14](https://github.com/nemtech/catapult-rest/releases/tag/v0.7.14) | [sdk-js@0.11.5](https://github.com/nemtech/nem2-sdk-typescript-javascript/releases/tag/v0.11.5) | [sdk-java@0.9.0](https://github.com/nemtech/nem2-sdk-java/releases/tag/v0.9.0-beta) | sdk-python@? | sdk-unity@? | sdk-php@? |
| :-: |:-: | :-: | :-: | :-: | :-: | :-: | :-: |
| catbuffer | :white_check_mark:  | :stop_sign:  | :stop_sign:  |  :stop_sign: | :o: | :stop_sign: | :stop_sign: |
| mosaic/namespace split | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :o:  | :white_check_mark: | :stop_sign: | :stop_sign: |
| aliases | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :o:  | :white_check_mark: | :stop_sign: | :stop_sign: |
| receipts | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :stop_sign: | :stop_sign: | :stop_sign: | :stop_sign: |
| account props | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |
| fees | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| delegated harvesting | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |
| cow DTOs | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  |  :o: | :stop_sign: | :stop_sign: |
| secret locks hash algos | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :stop_sign: | :stop_sign: | :stop_sign: |
| hashlock | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :white_check_mark:  | :white_check_mark: | :stop_sign: | :stop_sign: |
| merkle proofs | :white_check_mark:  | :white_check_mark:  | :stop_sign:  | :stop_sign:  | :stop_sign: | :stop_sign: | :stop_sign: |

## Projects Status Updates

Following table describes status updates of Projects grouped in different _special interest groups_ as defined in following repository:

  - https://github.com/nemtech/community

| Project | Milestone | Version Tag | Comment |
| :-:  | :-: | :-: | :-: |
|**SIG-api** | | | |
| [catapult-server](https://github.com/nemtech/catapult-server) | Cow | [v0.3.0.2](https://github.com/nemtech/catapult-server/releases/tag/v0.3.0.2) | |
| [catapult-rest](https://github.com/nemtech/catapult-server) | Cow | [v0.7.14](https://github.com/nemtech/catapult-rest/releases/tag/v0.7.14) | |
| [catbuffer](https://github.com/nemtech/catbuffer) | Cow | N/A | |
| [nem2-library-js](https://github.com/nemtech/nem2-library-js) | Cow | [v0.9.14](https://github.com/nemtech/nem2-library-js/releases/tag/v0.9.14) | |
| [nem2-sdk-typescript-javascript](https://github.com/nemtech/nem2-sdk-typescript-javascript) | Cow | [v0.11.5](https://github.com/nemtech/nem2-sdk-typescript-javascript/releases/tag/v0.11.5) | |
| [nem2-sdk-java](https://github.com/nemtech/nem2-sdk-java) | Alpaca | [v0.9.0-beta](https://github.com/nemtech/nem2-sdk-java/releases/tag/v0.9.0-beta) | |
| [nem2-sdk-csharp](https://github.com/nemtech/nem2-sdk-csharp) | Alpaca | N/A | |
|**SIG-client** | | | |
| [nem2-cli](https://github.com/nemtech/nem2-cli) | Cow | [v0.11.1](https://github.com/nemtech/nem2-cli/releases/tag/v0.11.1) | Not all features are implemented. |
| [nem2-prototyping-tool](https://github.com/nemtech/nem2-prototyping-tool) | Alpaca | N/A | Depends on SDK update.|
|**SIG-docs** | | |
| [nem2-docs](https://github.com/nemtech/nem2-docs) | Cow | N/A| |
| [nem2-curricular-framework](https://github.com/nemtech/nem2-curricular-framework) | Alpaca | N/A| |
| [nem2-workshop-nem-applied-to-supply-chain](https://github.com/nemtech/nem2-workshop-nem-applied-to-supply-chain) | Alpaca | N/A | Depends on SDK update. |
| [nem2-workshop-document-notarization](https://github.com/nemtech/nem2-workshop-document-notarization) | Alpaca |  N/A | Depends on SDK update. |
|**SIG-testing** | | | |
| [nem2-scenarios](https://github.com/nemtech/nem2-scenarios) | Bison | N/A | |
| [test-vectors](https://github.com/nemtech/test-vectors) | N/A | N/A | |
|**SIG-tooling-infra** | | |  |
| [catapult-service-bootstrap](https://github.com/nemtech/catapult-service-bootstrap) | Cow | [v0.3.0](https://github.com/tech-bureau/catapult-service-bootstrap/releases/tag/v0.3.0) | |
| [nem2-camel](https://github.com/nemtech/nem2-camel) | N/A | N/A | |

## Tests

TBD

## References

- `catapult-server`: https://github.com/nemtech/catapult-server
- `catapult-rest`: https://github.com/nemtech/catapult-rest
- `catbuffer`:  https://github.com/nemtech/catbuffer
- `nem2-sdk-typescript-javascript`: https://github.com/nemtech/nem2-sdk-typescript-javascript
- `nem2-sdk-java`: https://github.com/nemtech/nem2-sdk-java

## History

| **Date**      | **Version**   |
| ------------- | ------------- |
| Apr 25 2019    | Initial Draft |
