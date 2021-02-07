+++
date = 2020-12-31
description = "See how easy it is to setup link click tracking in Google Analytics."
tags = ["marketing"]
title = "Setup Google Analytics Click Tracking in 5 Minutes"
showtoc = true
tocopen = true
draft = false

+++
## Overview
I want to track how many clicks I send to specific external website, then I want to compare total clicks to how many views that page gets to calculate a click-through-rate. 

This isn't enabled by default in the old Google Analytics, but it is in Google Analyyics v4.

Google Analytics is only as useful as the data you feed into it. Google Tag Manager(GTM) is a powerful and fast way to send data into Google Analytics. I recommend every digital marketer learn GTM. 

## Prerequisites
* Publish access to Google Tag Manager
* Google Analytics

## How to Setup Click Tracking in Google Analytics
### Add Click URL Variables to GTM
First you'll need to add some of the built-in variables to your GTM container, if you haven't already.

Go to Variables then click Configure.

Scroll down and enable Click URL.

![GTM Click Variables](/uploads/GTM_Variables.png)

### Setup a trigger
Create a new trigger that looks for Clicks to a specific URL. Here's what mine looks like.

![GTM Click Trigger](/uploads/Click_Trigger.png)

### Setup a GA Event Tag
Now that we have the trigger setup, we need to build the tag that sends the data to Google Analyyics. 

Create a new GA Universal Analytics tag.

**Make sure to change the type to Event.**

All of the variables like Category, Action, and Label are up to you. Try and keep them consistent, so if you add other events you can easily understand them. 

Here's what mine looks like

![GTM GA Tag](/uploads/GA_Tag.png)

### Publish
That's it! 

You can check that it's working correctly using GTM's preview mode.

Click Preview and type in your website URL. 

Then navigate to a page that has the link you want to check on it. 

Click on your link, then head back to GTM's debugger. You should see this.

![GTM Preview Mode](/uploads/GTM_Preview.png)

## Track Link Clicks in Google Analytics V4
Luckily this is on by default! You can check by going to:
Admin -> Data Streams (under Property) -> Click on your website

![GA V4](/uploads/GA_V4.png)

