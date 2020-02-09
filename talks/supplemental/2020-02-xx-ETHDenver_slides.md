Theme: notes
Palet: Red
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

Native mobile apps clearly are the current winner in web 2.

<br />

A slightly larger swath of **disengaged** users might try a mobile web app first, but the “sticky”, **power users** prefer native mobile apps.


---

# when is mobile the right fit?
<br />

* high frequency
* real time
* biometric auth
* convenient, local data persistence required

---
Layout: SectionTitle

# what about censorship?


---
# censorship
<br />

The main concern when talking about building native mobile web 3 apps is censorship, but using contract-based accounts (or WalletConnect) means that there’s no loss of funds or ability to use the contracts with the same “account” even in the case of censorship.


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

> ## Policies change along with the zeitgeist

---
Layout: SectionTitle

# how


---
# building native mobile dapps
<br />

Let's talk best practices for building a native mobile Ethereum dapp with a simple UX without any decentralization tradeoff.

---
Layout: HeaderAndColumns

# what is needed to do this well?
<br />

+++
<br />

* in-dapp fiat onramps
* The Graph
* in-dapp ephemeral accounts
* in-dapp contract-based accounts
* ENS
+++
<br />

* meta-transactions
* deep linking
* biometric auth
* push notifications
* L2

---
Background: /Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/TasitLogoSvg3072.png


---
# boiling the ocean?
<br />
<br />
<br />

![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/Cooking-Man-Emoji.png) 
![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/Water-Wave-Emoji.png)
![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/Fire-Emoji.png)

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
const a = 10;
a = a + 5;
console.log(a);
```



---
# why now?
<br />
<br />
<br />
<br />

### In-dapp fiat onramps recently have made this a viable option.


---
# is it worth making a new account?
<br />

For new users, they don't have another account anyway, and this could evolve into their main account.
<br />
<br />

A new account is better for OPSEC and accounting reasons anyway.

---
# (ephemeral and/or contract-based)

---
Layout: SectionTitle

# ongoing UX

---

# the graph
---

# ENS
---

# meta-transactions
---

# 3Box
---
Layout: SectionTitle

# mobile-specific features

---

# deep linking
---

# biometric auth
---

# push notifications
---
Layout: SectionTitle

# scaling and privacy
---
# L2, Eth2, etc.
---
Layout: SectionTitle

# wrapping up
---

# dapps are useful
<br />

Dapps already deliver significant value and “a-ha” moments to crypto-native “innovators” in ways that will eventually be useful for mainstream people too.


---
# UX is the problem
<br />

So the only reason (setting the scaling discussion aside for the moment) that there aren’t lots of users flooding the network yet is that there aren’t sufficiently simple tools for great web 2 product teams to build native mobile apps for Ethereum dapps.
---
# user interviews
<br />

We're actively doing user interviews to shape which features are prioritized.
<br />

Please reach out on Twitter to **[@paulcowgill](https://twitter.com/paulcowgill)**

---
# thanks
<br />

Work on Tasit is supported in part by:
<br />
<br />

* Ethereum Foundation
* Gnosis GECO
* Gitcoin Grants



---
<br />
<br />
<br />
<br />

> ### Don't use too many browser APIs in your js SDK.


