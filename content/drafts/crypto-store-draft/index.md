---
title: "[Draft] Sell anything online. For free."
date: "2022-03-09 10:30"
description: "Sell stuff, get paid in crypto" 
hidden: true
---

### Side project? Or a one-way ticket to prison? 

I recently stumbled upon a project that was intriguing because it was so simple. It's called [onetem.store](https://oneitem.store).

It's an online store builder, but that's not what makes it interesting. There are hundreds of those, but this one is cool because of what it _doesn't_ do. There's no inventory, no shipping tracker, no pop-ups. [The creator built it in about a week](https://tinyprojects.dev/projects/one_item_store) and then sold it for a couple thousand bucks. Not bad!

This got me thinking. Can we do better? What if we could skip the part where you pay 3% tax to Stripe? Disclaimer: I think Stripe is great. I use them professionally and I love the product and the folks who build it. It's well worth the 3-ish percent fee.

A bit of background. My day job is at [Cameo.com](https://www.cameo.com/praz?ref=blog), where I'm the Tech lead of the Payments team. We do regular Web2 marketplace-style payments, but recently we've also taken the plunge into [Web3](https://pass.cameo.com). We'll have more to announce in this area soon. As for me, I've been interested in crypto ever since the run in 2017. I work in the Payments space, so it's a professional obligation to stay up to date on the latest tech.


If you follow crytpto at all, you've heard of Solana. At a very high level, it's a blockchain that is kinda like Ethereum, except it can handle can handle thousands of transactions per second at very little cost. Instead of proof of stake, they use something called proof of history. [Check this out](https://2501babe.github.io/posts/solana101.html) for a good explanation.


For me, it hit home when I fired up my terminal and sent a couple bucks to a friend _instantly_ with Solana. And it was free! It reminded me of the first time I used Venmo, except this was even better - there's no middleman, no account verification, nothing.

The team at Solana Labs just released [Solana Pay](https://solana.com/news/solana-pay-announcement), which is basically a pre-built smart contract and some Javascript libraries that let merchants easily accept payments. Payments can happen in Solana, the project's native currency or USDC.

This sounds like the perfect way to do payments at (essentially) zero cost for our online store!
### **online store**  🤝  **instant, free payments**

I quickly hacked together a prototype, [which you can try here](https://crypto-store.vercel.app/).

![create a new store](./create-store.png)

<!-- And so the Simple Crypto Store (plz help me find a better name) was born! You can create an online store in 30 seconds and start selling your stuff right away. No payment processor needed. Zero payment processing fees. -->

### Why would I use this?

Do you sell stuff online? Are you tired of paying up to [9% fees on Gumroad](https://gumroad.com/pricing)?

## Problems (besides Jail)

This project might end with me in prison, but we'll get to that in a bit. Let's talk about the problems of accepting crypto payments as a merchant.
### There's no such thing as chargebacks in crypto
Chargebacks are a pain for merchants, but they're great for buyers. Got charged for something that didn't show up in the mail? Call Chase and they'll take it off your statement. Let's say you buy something with Solana and it never shows up. Who do you call? Sorry Karen, there's no manager you can speak to. This is a real problem for buyers!

### Who pays the fees?
Credit card processors involve a handful of steps, and each step costs money. The card issuers, the merchant's bank, Visa & Mastercard, and more all need to get paid when you swipe the plastic. In crypto and web3, the buyer pays the transaction fee. You've likely heard about the high gas fees on Ethereum. Solana solves this - most transactions cost fractions of a penny.

### Your buyer needs to have a crypto wallet
This one is pretty obvious - if you collect crypto payments, only people who have a wallet can be your customers. The number of people with a wallet will grow over time, but it's not very large yet.

<!-- Because you're the product, of course. American Express has their hand in both jars. You get to fork over $600 a year for the privilege of dropping that Platinum card on the table in front of all your friends. But they're also taking a cut of that transaction on the back end! (Remember when some businesses didn't accept Amex?) Different cards cost more for merchants to accept. -->
## Ok, so how do we solve these problems?
If the goal is to enable free, instantaneous value transfer, then something like Solana gets us pretty darn close. We still have the problem of purchase non-fuflillment, which credit cards solve with Chargebacks.


One way to solve this problem is with an escrow payment. Another (weaker) option is social proof, like reviews. 

Escrow payments would work, but then you need to bring in a third party. This would only make sense for higher value transactions because it's operationally expensive.

Could reviews work? The nice part about a public database (aka a blockchain) is that anyone can read it. We can verify that a review is legit, because we can see that this person actually bought the thing that they're reviewing.

Has this worked in the past? Reviews worked great for Airbnb, but not as well for Amazon. It's well known that most Amazon reviews [are bullshit](https://www.amzfinder.com/blog/top-100-facebook-groups-list-amazon-reviews/).

Reviews seemed to work pretty well on the Silk Road, which brings us back to the Jail part. If anyone can sign up and sell anything relatively anonymously, there's a chance that bad people start selling bad things. 

In this regard, the Simple Crypto Store looks a lot like the Silk road. We've heard this story before, and the other guy is [sitting in a jail cell](https://www.investopedia.com/tech/ross-ulbricht-dark-net-pirate/). Please don't sell illegal stuff here. I like being not in jail.

### Roadmap

I think this project could go a lot of ways. Adding reviews would be cool, and maybe necessary. When I figure out how to do it, I'll need to add the ability to pay with ETH and Bitcoin Lighning ([let me know](https://twitter.com/prazgaitis) if you have tips on how to do it!).

There are a few ways I'd like to try and monetize this project. I'd like to keep payment processing free for merchants. A 1-2% fee is still less than a merchant would pay anywhere else, and it would be a nice deterrant to prevent money laundering. Shopify charges a monthly fee, so that's another option. Another option is offering escrow for larger transactions. There are also upsell opportunities -- give merchants the ability to sell multiple products, multiple photos per product, custom domains, memberships, digital downloads, etc. The opportunities are endless!

Let me know what you think, and if you have something to sell, let's do it! 🚀