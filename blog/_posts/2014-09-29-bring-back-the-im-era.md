---
layout: post
title:  "Bring back the IMera!"
date:   2014-09-29
tags: [xmpp,jabber,ejabberd]
comments: true
---


A few years ago I decided to start a Jabber/XMPP server for a few close friends as an experiment. Now it has become something a little bit larger and has changed what I think of the status quo.

## History

At first, I started my Jabber network as a free service for my friends and the only price I had to pay was living in the same room as a rack server. If you're not farmiliar with the hardware, a 2U-sized server usually sounds a little bit louder than a normal vaccuum cleaner, but not quite as loud as a large shop-vac. Originally the server was running Debian (lenny) with [OpenFire](www.igniterealtime.org/projects/openfire). Then, I moved across the country for college. My parents were nice enough to let me keep the servers running, even though it's not exactly cheap to run a server like that reliably. Surprisingly, it worked really well for about two years--also, the internet connection was Comcast Cable. Then, network hardware began to fail, and I wasn't able to fix it quickly enough--I was across the country, so my parents had to help me remotely. 

The hardware issues brought the jabber services down intermittantly on a few different occasions. The worst outage was for about a week where many people switched to Facebook chat as their next-best alternate chat medium. Since so many people depended upon the service, I got numerous complaints from them about the uptime and reliability of the network. At this point there were probably 20 active users on consistently and a little more than 150 registered users. I needed to move the server somewhere more reliable.

## New and Improved!

The best parts about technical difficulties in time-critical situations are hot-fixes. Since services are down, it's actually an excellent opportunity to experiment and add new features to your product. It's also easier to see what functionality you can remove without your users noticing, helping you create a more lean system. Obviously, there are some caveats to this approach for improvement, but for a small-scale Jabber network it can be reasonable to take advantage of down-time like this.

I ended up changing multiple things like the OS, the server daemon and authentication system entirely. Exporting user data from OpenFire was a bit of a pain in the ass. Most online communities really doesn't like it when you ask questions like "how do I move all of my users from your <em>current_closed-source_software</em> to one like <em>insert_open-source_competitor_here</em>", on IRC these questions remain ignored at best. I forgot exactly what I did (in python) to do the switch, but it ended up working pretty well and migrated the services without many problems. I chose [eJabberd](http://www.ejabberd.im) since it has a great community and can scale much better than OpenFire can; furthermore, I was also looking for a handy excuse to learn function programming and eJabberd is written in Erlang!

I ended up retiring all of the hardware I was hosting at my parents' house. I am a college student who moves frequently and in order to prevent these problems from happening again, I needed to host this service independantly from where I live. I decided to host my server on DigitalOcean because it's dirt-cheap and reliable. I have had two downtimes in the past year and both were for less than 2 minutes, that's good enough for me. I have had no complaints about reliability and my Jabber network continues to acquire new users. In the future, I plan on setting up a few redundant instances of my jabber network on various different hosts in a cluster.

## Reflection

Reliability is key, especially in communications. I'm sure that 50% of my jabber network is used to coordinate drinking activities among my college friend group, but even that has to happen reliably--and I'm glad I am able to help. Despite the fact these conversations are not exactly "mission-critical", I always hear about a downtime within 30 sec or less (I usually know before they do). If both of those things are correct, maybe my jabber network is probably the closest thing to an alcoholics' anonymous chatting network.

I have no idea why my Jabber service has gained any traction, there are plenty of other options available with higher levels of "leet" (e.g., IRC). My Jabber network requires the user to install new software, and spend time configuring some things manually--it's not polished, and yet, people still continue to register and reccomend it. I've asked a couple of people why and I've heard anything from NSA-bashing to "it's just the right-level of leet"; however, I have a different theory.

## IM Nostalgia

My friend group is mostly people born in the 1990's and I'd bet that most of used AIM and MSN as their first instant messaging platform. Now the interface has changed from the old chat window to weird tabs things on the bottom right of your desktop (google hangouts). Most chatting isn't even done with a desktop client anymore (e.g., Facebook Chat). All of the tech giants seem to be diverging from the original IM look and feel, and I think they're getting it wrong (except for iMessage). I think that people from my generation want the old back, and it's becoming more and more scarse. I suspect that small-scale chat networks like mine would not have gained any traction when market was dominated by AIM and MSN.

Maybe the market is moving in the other direction for a good reason, or perhaps the only explination for anyone to use a private jabber network is NSA-fear. I'm not exactly sure, but I'll keep hosting this jabber server for the nostalgic 90s kids like myself. 