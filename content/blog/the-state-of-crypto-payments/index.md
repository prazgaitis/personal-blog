---
title: "The state of Crypto Payments in 2022"
date: "2022-03-14 20:30"
description: "When will crypto start taking market share from Visa?" 
hidden: false
---

I'm disappointed. It's 2022 and I can only find two places to (legally) spend my crypto - an NFT or a Tesla belt buckle.

![As much as it pained me to use dogecoin, I bought the belt buckle. For science.](https://i.imgur.com/TyYzsbQ.jpg)

2021 was the year that NFTs took off. [OpenSea did over $15B](https://www.aakashg.com/2022/01/05/opensea/) in transaction volume in 2021, and countless other NFT marketplaces sprung up in the wake of all the new demand.

What about physical goods though? We were promised a techno-future where commerce happens frictionlessly and value is exchanged freely online. So why haven't crypto payments started to eat Visa & Mastercard's lunch?

There are two main reasons we haven't seen crypto starting to replace credit cards: lack of incentives for merchants, and lack of incentives for customers.

## The rough spots

Let's start with the merchant side. Merchants have an incentive to add support for payment methods that people like to use. Crypto isn't _quite_ mainstream yet. The reality is that there just aren't that many people who have crypto wallets yet. PayPal has [upwards of 400m monthly users](https://www.businessofapps.com/data/paypal-statistics/). MetaMask, the most popular Ethereum wallet, claims to have 21 million users. Coinbase has [73m users](https://earthweb.com/coinbase-statistics/), but only 6 million of those transact in any given month. Adding the ability to check out with crypto likely won't move the needle on sales today.

Next up is the uncertainty about accounting and taxes. Do you want to keep Ethereum on the balance sheet? If so, you'll need to account for price volatility. Let's say you make a sale and earn 1 ETH when ETH trades at $3000 USD. If you hold onto that ETH and the price goes up to $4000 USD, you've got $1000 USD of capital gains and Uncle Sam wants his cut.

What about buyers?

First, the obvious points of friction. Shoppers don't want to trade a speculative coin that could go to the moon tomorrow for a depreciating asset. This is a problem with both digital and physical assets.

Let's say you buy an NFT for 1 ETH. If you get lucky and the price goes up to 1.1 ETH, the price of ETH could drop 20%. Even if the value of the NFT stays flat (it probably won't - the vast majority NFTs lose value), how much did that NFT _really_ cost you? 😬

There are more subtle reasons too. Look at this big ole disclaimer on Travala.com, a travel booking site. ![travala refund policy](https://i.imgur.com/v9WxAHa.png)

This adds friction to the booking process. What happens if you cancel your trip? The refund process is not really clear or consistent.

And what about chargebacks? They're a notorious thorn in the side for merchants, but they do give the buyer some protection. Got charged for something that didn't show up in the mail? Call Chase and they'll take it off your statement. If you paid with crypto, you're outta luck.

In the US, using crypto to buy something counts as a taxable event. If you buy a TV with crypto, you technically need to report the capital gains when you settle up with Uncle Sam.

Lastly, it's still too confusing. To buy the Tesla belt buckle, first I have to figure out where to buy dogecoin. I see that there is a dogecoin wallet in the App Store, but it won't let me exchange my dollars for coins. I _also_ have to make sure the wallet allows me to send it somewhere. Coinbase does the trick, but Robinhood does not -- I can buy coins, but I can't send them anywhere.

The same is true when buying NFTs - I need to buy ETH somewhere (and pay a fee), then send it to a compatible wallet (another fee), and then mint the NFT (more fees). Whew.

It's not all bad though - let's look at some of the benefits.

## Why it _might just work_

Some of the downsides with crypto also happen to be benefits.

Merchants love the fact that there are no chargebacks. Sure, the buyer doesn't get any protection, but there are other ways to get around this problem. Higher value transactions can use an escrow service. For lower value transactions buyers might have to take a risk and hope that the merchant values their repuration enough to consistently deliver the product.

Reviews can work in our favor here. The nice part about a blockchain is that it's public and anyone can read it. We can verify that a review is legit because we can see that this person actually bought the thing that they're reviewing.

Has this worked in the past? Reviews worked great for Airbnb, but not as well for Amazon. It's well known that most Amazon reviews [are bullshit](https://www.amzfinder.com/blog/top-100-facebook-groups-list-amazon-reviews/).

Reputation works both ways here. Merchants can easily tell who their best customers are, because the purchase history is all on-chain. You can also do some cool things with digital rewards here too. Maybe you can bought concert tickets and some band merch with Solana. The band can give out backstage passes to fans who have been to more than 10 shows. You can prove that you've been at each show - the receipts are all on-chain.

Let's talk about fees.

It usually costs the merchant about 3% to run a credit card transaction. Most payment processors will slap on another 1% for foreign exchange if you want to charge the buyer in their local currency. There are a lot of players involved in this process, and everyone charges a toll.

Crypto flips this on its head! For crypto purchases, the _buyer_ pays the transaction fee. Sure, we won't use the Ethereum mainnet where transaction fees are about [$46 today](https://coinmarketcap.com/alexandria/article/sick-of-high-ethereum-gas-fees-do-this-instead). Other chains like Solana, Bitcoin Lightning, Avalanche, or Polygon (an Ethereum L2) offer instant transactions for fractions of a penny.

And what about those taxes? Stablecoins could be an answer here. These won't change in value, so there shouldn't be any capital gains to worry about.

## Ok, maybe I'm convinced. How will it play out?

There are a few things that need to happen

First, crypto adoption needs to continue (and it will). There needs to be a critical mass of users with a wallet on their phone or web browser so that merchants can't ignore this new payment method.

Whatever you think about NFTs, they've been fantastic user acquisition channel for crypto in general. This will also continue, despite the mind-boggling prices for pictures of monkeys. Humans are irrational, and gambling is rooted deep in our psyche.

We're seeing new crypto wallets pop up almost daily. The winner will be the one that has multi-chain support. It will need to be a fiat on-ramp as well. As we discussed earlier, there are still too many steps involved in actually _getting_ crypto. Keep an eye on [Phantom.app](https://phantom.app/), the leading Solana Wallet. The team just raised [a big round](https://blockworks.co/crypto-wallet-raises-109-million/), and is looking to add ETH support. [Coinbase Wallet](https://www.coinbase.com/wallet) is the gorilla here. They've got the engineering chops, a lot of users, and very deep pockets.

Next, we need to build better tools for merchants. In the late 90's there was Authorize.net, which now seems antiquated compared to [Stripe](https://stripe.com). If you run a Shopify store today, you would never even consider integrating directly with Visa and the card issuing banks direclty. No, you'd use a payment processor like Stripe, Braintree. It'll be the same way with the blockchain and smart contracts. 

The difference is that this time you link up to a global, permissionless network instead of an endless chain of middlemen.

We already have projects like [Solana Pay](https://solana.com/news/solana-pay-announcement), which allow merchants to accept payments without ever needing to think about a blockchain. It ends up being a better experience than credit cards, and it's much cheaper too.

Most, if not all of the problems above can be solved with better tooling. Given that some of best engineers are flocking to the space, it seems like we'll get there.

Let's keep building!

Thanks to [Bitcoin Blaize](https://twitter.com/blaizebitcoin) for bouncing around ideas for this piece.