# Clients Protocol Compatibility

## Table of contents

- [Abstract](#abstract)
- [Client Applications](#client-applications)
- [Features Compatibilities](#features-compatibilities)
  - [Icon Status Attribution](#icon-status-attribution)
  - [Wallets](#wallets)
  - [Explorer](#explorer)
  - [Faucet](#faucet)
  - [Command Line Interface](#command-line-interface)
- [History](#history)

## Abstract

This document aims to group technical features of Milestones in the Catapult Protocol Development project and assess/update status reports about specific **Clients** compatibility.

The document should provide with an easy aggregation of all features addressed in the protocol project during milestones development and should provide a clear compatibility table for individual protocol features / or changes.

## Client Applications

Following client applications are taken into account for this compatibility status update:

| Deliverable | Package Name |Repository URL |
| :-: | :-: | :-: |
| **Wallets** | | |
| Desktop Wallet | nem2-desktop-wallet | [nem2-wallet][wallet-desktop] |
| Mobile Wallet (RFP) | nem2-wallet-mobile | [nem-catapult-wallet][wallet-rfp] |
| Hardware Wallets Integrations | nem2-wallet-hardware | N/A |
| **Explorers** | | |
| Node/Block Explorer | nem2-explorer | [nem2-explorer][explorer] |
| **Faucet** | | |
| Catapult Faucet | nem2-faucet | [nem2-faucet][faucet] |
| **Command Line** | | |
| NEM2 CLI | nem2-cli | [nem2-cli][cli] |

## Features Compatibilities

### Icon Status Attribution

Following table describes the status attributions for each of the icons that will be used in the protocol features compatibility tables:

| Icon | Status |
| :-: | :-: |
| :white_check_mark: | Feature is available. |
| :heavy_minus_sign: | Not applies. |
| :stop_sign: | Feature is not available. |

### Wallets

Wallet packages are being worked on mostly by foundation teams. Following packages are target of the Stories table:

- [nem2-desktop-wallet][wallet-desktop]: **Wallet Desktop Build**, installable on major OSs.
- [nem-catapult-wallet][wallet-rfp] (RFP): **Outsourced** to Hatio.
- [nem2-cli][cli]

#### Stories

| User Story | [Command Line][cli] | [Desktop Wallet][wallet-desktop] | [Mobile Wallet][wallet-rfp] | [Hardware Wallet][wallet-hardware] |
| :-: | :-: | :-: | :-: | :-: |
| **Accounts** | | | | |
| User can create new account | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can create new HD account | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can create multiple accounts | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can name accounts | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can import private key | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can import pass phrase | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can export private key | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can export pass phrase | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can link account (harvesting) | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| Private key / Pass phrase storage is secure | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| | | | | | | |
| **Data Services** | | | | | | |
| User can view mosaic balances | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can view transaction history | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can view transaction details | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can view mosaic alias info | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can view account alias info | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can view multisig info | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can view account restrictions | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can view mosaic restrictions | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can view metadata | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can view block data | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can view receipts data | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User is notified about transactions | :white_check_mark:  | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User is notified about pending co-sigs |  :white_check_mark: | :stop_sign: | :white_check_mark: | :stop_sign: |
| User can view pending co-sigs | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can export transaction history | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can switch network _node_ | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can switch _network_ | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| | | | | | | |
| **Usability** | | | | | | |
| User can read QR Code | :heavy_minus_sign: | :stop_sign: | :white_check_mark: | :stop_sign: |
| User can export Account with QR Code | :heavy_minus_sign:| :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can export Transaction with QR Code (Invoices) | :heavy_minus_sign: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can switch _language_  | :stop_sign: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can use aliases for Mosaics | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can use aliases for Accounts | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| | | | | | | |
| **Transactions** | | | | | | |
| _User can issue Transaction URI*_ | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can specify transaction MAX_FEE | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Transfer without message | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can issue Transfer with message | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can issue Transfer with encrypted message | :white_check_mark: | :stop_sign: | :white_check_mark: | :stop_sign: |
| User can issue Transfer with persistent harvesting delegation | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Alias for mosaic | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Alias for account | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Aggregate Complete with multiple transfers | :heavy_minus_sign: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Aggregate Complete with custom transactions | :heavy_minus_sign: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Cosignature | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can issue Register Namespace | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Mosaic Definition | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Mosaic Supply Change | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Secret Lock | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Secret Proof | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Hash Lock | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| User can issue Multisig Account Modification | :white_check_mark: | :white_check_mark: | :stop_sign: | :stop_sign: |
| Multisig Account Modification requires opt-in | :white_check_mark: | :white_check_mark: | :white_check_mark: | :stop_sign: |
| User can issue Account Address Restriction | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Account Mosaic Restriction | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Account Operation Restriction | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Mosaic Global Restriction | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Mosaic Address Restriction | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Account Metadata |:white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Mosaic Metadata | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |
| User can issue Namespace Metadata | :white_check_mark: | :stop_sign: | :stop_sign: | :stop_sign: |

* **Due to the possibility of issuing Transaction URI, in fact any transaction type can be issued. Each transaction type is listed as to determine whether there is _screen to prepare_ said transaction types.**

### Explorer

The Explorer project is being worked on by a team in the foundation. The source code for this Software Package can be found at:

- [dev-block-explorer][explorer-mijin]
- [nem2-explorer][explorer]

#### Stories

| User Story | Dev Block Explorer | Explorer Framework |
| :-: | :-: | :-: |
| User can view account balances | :white_check_mark: | :white_check_mark: |
| User can view transaction history | :white_check_mark: | :white_check_mark: |
| User can view transaction details | :white_check_mark: | :white_check_mark: |
| User can view mosaic alias info | :stop_sign: | :white_check_mark: |
| User can view account alias info | :stop_sign: | :white_check_mark: |
| User can view namespace info | :stop_sign: | :white_check_mark: |
| User can view block history | :white_check_mark: | :white_check_mark: |
| User can view receipts data | :stop_sign: | :white_check_mark: |
| User can view merkle data | :white_check_mark: | :stop_sign: |
| User can export transaction history | :stop_sign: | :stop_sign: |
| User can view network nodes | :stop_sign: | :white_check_mark: |
| User can view node version | :stop_sign: | :white_check_mark: |
| User can view beneficiary info | :stop_sign: | :white_check_mark: |
| User can view account metadata | :stop_sign: | :white_check_mark: |
| User can view mosaic metadata | :stop_sign: | :white_check_mark: |
| User can view namespace metadata | :stop_sign: | :white_check_mark: |
| User can view account address restriction | :stop_sign: | :white_check_mark: |
| User can view account mosaic restriction | :stop_sign: | :white_check_mark: |
| User can view account operation restriction | :stop_sign: | :white_check_mark: |
| User can view mosaic global restriction | :stop_sign: | :white_check_mark: |
| | | |
| **Transactions** | | |
| User can view Transfer without message | :white_check_mark: | :white_check_mark: |
| User can view Transfer with message | :white_check_mark: | :white_check_mark: |
| User can view Transfer with encrypted message | :stop_sign: | :stop_sign: |
| User can view Alias for mosaic | :stop_sign: | :white_check_mark: |
| User can view Alias for account | :stop_sign: | :white_check_mark: |
| User can view details of Aggregate Complete with multiple transfers | :white_check_mark: | :white_check_mark: |
| User can view details of Aggregate Complete with custom transactions | :white_check_mark: | :white_check_mark: |
| User can view Cosignature | :white_check_mark: | :white_check_mark: |
| User can view details of Register Namespace | :white_check_mark: | :white_check_mark: |
| User can view details of Mosaic Definition | :white_check_mark: | :white_check_mark: |
| User can view details of Mosaic Supply Change | :white_check_mark: | :white_check_mark: |
| User can view details of Secret Lock | :white_check_mark: | :white_check_mark: |
| User can view details of Secret Proof | :white_check_mark: | :white_check_mark: |
| User can view details of Hash Lock | :white_check_mark: | :white_check_mark: |
| User can view details of Multisig Account Modification | :white_check_mark: | :white_check_mark: |
| User can view details of Multisig Cosignatory Modification | :white_check_mark: | :white_check_mark: |
| User can view details of Account Address Restriction | :white_check_mark: | :white_check_mark: |
| User can view details of Account Mosaic Restriction | :white_check_mark: | :white_check_mark: |
| User can view details of Account Operation Restriction | :white_check_mark: | :white_check_mark: |
| User can view details of Mosaic Global Restriction | :stop_sign: | :white_check_mark: |
| User can view details of Mosaic Address Restriction | :stop_sign: | :white_check_mark: |
| User can view details of Account Metadata | :stop_sign: | :white_check_mark: |
| User can view details of Mosaic Metadata | :stop_sign: | :white_check_mark: |
| User can view details of Namespace Metadata | :stop_sign: | :white_check_mark: |

### Faucet

The Faucet project was released by a community member. The source code for this Software Package can be found at:

- [nem2-faucet][faucet]

#### Stories

| User Story | Integration Status |
| :-: | :-: |
| User can request **currency** mosaic amount | :white_check_mark: |
| User can request custom mosaic amount | :white_check_mark: |
| User can install faucet on owned server | :white_check_mark: |
| User can specify custom mosaic faucet | :white_check_mark: |
| User can specify custom network faucet | :white_check_mark: |
| User can change amount settings | :white_check_mark: |
| User is confirmed with Captcha (no-bots) | :white_check_mark: |
| User can send link to send faucet coins | :stop_sign: |
| User can specify transaction MAX_FEE | :stop_sign: |

## History

| **Date**      | **Version**     |
| ------------- | --------------- |
| Jul 14 2019   | Initial Draft   |
| Sep 12 2019   | Second Update   |

[wallet-desktop]: https://github.com/nemfoundation/nem2-desktop-wallet
[wallet-mobile]: https://github.com/NemTechCN/nem2-mwallet-CN 
[wallet-rfp]: https://github.com/hatioin/nem-catapult-wallet.git
[wallet-hardware]: #
[explorer]: https://github.com/nemfoundation/nem2-explorer
[explorer-mijin]: https://github.com/nemtech/dev-block-explorer
[faucet]: https://github.com/nemfoundation/nem2-faucet
[cli]: https://github.com/nemtech/nem2-cli
