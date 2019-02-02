## Windy City DevFest

Fri, February 1, 2019

### Using Ethereum, React Native, and the Tasit SDK to build 3rd-party mobile clients for dapps (decentralized apps)

[Google Slides for this presentation](http://bit.ly/2019-02-01-windy-city-devfest-ethereum-tasit)

[Event link](https://windycity.devfest.io/)

##### Talk Description

In this talk, I'll provide an introduction to developing with Ethereum, and I'll show how to use React Native to create a 3rd-party mobile app for an Ethereum dapp (decentralized app), using the Tasit SDK under the hood.

Having built React Native apps with "traditional" back ends before, I can see that the tooling isn't quite there yet for Ethereum dapps such that a newer dev can ship a React Native MVP with new business logic or a sleeker design quickly without (A) worrying about Ethereum-related back-end details or (B) reinventing the wheel with some foundational onboarding features on the client-side. The Tasit SDK aims to solve those problems.

The Tasit SDK supports ephemeral Ethereum accounts, simple onboarding, an API that abstracts away low-level Ethereum details, and first-class support for popular ERC standards.

It's easy to mock today's Ethereum dapps for not having many users yet - the reason for the low user growth is that the UX of dapps is pretty terrible right now. Most dapps don't have standalone native mobile apps, and the onboarding is too confusing for regular people. Given that everything in Ethereum is permissionless and interoperable, if you nail the UX in your own 3rd-party mobile app for a dapp, it's easy to eclipse the number of users of the "real" dapp and become the de facto front end for the dapp.

Having multiple front ends for a dapp is important for "right to exit" - that is, being able to use an alternative client implementation with a different feature set, different governance, and/or different pricing, without needing to export and import your data to do so. What's unique about the Ethereum ecosystem is that making a 3rd-party client is fully permissionless, which means there's no risk that the developers of a smart contract can suddenly "throttle" users of their "API" in the way that would have been possible in web 2.0.Using Ethereum, React Native, and the Tasit SDK to build 3rd-party mobile clients for dapps (decentralized apps)
