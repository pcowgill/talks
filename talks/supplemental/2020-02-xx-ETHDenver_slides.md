Theme: notes
Palet: Green
Size: Wide

---

Layout: Title

# Native mobile Ethereum dapps

## Paul Cowgill 📱 Tasit Labs

---

Layout: Default

# Outline

<br />

### **why**

<br />

### **what about censorship?**

<br />

### **how**

---

Layout: Default

# who am I?

<br />

### [@paulcowgill](https://twitter.com/paulcowgill)

<br />

![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/PaulStylized.png)

---

Layout: SectionTitle

# why

---

Layout: Split

## phones

<br />

### Young people worldwide do most things on the internet from their phones.

<br />

{{iphone}}
<br />

+++

## laptops

<br />

### And yet we're building web-based dapps optimized for use on laptops.

<br />

{{browser}}
<br />

---

# native vs. web

<br />
<br />
<br />

Native mobile apps clearly are the current winner in web 2.

<br />

A slightly larger swath of **disengaged users** might try a mobile web app first, but the “sticky”, **power users** prefer native mobile apps.

---

# when to use native mobile?

<br />

- high frequency
- real time
- low(ish) stakes—although this is changing
- biometric auth
- convenient, reliable, local data persistence required
- uses camera or GPS

---

Layout: SectionTitle

# what about censorship?

---

# censorship

<br />
<br />
<br />
<br />

Using **contract-based accounts** (or **WalletConnect**) means that there’s no loss of funds or ability to use the contracts with the same “account” even in the case of censorship.

---

# scenarios with React Native

<br />

### Apple takedown?

Works on Android
<br />
<br />

### Google takedown?

Works on iOS
<br />
<br />

### Both platforms censored?

**react-native-web** and/or sharing code with a React codebase
<br />

---

<br />
<br />
<br />
<br />

> ## Policies change along with the zeitgeist.

---

Layout: SectionTitle

# how

---

# building native mobile dapps

<br />
<br />
<br />

Let's talk best practices for building a native mobile Ethereum dapp with a simple UX without any decentralization tradeoff.

---

Layout: HeaderAndColumns

# what is needed to do this well?

<br />

+++

### onboarding

<br />

- in-dapp fiat onramps
- in-dapp wallets
  _ burner accounts
  _ contract-based accounts
  +++

### ongoing UX

<br />

- ENS
- The Graph
- optimistic UI
- meta-transactions

+++

### mobile stuff

<br />

- deep linking
- biometric auth
- push notifications
- L2

---

Background: /Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/TasitLogoSvgAlt3072.png

---

Layout: SectionTitle

# onboarding

---

# in-dapp fiat onramps

---

# in-dapp wallets

<br />
<br />

> ### To attract the next wave of Ethereum users, we should assume that users don’t have a wallet yet.

---

# a single, fluid UX

<br />

Let’s set them up with their first "wallet” in the app they want to use instead of kicking them elsewhere to a separate app to set one up before they can get started.
<br />

```js
import { Account } from "tasit-sdk";
const burnerWallet = Account.create();
const { address } = burnerWallet;
console.log(address); // '0x...'
// ...
```

---

# why now?

<br />
<br />
<br />
<br />

### In-dapp fiat onramps recently have made this a viable option.

---

# another new account?

<br />

For new users, they don't have another account anyway, and this could evolve into their main account.
<br />
<br />

A new account is better for OPSEC and accounting reasons anyway.

---

# (burner and contract-based)

<br />
<br />
<br />

```js
Account.upgrade(burnerWallet);
```

---

Layout: SectionTitle

# ongoing UX

---

# optimistic API

<br />

```js
import { Contract } from "tasit-sdk";

const { NFT } = Contract;

const contractAddress = "0x0E86...333";

const contract = new NFT(contractAddress);

const action = contract.safeTransferfrom(/*...*/);
action.on("error", errorListener);
action.on("enoughConfirmations", successListener);
action.send(); // broadcast

// Do optimistic UI updates immediately, while making sure
// to update the UI again when there are enough
// confirmations for your use case
// ...
```

---

# the graph

<br />
<br />

```js
const action = contract.safeTransferfrom(/*...*/);
action.on("error", errorListener);
action.on("presentInTheGraph", successListener);
action.send(); // broadcast
// ...
```

---

# ENS

---

# meta-transactions

<br />
<br />
<br />

```js
const action = contract.myFavoriteMethod(/*...*/);
action.on("error", errorListener);
action.on("enoughConfirmations", successListener);
action.sendForFree(); // meta-tx broadcast

// ...
```

---

# 3Box

---

Layout: SectionTitle

# mobile-specific features

---

Layout: HeaderAndColumns

# deep linking

+++

{{iphone}}
<br />

+++

{{iphone}}
<br />

---

# biometric auth

---

# push notifications

---

Layout: SectionTitle

# boiling the ocean?

<br />
<br />

![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/Cooking-Man-Emoji.png)
![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/Water-Wave-Emoji.png)
![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/Fire-Emoji.png)

---

Layout: SectionTitle

# scaling and privacy

---

# scaling and privacy

<br />

### L2

state channels, (optimistic|zk) rollup
<br />
<br />

### Eth2

<br />

### Privacy

---

Layout: SectionTitle

# wrapping up

---

# dapps are useful

<br />
<br />
<br />

Dapps **already** deliver significant value and “a-ha” moments to **crypto-native** “innovators” in ways that could be useful for mainstream people too if packaged correctly.

---

# UX is the problem

<br />
<br />

## So the only reason (setting the scaling discussion aside for the moment) that there aren’t lots of users flooding the network yet is that there aren’t sufficiently simple tools for **great web 2 product teams** to build native mobile apps for Ethereum dapps.

# where to go from here

<br />
<br />

We're actively doing **user interviews** and **developer interviews** to shape which features are prioritized.
<br />
<br />

Please reach out on Twitter to **[@paulcowgill](https://twitter.com/paulcowgill)**

---

Layout: SectionTitle

# thanks

<br />

## Work on Tasit is supported in part by:

<br />
<br />
<br />

![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/geco_rgb_sponsor_white.png)
![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/ecosystem-support.svg)
![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/gitcoin_logo_white.png)

---

Layout: HeaderAndColumns
+++

### 🤐

### **Website**

### [tasit.io](https://tasit.io)

<br />
<br />

### 🐦

### **Twitter**

### [@TasitProject](https://twitter.com/TasitProject)

<br />
<br />

### 💬

### **Discord**

### [bit.ly/tasit-discord](https://bit.ly/tasit-discord)

<br />
<br />

### 💬

### **Telegram**

### [t.me/tasitproject](t.me/tasitproject)

+++

### 💻

### **GitHub**

### [github.com/tasitlabs](https://github.com/tasitlabs)

<br />
<br />

### 📄

### **Docs**

### [docs.tasit.io](https://docs.tasit.io)

<br />
<br />

### 📝

### **Medium**

### [medium.com/tasit](https://medium.com/tasit)

<br />
<br />

### 💡

### **Feature requests**

### [feedback.tasit.io](https://feedback.tasit.io/feature-requests)

---

<br />
<br />
<br />
<br />

> ### Don't use too many browser APIs in your js SDK.
