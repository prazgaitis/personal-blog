---
title: "QR Code credit card fraud - Covid style"
date: "2020-07-14 10:30"
description: "How fraudsters can steal your credit card info with a QR code and outdoor dining"
hidden: false
---

![credit card at a restaurant](https://images.unsplash.com/photo-1572798793834-67d5e285760d?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&ixid=eyJhcHBfaWQiOjYzOTIxfQ&w=3600)
A few days ago, a friend (lets call her Eli) told me about how someone stole her credit card info at a restaurant.

We're in Chicago in the middle of the Covid-19 pandemic. Restaurants have started to open back up, but only those with outdoor seating. To avoid spreading Covid, some restaurants are placing a laminated piece of paper with a QR code on each table.

This QR code links to a menu on the restaurant's website. What a great idea! Restaurants don't need to hand out menus, in fact they don't even have to print them anymore! They can update the menu in realtime as things go out of stock or the selection changes.

When Eli sat down at this restaurant in Chicago, she used the QR code to open up the menu and browsed around for a bit. After a few minutes, a pop-up asked her to enter her credit card info for a seamless checkout.

Hmm. This is where alarm bells might go off, but remember - we're in the middle of a pandemic. Passing credit cards to a server is dangerous! What if they have covid? What if _you_ have Covid and you infect your server? It would be best to have everything be contactless. Eli entered her card info, thinking that this was actually a pretty good user experience.

As you may have guessed by now, it wasn't the restaurant collecting her credit card info. Someone placed a fake menu on the table with a QR code pointing to their own phishing site. This seems pretty easy to do. Someone could walk by and place fake menus on a few tables.

On the tech side, things are even easier. The attacker can register a generic sounding domain, eg. lookatmenu.app. Next, they create a unique QR code for each target restaurant. You don't even need a separate domain for each restaurant. Just add the restaurant's actual menu URL as a query parameter. Eg: [https://lookatmenu.app?s=https://orders.giordanos.com/#/menu/national/ToGo/Pickup](<https://lookatmenu.app/?s=%5Bhttps://orders.giordanos.com/#/menu/national/ToGo/Pickup%5D(https://orders.giordanos.com/#/menu/national/ToGo/Pickup)>)

You can pass this query string into an iFrame, which makes it look like you're actually on [giordanos.com](http://giordanos.com/). After a few seconds, simply show a popup to a payment form of your choosing.

In Eli's case, it was some sort of nondescript subscription service. If it's something with a generic name for a \$20/month or so, a lot of people might not notice for a long time.

[Here's a codepen with example code](https://codepen.io/pranas/pen/rNxZMMy).

## **So, how do I protect myself?**

1. Always look at the URL of the page when entering credit card info. If anything seems off, don't enter your payment info.
2. Be sure to ask the server if the menu is legit.

Although I hate to hear stories like this, it's always interesting to see how fraudsters exploit technology and our trust. Luckily, my friend's credit card company refunded the charges and issued a new card.

Stay safe out there!
