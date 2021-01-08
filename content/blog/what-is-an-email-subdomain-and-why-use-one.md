+++
affiliate = ""
canonicalurl = "https://www.mailgun.com/blog/the-basics-of-email-subdomains"
date = 2020-12-21T06:00:00Z
description = "Everything you wanted to know about email subdomains but were afraid to ask. "
lastmod = ""
tags = ["email"]
title = "What Is An Email Subdomain and Why Use One?"
showToc = true
TocOpen = true


+++
When it comes to email sending, sometimes you need more than the press of a button to get your message across. You may have heard of email subdomains, but you may be wondering - how do you use them? And, wait a minute, what exactly _are_ they?  
  
Well, have no fear, because we’re going to use this post to tell you all about email subdomains and why you need them. It’s everything you ever wanted to know about subdomains but were afraid to ask. 🤔 Now, let’s get started.

## What is a subdomain?

To explain what a subdomain is you first need to understand what domains are.

**A domain is a unique, human-readable way of identifying a website**. Often, this is referred to as the parent domain or the root domain. 

Right now, you’re on the domain **NickLafferty.com**. Behind the scenes, the domain name is connected to a unique IP address through DNS records, but memorizing a set of four numbers is a lot harder than remembering the name Mailgun.com. Because of that, the human-readable way is used for identification purposes. 

A subdomain is a prefix that comes before the root domain. 

Subdomains are often used on websites to send traffic to a different IP address while still keeping users on the same root domain. For example, Mailgun hosts their developer documentation on a separate service, so they use **[documentation.mailgun.com](https://documentation.mailgun.com/en/latest/)**.

But how does this relate to email?

## What’s the difference between an email domain and an email subdomain?

Email domains are the most common way that people send and receive emails in a professional way. Your business looks a lot more professional with a @yourdomain.com domain instead of an @gmail.com or @yahoo.com address. **Many businesses prefer to use their root domain for professional emails because it’s a way to easily verify the email is sent from the company.**

For example, Mailgun’s professional emails are all sent from **Mailgun.com**.

**An email subdomain delivers email from the subdomain instead of the root domain.** Here’s an example:

**[sam@learn.mailgun.com](mailto:sam@learn.mailgun.com)**

Learn.mailgun.com is the subdomain that Mailgun uses to send marketing messages. Every user that signs up for a Mailgun account gets a welcome email from Sam, sent from that address.

## Why should you use one?

Inbox providers like Gmail and Yahoo care about **email reputation**, which is a grade for how well users interact with your emails. If Gmail sees that their users are highly engaged with your emails, **it’s highly likely that you’re following email best practices**. But if users are sending negative signals to Gmail, like marking your email as spam, then that’s bad.

Your email reputation is based on both **domain reputation** and **IP address reputation**. We wrote more about [email reputation](https://www.mailgun.com/blog/domain-ip-reputation-gmail-care-more-about/) in a separate post, but the important part here is that subdomains have a different reputation than their root domains.

This is a good thing - otherwise, **the reputation of your** **[email marketing](https://www.mailgun.com/email-marketing/)** **campaigns could affect whether potential customers receive emails from your sales team.** 

Imagine if none of your business emails were delivered to the inbox!  

This is exactly why Mailgun recommends all customers use a subdomain when sending through our service.

## Best Practices

Many of our customers separate their **marketing emails** from their **transactional emails** through subdomains, which means they set up at least two separate subdomains to send email through. This sounds complicated, but it’s actually super easy. Later on, we’ll walk you through how to set up a Mailgun subdomain step-by-step. Here’s an example domain setup for a fake company, Meowgun. 🐱

Meowgun is a professional company that wants to send business emails from their Meowgun.com domain. They’ve configured it with Google Workspace and set up the proper DNS records.

Meowgun also wants to send a cat-facts email newsletter, and a password reset email to their users. Here are the domains they added to Mailgun:

* newsletter.meowgun.com
* reset.meowgun.com

**Note**: **The names of your subdomains don’t matter in terms of email reputation, so use whatever makes sense for you. It helps to be as clear as possible to avoid any confusion with your users.**

Meowgun hires an intern to manage their newsletter, and they accidentally send an email blast to a segment of unengaged users. As a result, their Gmail reputation decreases.

But because Meowgun’s newsletter sends through a separate email subdomain, Meowgun.com’s reputation is unaffected - and their employees continue sending and receiving email without any inboxing problems. It sounds like their intern should [read about email best practices](https://www.mailgun.com/blog/best-practices-for-successful-email-delivery/) before sending the next cat-facts newsletter, though.

## How to use an email subdomain in Mailgun

1. Login to Mailgun and **navigate to ‘Sending’ in the left-hand menu**.
2. Click the green ‘Add New Domain’ button in the top right corner of your screen.
   1. **Note: You must add a credit card to your Mailgun account before you’re allowed to add custom domains. If your button is greyed out, then you need to add a credit card before moving on.**
3. Click ‘Add Domain’
4. On the next screen Mailgun provides you with some DNS records to add to your domain.
   1. MX Records
   2. [SPF Records](https://www.mailgun.com/blog/spf-records-basics/)
   3. [DKIM Records](https://www.mailgun.com/blog/understanding-dkim-how-it-works/)

Once you’ve added your DNS records and they’ve been verified by Mailgun, **which can take up to 48 hours**, you’re good to go!

**Note**: MX records are recommended for all domains, as they’re a verification step commonly used by inbox providers. They are also required if you want to receive email at the same subdomain you added to Mailgun.

Check out this help article about [using Mailgun with a Google Workspace account](https://help.mailgun.com/hc/en-us/articles/203357040-Can-I-Use-the-Same-Domain-Name-for-Mailgun-and-for-Google-Apps-Or-Another-Email-Server-).

## Wrapping Up

Now that we’ve covered what an email subdomain is, why they’re important, and how to set one up for Mailgun, you’re ready to send some emails. Hopefully, all your questions have been answered, and you aren’t afraid to ask anything else. Onto the next mystery! 🔍

Happy sending!