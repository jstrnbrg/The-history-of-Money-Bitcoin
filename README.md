# The history of Money & Bitcoin


## Table of Contents
1. [Project description](#project-description)
2. [Contributor workflow (please read)](#contributor-workflow)
3. [Epoches and chapters](#preliminary-draft-of-epoches-and-chapters)
4. [Sources](#possible-sources)
5. [Help needed](#help-needed)

## Project description
The basic idea is to create an app that explains the origins of money, what money even is, why bitcoin is important and why it could (will) be the next step in monetary evolution and at the end give some tips on how to get started, i.e where to buy, where to store etc.  
This app seems great as a base and can be adapt it to our content/needs as necessary.  
HistoryOfEverything: https://github.com/2d-inc/HistoryOfEverything  
The app is open-source under a MIT License.

Similarly to that app, I would structure everything into a few different mega-chapters/epoches and then have 5-10 shorter chapter in these epoches, each with a reading time of up to 5 minutes.  
For a preliminary draft of the epoches and chapters please see below at.  
Each chapter should have a few "deep dive" resource links at the bottom.

_______________________________________________

## Contributor workflow

The content is maintained using a "contributor workflow" where everyone contributes patch proposals using "pull requests".
This facilitates social contribution, easy testing and peer review.

To contribute a patch, the workflow is as follows:


  1. Create topic branch
  2. Commit changes
  4. Push changes to your branch
  5. Create pull request to the master branch

In general [commits should be regard one chapter/topic](https://en.wikipedia.org/wiki/Atomic_commit#Atomic_commit_convention) and diffs should be easy to read.

Commit messages should be verbose by default consisting of a short subject line (50 chars max), a blank line and detailed explanatory text as separate
paragraph(s), unless the title alone is self-explanatory (like "Corrected typo in Makefile") in which case a single title line is sufficient.

Further explanation [here](http://chris.beams.io/posts/git-commit/).

If a particular commit references another issue, please add the reference. For example: `refs #1234` or `fixes #4321`.

Please refer to the [Git manual](https://git-scm.com/doc) for more information about Git.

If a pull request is not to be considered for merging (yet), please prefix the title with [WIP] or use [Tasks Lists](https://help.github.com/articles/basic-writing-and-formatting-syntax/#task-lists) in the body of the pull request to indicate tasks are pending.


At this stage one should expect comments and review from other contributors.
You can add more commits to your pull request by committing them locally and pushing to your fork until you have satisfied all feedback.

_______________________________________________

## Preliminary draft of epoches and chapters

### 1. What is money?
#### A shared myth:
- Money has value because we believe it has value and because everyone does, it has.
#### Functions of money:
- MoE
- SoV
- UoA
#### How does money naturally emerge?
- Sale-ability
_______________________________________________

### 2. Early forms of money
#### Proto money
#### Shells
#### Stones, beads etc
_______________________________________________

### 3. Commodity money
#### Gold
#### Silver etc
_______________________________________________

### 4. Commodity backed money
#### Gold standard
#### Silver standard
_______________________________________________

### 5. Fiat Money
#### Keynsian & Moneterian
- What is their main claim?
#### Austrian
- What is their main claim?
#### Sound vs Unsound money
_______________________________________________

### 6. History of Bitcoin
#### Failed early efforts:
- DigiCash, e-gold
- Why did they fail? Centralisation
- Hal finney, Nic szabo, adam back, w. dai etc.
#### Cypherpunks
- (https://www.coindesk.com/the-rise-of-the-cypherpunks)
- Who were they? What do they stand for?
- Manifesto: https://github.com/NakamotoInstitute/nakamotoinstitute.org/blob/master/sni/static/docs/cypherpunk-manifesto.txt
#### Birth of bitcoin and bitcoin white paper
- Who was Nakamoto?
- What happened to his coins?
- What happened to him?
- How did he release his invention?
- Did he premine?
#### Early usage of bitcoin
- Is it only used for illegal things?
- Do only crooks use bitcoin?
- Is Bitcoin anonymous?
#### famous exchange hacks
- Third parties are a secuity hole.
- How does bitcoin enable you to not trust any third party?
#### Waves of adoption and price bubbles
#### Scaling bitcoin debate, UASF
- Vertical scaling (bigger blocks) vs layered scaling
- UASF: which proves that miners have not much to say in Bitcoin --> might be a bit too deep for this audience??
_______________________________________________

### 7. Why bitcoin
#### Forks & Altcoins
- (if not shitcoins ;-), illusion of next bitcoin and why they are doomed to near zero monetary value compared to Bitcoin
#### Game theory , Schelling point, Lindy effect, network effect etc...
_______________________________________________


### 8. How Bitcoin works
#### Keys & Addresses
- What is a private key? A long random number
- What is a public key?
> Bitcoin makes use of cryptography to create a key pair that controls access to your bitcoin. The key pair consists of a private key, which a long random number, and mathematically derived from it a public key. The public key is used to receive coins, and the private key is used to sign transactions to spend the coins.
- Why is from private to public easy, but vice versa hard?
> The mathematical relationship between the public and the private key has the following properties: A) It is infeasible to calculate the private key from the public key,  B)  The private key can be used to generate digital signatures on messages. These signature can then be validated with the help of the public key without revealing the private key.
- What is an address?
> When sending Bitcoin the recipient is (in most cases) a Bitcoin address. A Bitcoin address is derived from a public key and allows. Using an address as the recipient compared to sending directly to a public key (which isn't possible in Bitcoin) has certain security and privacy advantages.
- Why do we need addresses? Other cryptos don't have them.
> This could be too deep. "Addresses provide greater security because even if the ECDSA breaks the double hash will still protect your money."
- How many private keys are there? Isn't it likely that someone else will generate the same private key?
> A private key is 64-characters long, each of which can be one of 16 characters, called hexadecimal (0-9 + A-G). That means there are 16^64 or 2^256 possible private keys. That is 115,79 quattuorvigintillion or 115792089237316195423570985008687907853269984665640564039457584007913129639936.
As a reference there are about 2^229 atoms in the milky way. How likely is it that you can tell me which of these atoms I'm currently thinking about?
https://www.youtube.com/watch?v=S9JGmA5_unY
- What does it mean to own bitcoin?
> Owing bitcoin means nothing more and nothing less than being in possession of the private key(s) that allow you to unlock/transfer these bitcoins. Just a random number, but undoubtedly a very important one.

#### Wallets
- What is a wallet? Why is "wallet" a mis-namer? What does a wallet do?
> A common misconception about bitcoin is that bitcoin wallets "contain" bitcoin. In fact, a wallet only contains digital keys (private keys). The “coins” are recorded in the blockchain. Users control the coins by signing transactions with the private keys in their wallets. In that sense, a bitcoin wallet actually is a keychain.
- How did wallets evolve?
> At first a bitcoin wallet would create a set of key-pairs which were unrelated to each other which means each of these keys had to be backed up individually, later with Bitcoin-Improvement-Proposal-32, short BIP-32, hierarchical deterministic wallets were introduced. This type of wallet stores one master private key from which all child keys are mathematically derived. This greatly reduced the complexity as it allowed users to only back up one private key. Another great improvement was the introduction of BIP-39 which allows us to represent the master private key as a mnemonic sentence, consisting of 12 to 24 words. From then on you did not have to back up a 64 character private-key for which one single wrong character means loss of coins but instead a sentence of easily recognisable words.
- What types of wallets are there?
> There are a few different kinds of wallets, depending on different use cases. Generally there is a spectrum from hot to cold wallets and a classification between custodial and non-custodial wallets.  
A *custodial* wallet is a wallet where you do not hold the master private key (seed) yourself, but a third party. Examples of that is leaving your bitcoin on an exchange. If the exchange gets hacked, your coins are likely lost. In the true bitcoin-spirit we would advise against using such a wallet as it comes with tremendous risks, which are not worth the convenience.
A *non-custodial* wallet is a wallet that contains the master private key (seed), thereby having full and sole control over the coins. Examples of such wallets are the following:  
*Paper wallets:* a paper wallet is a piece of paper with a privat key and an address printed on it. Paper wallets are generally not recommended anymore as it is easy to get it wrong and loose your coins.
*Software wallets:* An application that contains your master private key and let's you send and receive coins easily. A software wallet is recommended for low amounts, due to the insecure nature of a smartphone.  Similarly you would not put all your fiat money in to your purse/wallet that you carry around day in day out.
*Hardware wallets:* A dedicated device with the sole purpose of keeping your seed secure while still allowing you to interact with your coins with ease. This type of wallet is generally recommended to safekeep larger amounts of coins.
#### Transactions
- How is a tx constructed?
- What are inputs and outputs?
- What are fees? Can I pay no fee?
#### Bitcoin Network
- What is a node?
- What types of nodes are there?
- What are nodes doing?
- What if nodes run different, incompatible software?
- Difference between hard- and softfork?
> Softfork reduces the set of valid operations (e.g. 0.5 MB blocks would still be valid to nodes that did not follow the soft fork)  whereas hardforks introduce rules that would have been invalid before (e.g. 2 MB blocks are invalid right now so only nodes that update will see them as valid)
#### Blockchain
- Why do I need to know the complete blockchain?
- Isn't a blockchain slow and inefficient database?
- What makes the bitcoin blockchain so special?
#### Mining & Consensus
- How are miners getting paid? and why?
- What are miners doing?
- What are coinbase transactions?
- Which functions does mining fullfill?
- How many Bitcoins are there and how many will there be?
- How are nodes agreeing on which chain(tip) is the right one?
#### Why Bitcoin is immutable
-
#### How to kill bitcoin
- What are possible threats for bitcoin?
- ( We can omit this section. saifedean has some material here )
_______________________________________________


### 9. Lightning
- Lightning channel and Lightning network in simple words without going into technical ( comparing lighting channel to some real life analogy. One way to explain is like two people puts some money on a table and can exchange as many time as they want without declaring to whole world. And extend it to more than two people participating in exchange )
#### Multisig
#### Timelocks
#### Payment Channels
#### HTLC
#### Lightning Network

_______________________________________________

## Possible Sources

#### History of Money
https://medium.com/coinbundle/long-read-history-of-money-d75ed25d85c4
very high level, might be helpful to structure chapters

#### The history of money / the future of bitcoin and cryptocurrencies:
https://hackernoon.com/the-history-of-money-the-future-of-bitcoin-and-the-cryptocurrency-economy-5cc25e808275
high level summary

#### Shelling Out: The Origins of Money
https://nakamotoinstitute.org/shelling-out/
good for specific examples

#### Money by Yuval Noah Harari:
https://www.amazon.co.uk/Money-Vintage-Yuval-Noah-Harari-ebook/dp/B0759WV5ZG
very approachable, why do we have money etc.

#### History of bitcoin - Wikipedia
https://en.wikipedia.org/wiki/History_of_bitcoin

#### Theory of money and credit
https://mises.org/library/theory-money-and-credit/html

#### Denationalisation of money
https://mises-media.s3.amazonaws.com/Denationalisation%20of%20Money%20The%20Argument%20Refined_5.pdf
not read yet, why should the currency not be under government control?

#### The origins of money by Carl Menger
https://mises-media.s3.amazonaws.com/On%20the%20Origins%20of%20Money_5.pdf

#### The Bitcoin Standard

#### The ethics of money and bitcoin
https://medium.com/@nicolasdorier/the-ethics-of-money-and-bitcoin-f6c4f568d9f9

#### Bitcoin money book
https://thebitcoinrabbi.com/bitcoin-money-book/

#### Purely digital currencies before bitcoin
https://hackernoon.com/the-amazing-story-of-cryptocurrencies-before-bitcoin-fe1b0e55155b


#### http://unenumerated.blogspot.com/

_______________________________________________

## Infographics:
- Bitcoin History: The Complete History of Bitcoin Timeline: http://historyofbitcoin.org/
- A History of Bitcoin and Cryptocurrency’s Greatest Moments Infographic: https://coincentral.com/bitcoin-history/

_______________________________________________

## Help needed
If you or someone you know would like to help, please do so! The following is greatly appreciated:
- Content creation: You can easily answer some of the questions above? Then please do so and write a few paragraphs.
- Graphic creation: You are a great designer? We will need a few nice graphics to make the app aesthetically pleasing. Please contact us!
- App adaptation: We will need to customise the base app (see project description) to our needs and already have a lot of cool ideas to make the learning experience even more interesting which will need custom development. If you like the project, have coding skills and are interested to help, please have a look at the open issues and/or contact us.

If you have any other ideas, please also let us know.
