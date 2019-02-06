TODO: work in progress, check pt commit

# Overview

This document is a place holder for outlining notes and details gathered by community members that will influence an initial "base" wallet implementation.  Over time there will be multiple implementations from a web/desktop wallet, similar to a simplified nanowallet implementation for v2, as well as various "native" implementations for mobile platforms such as android and iOS.

The project will have a mix of dedicated and community part time resources participating in the effort. There are various partial to full one off efforts already underway in the community, we hope those interested will join in focused effort for the base implementation that other wallets can be built on top of and extended for custom/additive features, different user experience, as well as stripped down library and UI components that can be leveraged in custom applications where the notion of a wallet is more of a embedded approach with just a couple simple views and majority of the application is the end users/orgs custom solution.

## Project & Design Considerations

Some considerations that will need to be taken into account in regards to implementation at the library/sdk level, as well as a base user experience (UX) level.

### Library/SDK

While other SDKs exist currently the main supported SDK by the core project members is the [javascript/typescript SDK](https://github.com/nemtech/nem2-sdk-typescript-javascript).  With this being the case we will start with targeting an initial implementation that leverages this.  With this in mind this effort will consider how best to create simple additive libraries that work with the existing core js/ts SDK and where appropriate worth with the [sig-api group](sig-api/) if certain updates or additions are required or warranted to properly execute on this effort.

### User Interface (UI)

When working on the base wallet implementation it should be considered how to create a simple implementation that provides just the basics of the base protocol and usage, while leaving room for application developers to leverage the UI assets as base starting point for their implementations for "embedded" usage.  This same consideration and approach should exist for any language/platform implementation, but we will start with the base web/desktop wallet implementation while others follow.

For UI/app implementation we are currently considering:

* React
* Vue
* Angular

Based on the lead participants we will be choosing one as the initial implementation.

### Extensibility & Add-On Features

The current nanowallet implementation is more of a kitchen sink approach including every and all functionality.  This implementation will default to the most simplified form of usage both from UI and feature set.  It will be designed and implemented in such a way that it should be very to relatively straight forward for community and 3rd party developers to add/customize functionality for their specific needs.  Its assumed for now that features/add-ons would be included at build/package time from a lib/dependency perspective, and how that manifests to allowing for runtime style config at the UI/UX level for features and add-ons is tbd but definitely a simple approach will be taken in order to not make the design and implementation too complicated.


## Initial High Level Features

Outlining here non-exhaustive basic list of base features to target across the initial release of the implementation.  The APIs will be having minimal to no backwards breaking changes over the next copule releases for most of these features, some features will be coming in subsequent releases and added as available, most notable is the introduction of new transaction fee handling and introduction of the new metadata concept on accounts and assets.

* Send/Receive Transactions
  * QR Code Support
* Account Mgmt
  * Creation/Export
  * Transaction History
  * Address Book
  * Metadata mgmt
* Asset Mgmt (mosaics)
  * Create/Read/Update/Search
  * Metadata Mgmt
* Namespace Mgmt



## Reference Links

### Design/General Ref

* [NEM Uri Schema Proposal](https://github.com/nemtech/NIP/issues/6) (draft)
* [NEM QR Schema Proposal](https://github.com/nemtech/NIP/issues/3) (draft) 
* [Trezor Connect API](https://wiki.trezor.io/Trezor_Connect_API)


### UI/UX

* [https://medium.muz.li/best-wallet-design-inspiration-ever-522158572c16](https://medium.muz.li/best-wallet-design-inspiration-ever-522158572c16)
* [https://medium.muz.li/designing-a-crypto-wallet-app-concept-72478d216ec6](https://medium.muz.li/designing-a-crypto-wallet-app-concept-72478d216ec6)
* [https://medium.com/coinmonks/accessible-ux-design-in-crypto-products-review-of-brd-wallet-3e81da021193](https://medium.com/coinmonks/accessible-ux-design-in-crypto-products-review-of-brd-wallet-3e81da021193)

### Wallet References

TODO: add here

### Existing v1 NEM Wallets

* NEM Wallet [App Store](https://itunes.apple.com/de/app/nem-wallet/id1227112677), [source-iOS](https://github.com/NemProject/NEMiOSApp); [Play Store](https://play.google.com/store/apps/details?id=org.nem.nac.mainnet), [source-Android](https://github.com/NemProject/NEMAndroidApp)
* Racoon Wallet: need link
* Meteor Wallet: [website](https://www.meteorwallet.io/), [source-iOS](https://github.com/blockstart/nem-meteor-wallet-ios)
* NEMPay Wallet: [source](https://github.com/dgarcia360/NEMPay)

### Current v2 Community Efforts

* [Dev/Testing Wallet](http://wallet.48gh23s.xyz/)
