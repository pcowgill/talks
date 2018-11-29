### Who am I?

[@paulcowgill](https://twitter.com/paulcowgill)
[GitHub](https://github.com/pcowgill/)
[Medium](https://medium.com/@paulcowgill)
[Website](https://cowgill.io/)

This info is available at https://github.com/pcowgill/talks

This is a workshop. Let's get acquainted with the different components of the crypto / web3 stack and the current state of blockchain technology by using some tools from the Ethereum ecosystem.

### What if I have questions?

Feel free to interrupt me at any time. I prefer freeform / real-time questions.

Or if you're feeling shy, we can crowdsource questions online. Go to [sli.do](https://www.sli.do/) and enter the event code `#northwestern-crypto`. I'll check for the most upvoted questions every 10 min or so.

### What to expect

1. [Set up a wallet](#set-up-a-wallet)
1. [Get test ether](#get-test-ether)
1. [Explore the blockchain](#explore-the-blockchain)
1. [Gas](#gas)
1. [Collectibles](#collectibles)
1. [Other dapps](#other-dapps)
   a. [DAOs](#daos)
   b. [Burner wallets](#burner-wallets)
1. [Stablecoins](#stablecoins)

`// TODO: Add the links to the rest of the sections`

`{ Stop and prompt people to vote }`

### Set up a wallet

You should all use [MetaMask](https://metamask.io/) for today.

I'll be sending you testnet ETH using the [Gnosis Safe](https://safe.gnosis.io/).

There are lots of other great alternatives that we won't have time for today: [Argent](https://www.argent.xyz), [BRD](https://brd.com/), [Coinbase Wallet](https://wallet.coinbase.com/), [Status](https://status.im/), [Trust](https://trustwallet.com/), [Balance](https://balance.io/)

### Get test Ether

`{ Walk around the room scanning QR codes to send ETH on the Rinkeby testnet }`

- Viewing the transactions in [Etherscan](https://rinkeby.etherscan.io/address/0x22a2820597492f12ee9eb294fc3e1b4b4a2b379c)

  - Subscribe for notifications of transactions involving a certain address.

- Sending Ether between each other

  - Let's all send some to one person

### Explore the blockchain

Here are some alternatives to Etherscan.

##### Via a UI

- [Etherscan](https://etherscan.io)

- [Blockscout](https://blockscout.com)

- [Alethio](https://aleth.io/)

- [Ganache](https://truffleframework.com/ganache)

Others include [Google](https://cloud.google.com/blog/products/data-analytics/ethereum-bigquery-public-dataset-smart-contract-analytics), [ethplorer](https://ethplorer.io/), [scout.cool](https://www.scout.cool/), [dappboard](http://dappboard.com/), [trivial](https://trivial.co/), [Elementus](https://elementus.io/), [Dappradar](https://dappradar.com)

##### Programmatically

- [eth.events](https://eth.events/)

- [Graph protocol](https://thegraph.com)

### Gas

`{ Talk about gas a bit }`

- [ETH gas station](https://ethgasstation.info/)
- [gastoken](https://gastoken.io/)

_But it's not just about money..._

### Collectibles

Purchasing a digital collectible and exchanging it with other classmates

- [CryptoKitties](https://www.cryptokitties.co/)
- [Decentraland](https://decentraland.org/)
- [CryptoZombies](https://cryptozombies.io/) by [Loom Network](https://loomx.io/)
- [Vault](https://vault.io/)

### Other dapps

##### DAOs

Setting up an Aragon DAO

- [Aragon](https://rinkeby.aragon.org/#/)

##### Burner wallets

- Play with [xdai.io](https://xdai.io/) to show how burner wallets and meta-transactions can be used to onboard new users into the ecosystem without gas.
  - Wait, but what is DAI? [See below](#stablecoins)
  - [xDai explanation](https://medium.com/poa-network/poa-network-partners-with-makerdao-on-xdai-chain-the-first-ever-usd-stable-blockchain-65a078c41e6a)
  - [Blockscout for xDai](https://blockscout.com/poa/dai)
  - [Dai Bridge](https://dai-bridge.poa.network/)

##### TCRs

##### DeFi

[Loans](https://dharma.io/), [Bloom](https://bloom.co/)

##### Marketplaces

- OpenSea
- Decentraland Marketplace
- [Gitcoin](https://gitcoin.co/)
-
- [0x](https://www.0xproject.com/)

##### Prediction markets

https://olympia.gnosis.pm/
Augur

### Stablecoins

Obtaining a stablecoin such as DAI through the MKR contract, transacting it between each other

- [DAI explainer video](https://vimeo.com/247715549)
- [Buy DAI](https://oasis.direct/)

### Room for improvement

`{ Discuss which tools so far have room for improvement }`

We’ll have an open discussion of observations about the state of the tooling the students used, what was missing, what could be done better, etc. This will give students an understanding of how young this ecosystem is and what they could do to push it forward.

- [UX challenges](https://medium.com/ecf-review/challenge-of-ux-in-ethereum-122e1a33688d)

### Nodes / clients

We will then show the students a [geth](https://github.com/ethereum/go-ethereum) node: a client that helps to run the Ethereum blockchain, and how it is able to accept transactions and advance the state of the chain.

`{ Perhaps also discuss Parity, [Mustekala](https://www.musteka.la/), [Nimbus](https://nimbus.status.im/), etc. }`

### Developing smart contracts

We’ll introduce the students to the [Truffle](https://truffleframework.com/) framework for developing smart contracts.

##### ERC standards

[ERC standards](https://eips.ethereum.org/erc) like ERC20 for tokens (like DAI, the Aragon token, etc.) and ERC721 (like Cryptokitties, Decentraland, etc.) for collectibles (things we covered above).

"Application-level standards and conventions, including contract standards such as token standards (ERC20), name registries (ERC137), URI schemes (ERC681), library/package formats (EIP190), and wallet formats (EIP85)."

Source: https://eips.ethereum.org/

##### OpenZeppelin

[OpenZeppelin](https://openzeppelin.org/) is a library for inheriting from and extending existing smart contract logic.

### Why is this important

`// TODO: Add a link or two`

1. [Naval's thread about governance systems historically](https://twitter.com/naval/status/877467629308395521)
1. [AI -> tyranny, blockchain -> democracy](https://www.theatlantic.com/magazine/archive/2018/10/yuval-noah-harari-technology-tyranny/568330/)
1. [The Truth Machine](https://smile.amazon.com/Truth-Machine-Blockchain-Future-Everything/dp/1250114578/)
1. [Social justice](https://www.meetup.com/Blockchain-for-Social-Good-Chicago/)
1. [Podcast episode about why decentralization matters](https://www.breaker.audio/a16z/e/35542740)
1. [Toy markets](https://blog.ycombinator.com/toy-markets/)
1. Zero platform risk -> the great unbundling of front end and back end (and of individual front end features). Users get "right to exit" meaning that they can elect to use alternative clients without losing all of their data and the network effect of the platform, and the tech tycoons of the future can't prevent them from doing so.

### Privacy

If time allows, we will discuss privacy and how other blockchains incorporate it as a first-tier feature. We'll also discuss how private technologies like zero-knowledge proofs could be introduced to the Ethereum blockchain in the future.
