+++ title = "Intelligent Email Forwarding with Mailgun" 
date = "2019-07-21" 
description = "How to setup Mailgun as a free email server for your custom domain with smart filtering." 
draft = false 
tags = ["email"]

+++

{{< note text="Mailgun has changed their pricing plans as of March 2020. As a result their routes feature is now gated behind a plan that cost $35/month. I'll update this if their pricing changes again to allow the use of routes for free." >}}

**Disclosure**: I currently work for [Mailgun](https://mailgun.com). I used their product for years before I started working here.

I've had a personal website for a long time. It's gone through lots of iterations as I've transitioned from student life to working full time. As a marketer applying for jobs in 2013 I think having a website made me stand out from other applicants. It also helped that I had this kind of ridiculous headshot of me in a suit sitting in the middle of the woods. In reality that was my parent's backyard, but either way it made me a memorable candidate.

I've always had a link to my email on my website. I feel like this is just good practice, and it's the best way to get in touch with me. The problem is bots scrape my email from the website and send unsolicited spam about boosting SEO rankings or other junk offers. I keep my spam folder tidy, even go as far as unsubscribing from spam I get (when they actually follow CAN-SPAM and give me the option to). But sometimes they don't give you the option to unsubscribe, or they make it really obtuse, or they ask you to reply back to them to unsubscribe.

Enter Mailgun. Mailgun has a routes feature for inbound mail that let's you forward mail from a domain you own to any address. I forward email from my custom domain to my gmail.

But I don't want to forward everything. I want to stop some email before it gets to my inbox at all based on it's content, like those junk SEO offers.

Here's how I use Mailgun to do that.

First, [add your domain to Mailgun](https://help.mailgun.com/hc/en-us/articles/203637190-How-Do-I-Add-a-Domain-). They've written some great guides on how to do this so I won't repeat that here. You'll also want to verify ownership of your domain by adding a few DNS records. I wrote a [step-by-step guide here.](https://help.mailgun.com/hc/en-us/articles/360026833053-Domain-Verification-Walkthrough)

I'd also recommend setting up 2FA on your account to make sure it's as secure as possible.

Next you'll want to go to the Receiving page in the interface. This is where you'll setup your rules to forward email and to stop spam. I have 3 rules setup.

1. Match Recipient

This is where you can forward all mail to a specific email address, or every message to any address at the domain, to another email address. In my example I forward one email on my custom domain to my gmail address. I recommend against forwarding all email to your domain, because spammers will send all kinds of junk to common names. I set this up as priority 1. Mailgun routes are processed in order, starting from 0. So I want my filtering rules to process first, and block any spam, and then if email passes my filters it will forward to my real email.

2. Match Headers

I have 2 rules setup for this. I added the second one later after I kept getting a lot of spam that looked like forwarded emails, which all began with "re:". So I filtered out that phrase.

Here's how I have them setup. [![Screen-Shot-2019-07-21-at-3-05-11-PM.png](https://i.postimg.cc/G3sMF2tN/Screen-Shot-2019-07-21-at-3-05-11-PM.png)](https://postimg.cc/nMpYZnvY)

You can filter based on subject line, body, or anything in the header itself. I setup my filters to catch common cases I would see. Once you setup your filter, you need to decide what action to take. The proper action here is stop, which will do nothing to the emails, as long as the priority is lower than your forward filter.

Once your filters are setup you can go to the Logs page to see what emails you're getting. Any email that passes your filter will show as 'Delivered', emails that don't will stop at 'Accepted'.

[![Screen-Shot-2019-07-21-at-3-09-30-PM.png](https://i.postimg.cc/GpWDdcR8/Screen-Shot-2019-07-21-at-3-09-30-PM.png)](https://postimg.cc/xkP8PVcn)

Have you thought of any creative ways to use Mailgun's routes feature? Send me an email!