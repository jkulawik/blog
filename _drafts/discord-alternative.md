---
layout: post
title:  "The futile quest for a Discord alternative"
# subtitle: "Your friends won't make the switch anyway but oh well"
tags: [software]
---

Come with me on the fruitless journey of trying to find a Discord alternative.
Preferably free and open source; self-hosting is welcome.

### The rationale

The reasons for moving away from Discord are several.

* Discord can do what it wants with our data.
The company already shows its mindset by not letting you bulk delete your messages
and refusing to delete them along with your account;
instead the account is anonymized and its message history remains.

* Discord has existed for almost 10 years and will be ramping up its monetization sooner rather than later.
Just recently it was announced that the app would start integrating ads, although this has been fairly limited so far.

* There have been talks of Discord getting sold off to Microsoft in the past.
Getting bought by any large corporation is not good news for the future of any app.
As to why that is, maybe I will write another blog post about this someday.
For now look no further than how the code editor Atom was sunset in favor of VS Code after Microsoft acquired Github,
the creators of the app.

* Honestly I don't want to pay a decent chunk of money to be able to use custom emojis anywhere I want,
or in order to raise their limit.
At the moment the price is alright,
but it has fluctuated a lot in the past when Discord shifted around the available plans.

In short, my search for a Discord alternative stems from future-proofing,
data privacy paranoia and annoyance with emoji limitations.
There's also the minor gripe of sound missing from screen sharing on Linux,
an issue which has been around for years and nothing is being done about it.

### Challenges and criteria

I mostly use Discord for interacting with small groups of friends and briefly interacting
with larger communities, which are the use-cases I had in mind while evaluating the apps here.

The more I researched for this article, the more I realised how stupidly good Discord is on
many fronts; not only features, but how much it offers for free, how accessible it is,
and its availability on many platforms.
As such, finding an alternative comes with a set of tough challenges:

* Feature parity.
Discord has a large set of features and usually *something* will be missing from the alternatives.
Some notable ones that I realized I took for granted:
  * Screen sharing
  * The reply feature (i.e. indicate which message you're replying to)
  * Rich presence (i.e. embedding thumbnails and blurbs from links).
  YouTube embeds well in most apps, but other stuff not as often (e.g. tweets).

* Pricing.
My ideal candidate would be free and open-source, like Linux, Blender or GIMP.
While I won't deny I'm a bit of a cheap bastard,
I just don't want to deal with pricing changes
and being left at the mercy of some executive chasing the bottom-line.

* Self-hosting and privacy vs accessibility.
Self-hosting puts you in control of your data (and notably also the data of the people who use your server),
but at the same time often comes with hurdles.
Getting a server to run can be technically involved to the point of stopping you from using the app altogether.
On top of that, server administration comes with its own set of woes,
like update issues.

* Self-hosting vs. interconnectivity.
Many apps are partially (TeamSpeak) or fully centralized (Discord), which lets you interact with any "server".
Self-hosted servers typically don't have this though.
The feature of enabling interactions between self-hosted servers is called federation;
it is pretty much the ideal (but rare) balance between data ownership and openness.

* How good the mobile versions of the apps are, if there is one at all.
This is however the last thing I consider, as most apps fail other fundamental criteria.

There's also the issue of convincing other users to start using something new,
but that's a whole other can of worms.

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

![(A screenshot of the Telegram desktop app)](https://dl.flathub.org/media/org/telegram/desktop/d89cd596919de725258e2feda770e650/screenshots/image-1_752x519@1.png)

[Telegram](https://telegram.org/) offers [extensive customizability](https://telegram.org/blog/android-themes),
but it seems to be a mobile app first,
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

Skype offers a weird hybrid of online chat and traditional phone features.
It is the app everyone ran from back in the day
and it seems to have stayed in that category.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: no
* Custom emoji: no
* Self-hosting: no
* Pricing: free but it's owned by Microsoft so your data is definitely being harvested


---
## Business-oriented apps

Business-oriented apps tend to focus on integrating various development tools,
log-in solutions
and other things related to corporate administration.
They're typically designed to manage projects, which can be subtly detrimental to hosting a community.
These apps are usually very robust, but lack in customization.

Since they're meant for companies, they often come with a big price tag
and require you to self-host.
While I do want self-hosting, these apps are meant to be handled by professional admins,
which means most of them will be too hard to install and operate for a regular user.

All of those reasons place the business-oriented apps as unlikely to be good Discord alternatives,
but I included them for the sake of coverage.

### Mattermost

![(A screenshot of Mattermost)](https://dl.flathub.org/media/com/mattermost/Desktop/0bf11798092500f8b581cb7431c8a187/screenshots/image-1_orig.png)

An app targeted to developers;
as far as my interests go, it is one of the more suitable alternatives for Discord.
Mattermost would be a great alternative if not for its steep monetization of the premium version.

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

Fine for business, but not very enticing for communities.

* Voice chat: kinda? I'm not sure if it's built-in or integrated
* Screen sharing: depends, video calls are through integration only
* Multichannel support: yes
* Custom emoji: yes
* Self-hosting: yes
* Pricing: free version with a 25 user cap

### Zulip

![(A screenshot of Zulip)](https://dl.flathub.org/media/org/zulip/Zulip/cf358f6f6aef4d346485f6d10049ff01/screenshots/image-1_orig.png)

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
## Matrix clients

[Matrix](https://matrix.org/) is an open communication protocol,
designed for decentralized (federated) communication.

An account can be registered with any account provider ("homeserver")
and it can interact with any other Matrix server.
Think of it as how with email you can register anywhere but talk to others.
However, migrating your data can be cumbersome if you want to switch to another server;
this is natural though and it's good that it's even an option at all.

Since they're based on the same underlying protocol,
Matrix clients mostly differ with whether they implement the following features:
* End-to-end encryption
* Spaces (equivalent to Discord's servers)
* Voice/video calls and whether these can be done in groups or 1-on-1 only

Self-hosting a Matrix homeserver can be fairly involved,
as the official implementation (called Synapse) uses Docker, which can be a double-edged sword.
Despite having worked with Docker before, I couldn't get Synapse to work (neither the single image nor with docker-compose).
It is way too technically involved for a regular person anyway,
unlike e.g. TeamSpeak where it runs as a simple executable in a single folder.

### Element

![(A screenshot of Element)](https://element.io/images/Ui-grad-homepage.png)

[Element](https://element.io/) is the most mature Matrix client app.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: yes, but a bit convoluted; previously you could only create "rooms",
which would show up along with DMs in a messy way (think of it as Discord channels only showing up on your DM list and no servers). [The recently implemented Spaces feature](https://element.io/blog/spaces-the-next-frontier/) should alleviate this issue
and it makes for a more server-like experience.
* Custom emoji: No, and [this 8 year old Github issue](https://github.com/element-hq/element-meta/issues/339)
is not boding well for the possibility of those being implemented.
* Self-hosting: yes, but it requires registration
* Pricing: free version with up to 200 users and a few limitations (specifics are hard to determine because of the jargon they use)
* Other: federated and decentralised; you have good control over your data


### Other
A list of other Matrix clients can be seen [here](https://matrix.org/ecosystem/clients/).
I will not be going over them, as they tend to have less features.

---
## General and gaming-oriented apps

These are more likely to replace Discord than business apps,
but tend to be different enough that they won't be a perfect fit.

### TeamSpeak

![(A screenshot of Zulip)](https://discourse-forums-images.s3.dualstack.us-east-2.amazonaws.com/original/3X/b/d/bde87328b5d5cfe3a1ef611aeef0d375710a2b23.png)

While great for voice chat and featuring some nice customization,
[TeamSpeak](https://teamspeak.com/en/) has an unusual approach to text chats.

Servers only have voice channels.
These have an attached text chat, which is accessible only if you're in the voice call.
It is intended for sharing links and files during calls,
and designed with privacy in mind;
people who aren't in the voice call can't read it, and chat history gets deleted after the call.

Group text chats were recently added, but as with mobile apps, these are single-channeled.
The app interface can be a bit confusing at times, even in version 5.

TeamSpeak is great if you don't text much,
but it won't be a contender for Discord until it adds regular text channels to servers.
Sadly, despite TeamSpeak memeing on Twitter about being an underdog to Discord,
they seem to move backwards on this issue;
a singular global text chat for servers [was apparently removed in TeamSpeak 5](https://community.teamspeak.com/t/global-server-chat/2458/12).

* Voice chat: yes (great one, reportedly)
* Screen sharing: in the works for over a year, but no ETA or significant news about it.
* Multichannel support: not really; tied to voice calls and temporary
* Custom emoji: yes
* Self-hosting: yes, fairly simple with no extra hoops (unlike Element)
* Pricing: free version permits owning a single server with 32 users
* Other: quite limited text chat functionality, but has a simple reply feature and a message pin feature

### Steam chat

![(A screenshot of a Steam group chat)](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fs.aolcdn.com%2Fhss%2Fstorage%2Fmidas%2Fedce1225506731ed1963fda18a6294bc%2F206551184%2Fsgteamchat.jpg&f=1&nofb=1&ipt=4609225a19614ef2ebb109e121bb4ca15513f814454b55934653714211d52338&ipo=images)

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
but seem to have the same privacy and future-proofing issues as Discord.

### Guilded

![(A screenshot of Guilded)](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fstatic1.srcdn.com%2Fwordpress%2Fwp-content%2Fuploads%2F2020%2F05%2Fguildedlogo.jpg&f=1&nofb=1&ipt=eb8da7a0e2f464fb6c20277c33297e30ae45795b71dee7c5581d9d03a80f0800&ipo=images)

Guilded offers some massively impressive features,
posing it as a good candidate for being a "Discord killer".
However, there's a tiny caveat; Guilded is owned by Roblox, a company known for shady practices on their gaming platform.

TODO elaborate on this and link stuff


The features I mentioned above include:
...



### Revolt chat

![(A screenshot of Revolt)](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdl.flathub.org%2Frepo%2Fscreenshots%2Fchat.revolt.RevoltDesktop-stable%2F1504x846%2Fchat.revolt.RevoltDesktop-e70e44718034af84ddbd1f89375bb4cd.png&f=1&nofb=1&ipt=6ae14e269eb92b8ee6b1e67e16f3a52e0175bb7dc49cdb4978b31eb3eb2d00a1&ipo=images)

I've been putting this one off because it gets pretty crazy.

On the surface, Revolt is a drop-in replacement for Discord, and it's open source!

Upon further inspection though, suspicious things start popping up.

There's no information about self-hosting on their website,
and there's a registration form, while no clear monetization scheme is presented.
This makes the future of the app questionable,
as it can go in essentially any direction when it comes to data ownership.

Revolt is not federated.
Hosting your own Revolt instance requires users to register a separate account on it
and they have no access to other instances with it.

concerning comment here:
https://itsfoss.com/revolt/

slew of technical issues on reddit
https://www.reddit.com/r/revoltchat/


> could not figure out how to successfully self host and run revolt.
>
> Going back to Mattermost
>
> sorry guys
https://www.reddit.com/r/revoltchat/comments/q0sjit/can_i_host_my_own_server_yet_or_is_there_just_one/


* Voice chat: yes
* Screen sharing: no
* Multichannel support: yes
* Custom emoji: sort-of; need to be bought with Steam Points (which are granted along any game purchase) and are limited to what's available in the store
* Self-hosting: sort of; [explanation here]. [Users will have to register a new account on your instance](https://www.reddit.com/r/revoltchat/comments/18g69gr/i_have_a_few_questions_about_selfhosting_a_revolt/).
* Pricing: free
* Other: messages cannot be edited


## Conclusions

It's so over bros.
Seriously though;
things aren't looking the best, despite the multitude of chat apps on the market right now.