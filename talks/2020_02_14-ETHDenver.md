## ETHDenver 2020

Fri, Feb 14, 2020

### Native mobile Ethereum dapps: Why, how, and what to do about censorship

[Slides for this presentation](./supplemental/2020_02_14-ETHDenver/2020_02_14-ETHDenver.pdf)

[Event link](https://www.ethdenver.com/)

##### Description

Young people worldwide do most things on the internet from their phones. And yet we're all building web-based dapps optimized for use on laptops. Native mobile apps clearly are the current winner in web 2. A slightly larger swath of disengaged users might try a mobile web app first, but the “sticky”, power users prefer native mobile apps.

The main concern when talking about building native mobile web 3 apps is censorship, but using contract-based accounts means that there’s no loss of funds or ability to use the contracts with the same “account” even in the case of an Apple or Google takedown.

In this talk I'll cover best practices for building a native mobile Ethereum dapp with a simple UX without any decentralization tradeoff. At Tasit, we're building an SDK to make this simpler. It supports in-dapp fiat onramps, The Graph, in-dapp ephemeral accounts and contract-based accounts, ENS, meta-transactions, deep linking, biometric auth, push notifications, and L2. (We're not boiling the ocean here - our SDK makes use of other great SDKs internally!)

To attract the next wave of Ethereum users, we should assume that users don’t have a wallet yet. Let’s set them up with their first "wallet” in the app they want to use instead of kicking them elsewhere to a separate app to set one up before they can get started. In-dapp fiat onramps recently have made this a viable option.

Dapps already deliver significant value and “a-ha” moments to crypto-native “innovators” in ways that will eventually be useful for mainstream people too, so the only reason (setting the scaling discussion aside for the moment) that there aren’t lots of users flooding the network yet is that there aren’t sufficiently simple tools for great web 2 product teams to build native mobile apps for Ethereum dapps.

Work on Tasit is supported in part by the Ethereum Foundation, the Gnosis GECO program, and Gitcoin Grants. Thanks!
