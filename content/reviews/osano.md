+++
date = "2021-06-03"
description = "Osano is the caddilac of cookie management providers. Read my experience after purchasing Osano."
tags = ["reviews", "cookies"]
title = "Osano Review | Comparing Consent Management Software [2021 Review]"
showtoc = true
tocopen = true
draft = false
[cover]
image = "/uploads/osano_banner.png"
alt = "Osano Review"

+++

[Osano](https://www.osano.com) is a consent management platform, also known as a cookie management software, and in my opinion it's the cadillac of cookie managers.

I've had horrendous experience with other consent platforms and Osano is truly a breath of fresh air. 

Why do I have such strong opinions about this type of software? And who the heck am I to even be talking about this?

Let me explain.

## Why trust me?

I run growth marketing for [Mailgun](https://www.mailgun.com), one of the largest email service providers in the world.

Half a million users visit our websites each month and we take data privacy, security, and GDPR compliance **very seriously**.

You tend to do that when you're processing over 22 billion emails/month.

Ever taken a ride with Lyft or received a Substack newsletter? Those emails are all sent with Mailgun.

Our user's data and security is one of our top priorities, and that includes letting users opt into or out of website cookies.

I've personally implemented both OneTrust and Osano on the Mailgun websites. After having massive issues with OneTrust I shopped for an alternative, found Osano, signed and negotiated the contract, and implemented it.

So you can trust I know what I'm talking about. 

## What is consent management?
Consent management is the process for allowing users to control the type of personal data they share with websites and advertising platforms. Consent management became important after Europe passed the GDPR law in 2018.

Consent management for websites often takes the form of a cookie banner at the bottom of your screen that allows users to accept, partially accept, or deny most cookies(but frequently not all) tracking cookies. 

Cookies have been part of the internet since web browsers gained popularity, but managing which cookies to allow or deny can often be too complex for companies to manage in-house. 

This created a new set of tools called consent management providers that build and maintain software to maintain, and store, user's consent. 

Tools like Osano store consent for you, so in the case of a legal dispute you can call your consent vendor to retreive the user's consent on your behalf. 

## What is data privacy?
Data privacy is a form of data security for managing consent, regulatory compliance(like GDPR), and notices about how data is stored and shared with third parties.

## Osano Review
![Osano Homepage Screenshot](/uploads/osano_homepage.png)

Osano is a consent management platform headquarted in Austin, Texas. They're a Series A start-up that's raised over 8 million dollars in funding. 

Osano is also a public benefit corporation, which is a different corporate structure than most companies you're familiar with.

Most companies exist to maximize profit. Public companies like Amazon and Facebook seek to maximize shareholder value, which means increasing the stock price. 

In contrast, public benefit corporations seek to maximize public benefit. In fact, their corporate charters have to specify one or more public benefits as their statement of purpose.

Osano's mission is to **put people before profits to increase data transparency.**

Data privacy will define how the internet evolves over the next decade and technology like Osano plays a major part in that. 

### Osano vs OneTrust
OneTrust is the biggest player in the consent management space. They were one of the first to market, and they have an impressive roster of current customers:

* Oracle 
* Marketo
* Akamai
* Aetna 

But in my experience OneTrust has some serious downsides. Before I get into actually using the platform, let me show you their pricing page.

![OneTrust Pricing Page](/uploads/onetrust_pricing.png)

OneTrust has **25 products** for purchase on their pricing page.

Serious [choice overload](https://en.wikipedia.org/wiki/Overchoice). Trying to purchase OneTrust is confusing, let alone implementing it on your website.  

Their cookie consent product is at the very bottom of the list, starting at $44/month. That seems like a fair price, and it is, but what other add-ons do you actually need to be compliant with GDPR and other data privacy laws?

It's honestly super unclear what you need, and the pricing page is entirely self-service. 

Ok, buying it sucks. What about using it?

Let me tell you a story. 

### A OneTrust Horror Story

After you signup for OneTrust you configure it to scan your website from their servers. It crawls your website, page by page, and records every single cookie that is placed. 

The immediate problem here is that scan takes time. Seriously, it's super slow. 

Once, or if, the scan finishes, then you need to start categorizing cookies. One by one, cookie by cookie, you have to add some data. What company uses the cookie(which is not always easy to figure out), how long it's stored for, and what type of cookie it is.

Here's the most common categories of cookies:
* Required or Essential
* Marketing
* Analytics
* Advertising

Required or Essential cookies are ones that are completly necessary to run your website or app. No, Google Analytics is not an essential cookie. Think first-party cookies that store your logged-in status: cookies that are absolutely required to ensure basic functionality of your application. 

Website cookies are not usually static, they change over time as marketing teams add new tools or start advertising on new ad networks. If you start a LinkedIn Ads campaign for the first time then you need to place the LinkedIn script on your website to track conversions. 

So you'd need to update your cookie policy to give users the ability to opt-out of LinkedIn advertising cookies. 

For OneTrust to be effective they need to periodically scan your website successfully to update your list of cookies. But what if that scan fails?

That's exactly what happened to us. 

Despite **numerous attemps** to solve it, OneTrust's scan would not finish on our website. 

We spent hours going back and forth with their support trying to nail down the problem. It was a nightmare. 

Because their scan couldn't finish we couldn't update our list of cookies. Which means we couldn't add new scripts or cookies to our website, because we couldn't update our list and be GDPR compliant. 

I couldn't test new ads or channels, which in essence means I couldn't do my job as effectively as I would've liked.

I was blocked by some shitty tool. 

We never resolved our issue with OneTrust and eventually I got the greenlight to start shopping for new tools.

And that's how I found Osano. 

### Osano Pricing
![Osano Pricing](/uploads/osano_pricing.png)

Compared to OneTrust, Osano's [pricing](https://www.osano.com/plans) is straightforward. 

There's a **free plan** for developers that allows one domain, one user, and up to 5,000 monthly visitors. 

Then there's the **business plan** that allows two domains, two users, and 30,000 monthly visitors for $99/month.

There's also **business+**, which for $199/month you get 5 users, 4 domains, and up to 50,000 monthly visitors.

For anything above that you need a Custom Enterprise plan. And that's exactly the plan we have with Osano.

If you've ever shopped for Enterprise B2B software you know it can be a pain in the ass, and that's putting it lightly. First you submit a form, then you talk to a Sales Development Rep that qualifies you, then you talk to an Account Executive, then you get a demo, then you get pricing.

It's horrible.

But that wasn't my experience with Osano. In fact, the first person I talked to was their VP of Sales. We had a short call to understand my problems, and he did a short demo of the platform on the **very first call**. 

He also gave me a rough idea of pricing.

We ended up scheduling a second call with a technical rep from Osano, then he sent me a formal contract with official pricing, and that was it.

Two calls, a short contract, and we were ready to go. 

If you're a business interested in Osano, or want a personal intro, [send me an email](mailto:nick@lafferty.co).

### Osano Features
![Osano Consents Over Time](/uploads/osano_consent.png)

Unlike OneTrust, Osano uses a Javascript snippet to determine what cookies are on your website. There's no website crawl, it all comes from a single line of code you place.

Here's how easy Osano says it is to implement their tag.

| Five minutes and one line of JavaScript on your website can instantly make your website compliant with the data privacy laws of 40 different countries. Osano intelligently blocks unsanctioned third-party cookies and displays consent dialogs in any of 42 native languages.

Osano is installed on your website by adding the code to the **very top** of your <head> tag, ensuring it's the first thing that loads on your website.

Osano works by blocking every script or cookie that loads after it, if it's not allowd by your consent and categorization rules.

Categorizing cookies in Osano is a breeze. You can define rules that allow you to categorize cookies with specific naming structures the same. 

![Osano Cookie Categorization](/uploads/osano_cookie.png)

In that screenshot I've set any script with the domain cloudfront.net to Essential. It doesn't matter what comes before or after it, it'll be categorized the same. 

Osano stores user consent for seven years in a blockchain. They have one of the best consent storage policies I've ever seen, and the use of blockchain technology is really cool.

Another feature that my legal team **loves** is the privacy policy monitoring feature. 

You can add a list of vendors to Osano and it'll track when they update the legal documents on their website, and notify you when that happens. 

![Osano Privacy Policy Monitor](/uploads/osano_diff.png)

It'll even show you what specific lines were added, deleted, or modified. 

My legal team loves it because it automates part of their job. 

Osano also sends out a weekly privacy newsletter so they can stay on top of the latest legal changes to data privacy around the world, curated by their in-house team of attorneys. Again, super useful for my legal team. 

## Why are cookies important?
I'm a professional digital marketer. I get paid to increase the amount of people that visit a website each month and make a purchase. 

Graphs of website users and revneue need to go up and to the right. 

So naturally I track those numbers. Monthly website visitors, signups, leads, form submissions. Pretty much every trackable stat on a website. 

The most popular tool to do that is Google Analytics, a free website analytics tool.

I won't get into the bigger argument of how Google collects and uses your data as a business, but what's important is that Google Analytics sets cookies in your browser.

It uses those cookies to determine when you first came to a specific website, what websites you visited before and after, how long you stay on the website, where you're located, and many other things. 

To be GDPR compliant you need to give users a way to opt-out of Google Analytics cookies on your website. If the cookie isn't placed then your data isn't tracked in Google Analytics.

Great for the user, but not so great for the professional digital marketer. I know, boo-hoo, poor me. But I have a job and I need Google Analytics to do it well. 

So I have OneTrust setup on a Mailgun website, and OneTrust is configured to allow users to disable all Analytics and Tracking cookies. But it's opt-out, so by default the cookie is placed until users revoke consent.

That type of consent is totally fine for American users in the United States, but ever since GDPR passed it's not GDPR compliant. It's a requirement of GDPR to have cookies be explicity opt-in for any European citizen browsing your website, regardless of where they're geographically located.

That means that an EU user can land on a website, not consent to cookies, and continue to browse the website without being tracked. 

That's the law, I get it, so we have to be compliant. But it presents a tricky situation to be compliant with strict European regulations but still collect data from the more lax American users. 

So what my legal team did, and if you know anything about lawyers it's that their word goes above everything else, was to implement **European compliance for 100% of our website users**. 

So we had to make all Analytics cookies opt-in by default, instead of opt-out. 

The result was we lost analytics tracking for 70% of our website users. Again, I know, poor me.

But it's not just me. It's my boss, and her boss, the CEO, and our board of directors. Everyone looks at our website numbers. And they got kneecapped overnight.

Our OneTrust implementation also made our historical data useless. If I looked at website traffic year-over-year, it would show I was down 70%. Not because something was drastically wrong, but because we weren't placing the Google Analytics cookie for most of our website users. 

I was powerless to do anything about it, and I lived in cookie policy hell.

Eventually we found updated GDPR guidlines that said you can make anonymous analytics tools opt-out by default

## Conclusion

[Osano](https://www.osano.com) is a great piece of software for managing user consent. It's truly the cadillac of consent management platforms and it's only getting better over time.

Their support team is knowledgeable and responds to my questions in record time. I've received emails back in less than 5 minutes, that's how fast it is. Shoutout to Skye from the Osano team for being a rockstar.

Give Osano a try today and tell them Nick Lafferty sent you. 

{{< button "https://www.osano.com/" "Try Osano Today" >}}