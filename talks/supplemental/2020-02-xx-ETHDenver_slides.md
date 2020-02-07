Theme: notes
Palet: Green
Size: Wide


---
Layout: Title

# Native mobile Ethereum dapps
## Paul Cowgill, Tasit Labs


---
Layout: Default

# Outline
___
### **why**
___

### **how**
___
### **what about censorship?**


---
Layout: Default

# Who am I?

#### [@paulcowgill](https://twitter.com/paulcowgill)

![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/PaulStylized.png) 

---
Layout: SectionTitle

# Why

---
Layout: Split

## Phones
___
### Young people worldwide do most things on the internet from their phones.
___
{{iphone}}
___


+++
## Laptops
___
### And yet we're building web-based dapps optimized for use on laptops.
___
{{browser}}
___




---

# Native vs. web
___
Native mobile apps clearly are the current winner in web 2.
___
A slightly larger swath of disengaged users might try a mobile web app first, but the “sticky”, power users prefer native mobile apps.


{{Line-Chart}}
- time:1,3,10,30,100,300


---
Layout: SectionTitle

# What about censorship?


---
# Contract-based accounts
___
The main concern when talking about building native mobile web 3 apps is censorship, but using **contract-based accounts** means that there’s no loss of funds or ability to use the contracts with the same “account” even in the case of an Apple or Google takedown.


---
Layout: SectionTitle

# How


---
# Building native mobile dapps
___
Let's talk best practices for building a native mobile Ethereum dapp with a simple UX without any decentralization tradeoff.

---
Layout: HeaderAndColumns

# Tasit SDK
#### We're building an SDK to make this simpler

+++
___
* in-dapp fiat onramps
* The Graph
* in-dapp ephemeral accounts
* in-dapp contract-based accounts
* ENS
+++
___
* meta-transactions
* deep linking
* biometric auth
* push notifications
* L2


---
Layout: Split

![](/Users/paulcowgill/Code/general/paul-work-related/talks/talks/supplemental/images/sea-ocean-wave-vehicle-lava-screenshot-80695-pxhere.com.jpg) 
+++
# Boiling the ocean?
___
We're not trying to boil the ocean here - our SDK makes use of other great SDKs internally!




---
Layout: SectionTitle

# In-dapp wallets
## (ephemeral and contract-based)

---
___
___
___
___
___
> ### To attract the next wave of Ethereum users, we should assume that users don’t have a wallet yet.

---
# A single, fluid UX
___
Let’s set them up with their first "wallet” in the app they want to use instead of kicking them elsewhere to a separate app to set one up before they can get started.

```js
const a = 10;
a = a + 5;
console.log(a);
```



---
# Why now?
___
___
___
___
### In-dapp fiat onramps recently have made this a viable option.


---
# Is it worth making a new account?
___
For new users, they don't have another account anyway, and this could evolve into their main account.
___
A new account is better for OPSEC and accounting reasons anyway.

---
Layout: SectionTitle

# in-dapp fiat onramps

---
Layout: SectionTitle

# The Graph
---
Layout: SectionTitle

# ENS
---
Layout: SectionTitle

# meta-transactions
---
Layout: SectionTitle

# Mobile-specific features
## (deep linking, biometric auth, push notifications)
---
Layout: SectionTitle

# L2
---
Layout: SectionTitle

# In-dapp wallets

---
# Dapps let you do things you couldn't do with a capp
___
Dapps already deliver significant value and “a-ha” moments to crypto-native “innovators” in ways that will eventually be useful for mainstream people too.


---
# UX is the problem
___
So the only reason (setting the scaling discussion aside for the moment) that there aren’t lots of users flooding the network yet is that there aren’t sufficiently simple tools for great web 2 product teams to build native mobile apps for Ethereum dapps.
---
# User interviews
___
We're actively doing user interviews to shape which features are prioritized.
___
Please reach out on Twitter to **[@paulcowgill](https://twitter.com/paulcowgill)**

---
# Thanks
___
Work on Tasit is supported in part by:
___

* Ethereum Foundation
* Gnosis GECO
* Gitcoin Grants




