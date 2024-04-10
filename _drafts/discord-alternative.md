---
layout: post
title:  "The futile quest for a Discord alternative"
subtitle: "Your friends won't make the switch anyway but oh well"
tags: [software]
---

Come with me on the fruitless journey of trying to find a Discord alternative.
Preferably free and open source; otherwise the option of self-hosting is welcome.
I mostly use Discord for interacting with small groups of friends and briefly interacting
with larger communities, which are the use-cases I will be evaluating the apps here.

The rationale for moving away from Discord is as follows:
* Discord can do what it wants with our data,
and it already shows its mindset by not letting you bulk delete your messages
and refusing to delete them along with your account
(deleting your account only anonymizes your account, while its message history remains)
* Discord has existed for almost 10 years and will be ramping up its monetization sooner rather than later.
Just recently it was announced that the app would start integrating ads, although this has been fairly limited so far.
* There have been talks of Discord getting sold off to Microsoft in the past
* Honestly I don't want to pay a decent chunk of money to be able to use custom emojis anywhere I want,
or in order to raise their limit

In other words, my search stems from future-proofing, data privacy paranoia and annoyance with emoji limitations.

Finding an alternative to the powerhouse that Discord is comes with a set of tough challenges:
* Convincing other users to start using something else, but that's a whole other can of worms.
* Discord has a large set of features and usually *something* will be missing from the alternatives.
Some notable features that I realized I took for granted:
  * Screen sharing
  * The reply feature (i.e. indicate which message you're replying to)
  * Rich presence (i.e. embedding thumbnails and blurbs from links).
  YouTube embeds well in most apps, but other stuff not as often (e.g. tweets).
* How good the mobile versions of the apps are, if there is one at all.
This is however the last thing I consider, as most apps fail other basic criteria
* Privacy and accessibility are usually a trade-off.
Apps with self-hosting tend to be business oriented
and apps which offer free registration vary with their privacy,
which often cannot be easily discerned.


---
## Texting apps

Texting apps which are focused on direct messaging and group chats are a dime a dozen.

These won't replace Discord, but are worth mentioning to establish what I'm going for,
since many "Discord alternatives" articles tend to act like these are even remotely suitable.

While not necessarily bad for what they are, texting apps aren't in Discord's ballpark.
They tend to be mobile-first apps too, which usually makes for a clunky desktop experience.
Examples:
* WhatsApp
* Messenger
* Signal (A+ for privacy though)

Feature-wise they tend to be very similar:
* Voice chat: usually
* Screen sharing: somewhat rare
* Multichannel support: never
* Custom emoji: no
* Self-hosting: no
* Pricing: free but your data is likely being harvested

### Telegram

Telegram offers extensive customizability, but it seems to be a mobile app first,
so in some ways it might be a bit simplistic.
Other than that it seems like a good candidate.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: yes, called "topics", but these [might interfere with a few other features](https://caribbean.dev/telegram-group-topics-the-pros-and-the-cons/).
Note that this issue might be resolved already.
* Custom emoji: yes
* Self-hosting: no
* Pricing: free, with some premium features behind a paywall
* Other: reportedly privacy-friendly, supports message pinning

### Skype

Skype is a weird hybrid of a web app and traditional phone features.
It is the app everyone ran from back in the day
and it seems to have stayed in that category.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: no
* Custom emoji: no
* Self-hosting: no
* Pricing: free but it's owned by Microsoft so they're definitely harvesting your data


---
## Business-oriented apps

Business-oriented apps tend to focus on integrating various development tools,
log-in solutions
and other things related to corporate administration.
They're typically designed to manage projects, which can be subtly detrimental to hosting a community.
These apps are usually very robust, but lack in customization.
Since they're meant for companies, they tend to come with a big price tag
and have no option of registering outside a self-hosted instance.

All of those reasons place the business-oriented apps as unlikely to be good Discord alternatives.
There's also surprisingly many of these, so I wasn't able to analyze them in as much depth as the other ones.

### Mattermost

An app targeted to developers;
as far as my interests go, it is one of the more suitable alternatives for Discord.
Mattermost would be a great alternative if not for its steep monetization of the premium version.
If you don't need group calls, look no further; but you probably do need those.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: yes
* Custom emoji: yes
* Self-hosting: yes
* Pricing: there's a free option which limits voice chat to 1-on-1 calls;
the next license is $10 per month *per user*, sadly making Mattermost quite hostile to hosting even small communities.

PS. Apparently the 1:1 call limit was introduced very recently.
Massive bummer because it would have been the best fit for my use-case.
This is a good example of how company-owned software can pull the rug from under your feet
and is one of the reasons why I prefer FOSS solutions.

### Slack

Widely used business app, but similarly to Mattermost it has a per-user payment plan.
The lack of self-hosting eliminates the main advantage of using a business-oriented app.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: yes
* Custom emoji: yes
* Self-hosting: no
* Pricing: free version which limits voice chat to 1-on-1 calls and restricts you to a single "server" (workspace)


### Rocket chat

Probably fine for business, but not very enticing for communities.

* Voice chat: kinda? I'm not sure if it's built-in or integrated
* Screen sharing: depends, video calls are through integration only
* Multichannel support: yes
* Custom emoji: yes
* Self-hosting: yes
* Pricing: free version with a 25 user cap


### Element

Element uses an open communication protocol called [Matrix](https://matrix.org/),
designed for decentralized communication and is the most mature client app based on it.
It is one of the better of the business-oriented apps.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: yes, but a bit convoluted; previously you could only create "rooms",
which would show up along with DMs in a messy way (think of it as Discord channels only showing up on your DM list and no servers). [The ecently implemented Spaces feature](https://element.io/blog/spaces-the-next-frontier/) should alleviate this issue
and it makes for a more server-like experience.
* Custom emoji: No, and [this 8 year old Github issue](https://github.com/element-hq/element-meta/issues/339)
is not boding well for the possibility of those being implemented.
* Self-hosting: yes
* Pricing: free version should be sufficient
* Other: federated and decentralised; you have good control over your data

### Zulip

Zulip is a pretty good app for businesses,
but the lack of built-in voice/video calls is a shame.

Instead of servers, there are organizations,
so owning multiple servers does not sound very plausible.
Zulip uses a subscription-based channel approach;
an organization has hashtagged "streams", where you discuss separate topics.
Think of it as if you couldn't talk in a Discord channel directly and had to always start threads instead.
It's not the worst approach for a business, but pretty bad for a community.

* Voice chat: not native - integrates with Zoom or Jitsi
* Screen sharing: same as the above
* Multichannel support: threads-only, subscription based
* Custom emoji: yes
* Self-hosting: yes
* Pricing: free version with pretty much all the features you need
* Other: open source

### Google workspace

Google offers a good set of collaboration tools highly focused on business,
including tightly integrated voice call and chat apps.
Google Chat is based on group chats however and Google Workspace has no free option;
these factors make it not worth looking into any further.

### Microsoft Teams

Crapware with annoying hick-ups every few moments,
which in classic Microsoft fashion has an unintuitive interface with features hidden in obscure places.
The video chat is really solid, but asides from that do yourself a favor and don't bother with this thing.


---
## General and gaming-oriented apps

These are more likely to replace Discord than business apps,
but tend to be different enough that they won't be a perfect fit.

### TeamSpeak

While great for voice chat and featuring some nice customization,
TeamSpeak has a... specific approach to text chats.

Servers only have voice channels.
These have an attached text chat, which is accessible only if you're in the voice call.
This is mostly for the purpose of sharing links and files during calls,
but it's intended as private and chat history gets deleted after the call.

Group text chats were recently added, but as with mobile apps, these are single-channeled.
The app interface can be a bit confusing at times, even in version 5.

TeamSpeak is great if you mostly use Discord for voice calls,
but it is not a contender until it adds regular text channels to servers.
Sadly, despite TeamSpeak memeing about being an underdog to Discord on Twitter,
they seem to move backwards on this issue;
a singular global text chat for servers [was apparently removed in TeamSpeak 5](https://community.teamspeak.com/t/global-server-chat/2458/12).

* Voice chat: yes (great one, reportedly)
* Screen sharing: in the works for over a year, but no ETA or significant news about it.
* Multichannel support: not really (voice only)
* Custom emoji: yes
* Self-hosting: yes
* Pricing: free version which permits owning a single server with 32 users
* Other: quite limited text chat functionality, has a simple reply feature

### Steam chat

Bet you didn't expect this one, huh?
Steam's group chat feature offers a server-like experience now.
It's remarkably similar to Discord in the way it works, but much simpler.

* Voice chat: yes
* Screen sharing: no
* Multichannel support: yes
* Custom emoji: sort-of; need to be bought with Steam Points (which are granted along any game purchase) and are limited to what's available in the store
* Self-hosting: no
* Pricing: free
* Other: messages cannot be edited


### Mumble

Mumble is a voice chat app similar to TeamSpeak,
but it seems to have even less text chat capabilities;
in fact as far as I can tell, it doesn't have one at all.
It is a free open-source alternative to TeamSpeak though, if you want one.

### IRC

IRC is a classic but only uses plain text (no emojis, reactions etc.)
and as a text chat protocol, has no voice chat by definition.


---
## Discord clones

These might seem like the best pick at first,
but the issue is that you don't get control over your data.
These share Discord's freeware approach of "free until 


### Guilded

### Revolt chat

I've been putting this one off because it gets pretty crazy.

On the surface, Revolt is a drop-in replacement for Discord, and it's open source!

Upon further inspection though, suspicious things start popping up.

There's no information about self-hosting on their website,
and there's a registration form, while no clear monetization scheme is presented.
This makes the future of the app questionable,
as it can go in essentially any direction when it comes to data ownership.

concerning comment here:
https://itsfoss.com/revolt/

slew of technical issues on reddit
https://www.reddit.com/r/revoltchat/




## Conclusions

