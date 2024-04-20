---
layout: post
title:  "The futile quest for a Discord alternative"
# subtitle: "Your friends won't make the switch anyway but oh well"
tags: [software]
---

Come with me on the fruitless journey of trying to find a good Discord replacement.
Preferably free, open source and self-hostable.

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
the creators of Atom.

* Paywalled features. At the moment the price of Nitro is alright,
but it has fluctuated a lot in the past when Discord shifted around the available plans.
In a similar vein, Discord decided to lock certain features behind turning servers
into open communities (e.g. announcement channels).

In short, my search for a Discord alternative stems from future-proofing,
data privacy paranoia and annoyance with emoji limitations.
There's also the minor gripe of sound missing from screen sharing on Linux,
an issue which has been around for years and nothing is being done about it.

[This post on Reddit](https://www.reddit.com/r/pcgaming/comments/di0cqz/new_teamspeak_beta_with_free_voice_chat_text_chat/)
has a really cool comment that puts it well:
>  That's the main thing about Discord. **For now**, it's mostly free (as in free beer, NOT free speech); and there hasn't been big breaches, scandals or issues (as far as I know). But it's a fully hosted solution, where we user and community handlers have **zero control and guarantees**.
>
> Tomorrow Discord can have advertisement, selling outrageous amount of telemetry, ask everyone to pay, or anything else. If you think that's science-fiction, you're too young to remember when Movable Type was the hot thing on the interweb and almost everyone used it "because it's free".
>
> That's what Teamspeak and Mumble have. Control is in our hands. Even more so with Mumble, because it's open source. 

Lastly, I do not plan on moving away from Discord yet;
but if shit hits the fan, I want to have an overview on what to replace it with.

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
I just don't want to be left at the mercy of some executive chasing the bottom-line.

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

* Mobile client apps. How good they are, and if there is one at all.
This is however the last thing I consider, as most apps fail other fundamental criteria.

* Convincing other users to switch to the app.
I can make sacrifices in some regard, but convincing others to do so
would be making this task harder than it already is.


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

It's also worth noting that many of these use the XMPP protocol,
but as far as I can tell it doesn't have any interoperable clients
similar to Discord.

### Telegram

![(A screenshot of the Telegram desktop app)](https://dl.flathub.org/media/org/telegram/desktop/d89cd596919de725258e2feda770e650/screenshots/image-1_752x519@1.png)

[Telegram](https://telegram.org/) offers [extensive customizability](https://telegram.org/blog/android-themes),
but it seems to be a mobile app first,
so in some ways it might be a bit simplistic.
Other than that it seems like a good candidate.

One great feature of Telegram is its privacy:
> All data is stored heavily encrypted and the encryption keys in each case are stored in several other data centers in different jurisdictions. This way local engineers or physical intruders cannot get access to user data.

* Voice chat: yes
* Screen sharing: yes
* Multichannel support: yes, called "topics", but these [might interfere with a few other features](https://caribbean.dev/telegram-group-topics-the-pros-and-the-cons/).
Note that this issue might be resolved already.
* Custom emoji: yes
* Self-hosting: no
* Pricing: free, with some premium features behind a paywall
* Other: supports message pinning

PS. Telegram has some crazy stuff going on behind the scenes.
It was made by Russians who are now moving the company around the world and the company itself
"has a complex corporate structure of shell companies to delay complying with government subpoenas".

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

Since they're meant for companies, they come with a big price tag and require self-hosting.
These apps are meant to be deployed by professional admins,
which means most of them will be too hard to install and operate for a regular user.

All of those reasons place the business-oriented apps as unlikely to be good Discord alternatives,
but I included them to cover all bases.
As such, I decided not to go too much in depth about them for the sake of brevity.

Lastly, a note about Jitsi Meet: it's a free and open-source video conference platform,
which seems pretty decent from my experience with it and has most of the features from Discord
(even the reaction soundboard). Many apps can integrate Jitsi as their voice call platform,
and it can be self-hosted.

### Mattermost

![(A screenshot of Mattermost)](https://dl.flathub.org/media/com/mattermost/Desktop/0bf11798092500f8b581cb7431c8a187/screenshots/image-1_orig.png)

An app targeted to developers;
as far as my interests go, it is one of the more suitable alternatives for Discord.
Mattermost would be a great alternative if not for its steep monetization of the premium version.

* Voice chat: several integrations to choose from
* Screen sharing: depends on integration
* Multichannel support: yes
* Custom emoji: yes
* Self-hosting: yes
* Pricing: there's a free option which limits voice chat to 1-on-1 calls;
the next license is $10 per month *per user*, sadly making Mattermost quite hostile to hosting even small communities.
* Other: has a mobile app

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

A decent app that's a pretty strong contender,
but still has all the licensing trappings related to being business-oriented.
I've used it a fair bit and there's some clunkiness in the interface;
while feature-wise it's a good fit for me, something about this app doesn't entice me.

* Voice chat: several integrations, including Jitsi
* Screen sharing: same as the above
* Multichannel support: yes, but the way they're laid out is a bit confusing
* Custom emoji: yes
* Self-hosting: yes
* Pricing: free version with a 25 user cap
* Other: open-source

### Zulip

Zulip uses a subscription-based channel approach;
an organization (server) has hashtagged "streams", where you discuss separate topics.
Think of it as if you couldn't talk in a Discord channel directly and had to always start threads instead.
I think this design atomizes discussions too much, but it might be a matter of taste.

* Voice chat: integrates with Zoom or Jitsi
* Screen sharing: same as the above
* Multichannel support: threads-only, subscription based
* Custom emoji: yes
* Self-hosting: yes
* Pricing: free version with pretty much all the features you need
* Other: open-source

### Google Workspace

Google Workspace offers a good set of collaboration tools,
including tightly integrated voice call and chat apps,
but it is fully dedicated to business and has no free option.
Google Chat (a part of Workspace) can be used separately,
but it offers only group chats.

### Microsoft Teams

Crapware with annoying hick-ups every few moments,
which in classic Microsoft fashion has an unintuitive interface with features hidden in obscure places.
The video chat is really solid, but asides from that do yourself a favor and don't bother with this thing.


---
## Matrix

[Matrix](https://matrix.org/) is an open communication protocol,
designed for decentralized (federated) communication.

An account can be registered with any account provider ("homeserver")
and it can interact with any other Matrix server.
Kind of like with email where you can register anywhere and still talk to others.

Since they're based on the same underlying protocol,
Matrix clients mostly differ with whether they implement the following features:
* End-to-end encryption
* Spaces (equivalent to Discord's servers)
* Voice/video calls and whether these can be done in groups or 1-on-1 only

Self-hosting a Matrix homeserver can be fairly involved,
as the official implementation (called Synapse) uses Docker, which can be a double-edged sword.
Despite having worked with Docker before,
I couldn't get Synapse to work (neither the single image version nor with docker-compose)
and would have to spend a good hour or two trying to figure it out.
It is way too technically involved for a regular person anyway,
unlike e.g. TeamSpeak where it runs as a simple executable in a single folder.

There's always the option of registering an account on a free matrix instance.
Note that [matrix.org apparently censors users quite heavily, so it might be a better idea to register elsewhere](https://tatsumoto-ren.github.io/blog/list-of-matrix-servers.html).
This gets you back into the good old "not owning your data" situation though.
Worse yet, reading the above link goes to show that instance admins have the power
to delete your chat rooms and accounts at will.

### Element

![(A screenshot of Element)](https://element.io/images/Ui-grad-homepage.png)

[Element](https://element.io/) (previously Riot) is the most mature Matrix client app.

* Voice chat: yes, and [it's native](https://element.io/blog/introducing-native-matrix-voip-with-element-call/)!
* Screen sharing: yes
* Multichannel support: yes, but a bit convoluted; previously you could only create "rooms",
which would show up along with DMs in a messy way (think of it as Discord group chats).
[The recently implemented Spaces feature](https://element.io/blog/spaces-the-next-frontier/) should alleviate this issue
and it makes for a more server-like experience.
* Custom emoji: No, and [this 8 year old Github issue](https://github.com/element-hq/element-meta/issues/339)
is not boding well for the possibility of those being implemented.
There is a [Matrix feature proposal](https://github.com/matrix-org/matrix-spec-proposals/pull/1951) for them too,
but it's 5 years old and not merged yet.
* Self-hosting: yes
* Pricing: free version with up to 200 users and a few limitations (specifics are hard to determine because of the jargon they use)
* Other:
  * Federated and decentralised; you have good control over your data
  * Seems to have some nice features that aren't listed directly on websites
  * Has a decent mobile version
  * Supports bots and offers several ones already


### Other
A list of other Matrix clients can be seen [here](https://matrix.org/ecosystem/clients/).
I will not be going over them, as they tend to have less features.

---
## General and gaming-oriented apps

These are more likely to replace Discord than business apps,
but tend to be different enough that they won't be a perfect fit.

### TeamSpeak

![(A screenshot of TeamSpeak)](https://discourse-forums-images.s3.dualstack.us-east-2.amazonaws.com/original/3X/b/d/bde87328b5d5cfe3a1ef611aeef0d375710a2b23.png)

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
* Other:
  * Limited text chat functionality but has a simple reply feature and a message pin feature
  * Has been around for ages, so while still a proprietary app, it is pretty trustworthy

### Steam chat

![(A screenshot of a Steam group chat)](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fs.aolcdn.com%2Fhss%2Fstorage%2Fmidas%2Fedce1225506731ed1963fda18a6294bc%2F206551184%2Fsgteamchat.jpg&f=1&nofb=1&ipt=4609225a19614ef2ebb109e121bb4ca15513f814454b55934653714211d52338&ipo=images)

Bet you didn't expect this one, huh?
Steam's group chat feature offers a server-like experience now.
It's remarkably similar to Discord in the way it works, but muuuch simpler.

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

These might seem like the obvious pick at first,
but can have the same privacy and future-proofing issues as Discord.

### Guilded

![(A screenshot of Guilded)](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fstatic1.srcdn.com%2Fwordpress%2Fwp-content%2Fuploads%2F2020%2F05%2Fguildedlogo.jpg&f=1&nofb=1&ipt=eb8da7a0e2f464fb6c20277c33297e30ae45795b71dee7c5581d9d03a80f0800&ipo=images)

Guilded offers some massively impressive features,
posing it as a good candidate for being a "Discord killer".
However, there's a tiny caveat; Guilded is owned by Roblox,
a company known for shady practices on their gaming platform
(like earning money on underage game developers and taking a lion's share from their earnings).
This puts it in the same place as many other apps (including Discord)
where the company might decide to ruin the platform at some point.

Moving onto the app itself though;
Guilded works a bit differently than most of the apps listed here.
What Discord calls servers are called groups in Guilded,
and Guilded servers can have multiple groups.
It's like another layer of organisation above Discord's servers.
To avoid confusion, I will be using Guilded's terminology for the rest of this segment.

I'm not sure I fully understand Guilded's business model,
but there seems to be no premium features;
instead, users can buy subscriptions for servers,
which grants them roles and other per-server benefits (e.g. channel access)
which are configurable by the server owner.
Guilded earns money by taking a fee from those subs.
You can also buy a subscription (Guilded Gold) to fund development
and get access to beta features early.

Also worth nothing is that similarly to Discord,
[Guilded sells anonymised user data](https://support.guilded.gg/hc/en-us/articles/360039235054-Privacy).

The features I mentioned above include:
* Pretty fun customization (e.g. using gradients in roles intead of plain colors)
* Advanced channel types:
  * Streaming (video calls with screen sharing)
  * Voice channels; these are further organised into rooms,
  for an overall feel similar to TeamSpeak
  * Calendar channels for events
  * Scheduling channels (users can mark their availability over time)
  * Announcement channels
  * Forums
  * To-do lists
  * Docs (wiki-like stuff)
  * Media (this works kinda like social media, where people can comment and react on the media you post)
* Configurable bots; while there's no public API for programmers at the moment,
Guilded allows you to create bots from the GUI using a set of triggers and actions the bot can take in response.

Overview:
* Voice chat: yes
* Screen sharing: yes
* Multichannel support: yes
* Custom emoji: yes, unlimited per server.
I'm not sure these can be used across servers,
but can probably be used across groups in a server.
* Self-hosting: no
* Pricing: free
* Other: has a decent phone app

### Revolt chat

![(A screenshot of Revolt)](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fdl.flathub.org%2Frepo%2Fscreenshots%2Fchat.revolt.RevoltDesktop-stable%2F1504x846%2Fchat.revolt.RevoltDesktop-e70e44718034af84ddbd1f89375bb4cd.png&f=1&nofb=1&ipt=6ae14e269eb92b8ee6b1e67e16f3a52e0175bb7dc49cdb4978b31eb3eb2d00a1&ipo=images)

I've been putting this one off because it gets pretty crazy.

On the surface, [Revolt](https://revolt.chat/) is a drop-in replacement for Discord that's open source and abides by GPDR!
Upon further inspection though, questionable things start popping up.

I saw some rather concerning comments about the developer team, drama,
whether the app is really open source and about the self-hosting under [this article](https://itsfoss.com/revolt/).
I take them with a grain of salt, as they seem to come from griefers,
but they did set off a red flag in my head.

[This doc](https://wiki.revolt.chat/en/transparency/inquiries/2023-09-10-rebolt)
is linked in the comments, and is a somewhat tangible proof of drama going on around Revolt.

There's no information about self-hosting on their website,
although after some searching it can be found as [a Docker deployment](https://github.com/revoltchat/self-hosted).
Unlike the Synapse Matrix server, it has clear instructions on how to deploy it.
At the same time I found comments on 
[Reddit](https://www.reddit.com/r/revoltchat/comments/q0sjit/can_i_host_my_own_server_yet_or_is_there_just_one/
)
saying they couldn't get it to work.

Another big issue is that Revolt is not federated.
Adding federation support [is not on the roadmap for the developers](https://developers.revolt.chat/faq/federation).
Hosting your own Revolt instance requires users to register a separate account on it
and they have no access to other instances with it.
This creates an even bigger push for centralisation than with Element;
while Revolt's privacy policy seems good at a glance,
I'm not sure what to think of it in the light what I also found in the [FAQ](https://developers.revolt.chat/faq/federation):

> The Revolt team currently consists mostly of students (18-20 years old),
and the majority of the project organisation and work is being done by one person (Insert).

That's really damn impressive,
but at the same time leaves me worried for the longevity of the project.

One annoyance that I found was the lack of a feature list on the Revolt website,
or in the developer docs.

Lastly, glancing at the r/revoltchat subreddit
reveals that the app has a lot of technical issues,
hinting that it's still pretty early in development.

There's some good news on the monetization side though:
> We have a variety of monetisation ideas lined up internally, with these, it is not my intention for us to paywall features and I find it unlikely we would ever do that considering it would contradict what we're trying to achieve.

* Voice chat: yes, but unfinished
* Screen sharing: couldn't find any mentions of it, and definitely not even on the horizon considering the above
* Multichannel support: yes
* Custom emoji: yes
* Self-hosting: yes, but Revolt is not federated; [users will have to register a new account on your instance](https://www.reddit.com/r/revoltchat/comments/18g69gr/i_have_a_few_questions_about_selfhosting_a_revolt/)
and won't be able to interact with other Revolt instances.
* Pricing: fully free and intending to remain that way
* Other: End-to-end encryption, message pinning not implemented yet; entire GUI is customizable

I really hope this project succeeds
and learning about it made me appreciate the insane amount of work that goes into making such an app;
however, I'm not entirely sure how usable it is at the moment.

### Spacebar chat

Previously known as Fosscord,
[Spacebar](https://spacebar.chat/) is a free and open source Discord clone that's compatible with existing Discord bots.

It is still early in development and not really in a usable state,
but is posing up to be an interesting option.
In fact it's so eary in development that I could not find a screnshot of the app,
although the website offers a login form.
My first impression of it was better than of Revolt,
as it's very transparent about what it is and isn't.

* Voice chat: eventually
* Screen sharing: not for the foreseeable future
* Multichannel support: yes
* Custom emoji: yes
* Self-hosting: yes, although it is unclear whether it's federated or not
* Pricing: fully free and intending to remain that way


---
## Conclusions

I tried to concentrate on facts so far, so here's how I feel about
the apps I find suitable to replace Discord in some capacity.

**Revolt** - on the surface it's great and its GDPR compliance gives me hope.
On the other, the lack of documentation for potential users
gave me a major ick and the app is just not very mature yet.
The lack of planning for instance interoperability / federation is concerning.
I still haven't fully made up my mind about Revolt and will be watching its development.

**Guilded** - on one hand, its features are so cool that I want to jump to it right now.
On the other, I'd be doing so with resignation about future-proofing and privacy.
Considering its accessibility and features, it is the most likely
app to be adapted by regular users (i.e. non-techies) though.

**TeamSpeak** - Maybe it's the easy self-hosting,
the pretty nice "feel" or the long-standing reputation,
but something about this app makes me pretty partial to it.
The lack of proper text channels beyond group chats is a massive shame,
and still no support for video calls doesn't help either.
If not for those, I'd be picking TS as the successor to Discord.

Honorable mentions:
* Telegram - offers much better privacy than Guilded,
but when it comes to future-proofing and ownership it is on par with Guilded,
which in turn offers way better features.
I'm also not sure how to feel about its somewhat shady background
and not a fan of the design based on mobile app principles.
* Steam chat - my current backup for contact with online friends,
but due to its simplicity it will likely stay just a back-up.
* Mattermost - would have won my heart if not for the paywalling of group voice calls.
I'd be willing to even pay for it, but the pricing is ridiculous for a casual user.
It is a good but sad reminder of why a FOSS option is the way to go.
* Rocket chat - overall a good fit but for some reason I don't feel it.
It deploys with Docker and I'm not sure how accessible the install process is.
Besides, as with Mattermost it's subject to licensing restrictions that can change at a whim
(which is weird for a supposedly FOSS project).

Now, to finish of this gargantuan post.

As [this great post](https://www.reddit.com/r/discordapp/comments/t204t4/for_those_suggesting_guilded_revolt_signal_or/)
on Reddit points out, the fundamental issue with apps like Revolt, Guilded and so on
is that they are not based on an open protocol;
the moment they do something unpopular, you're looking for an alternative once again.

In light of that, the idealist in me says that **Element/Matrix** is the future.
The issue is however, that its development has been concentrating on enterprise support,
giving no love to the casual users (ekhm custom emojis nowhere in sight ekhm).
My attempts at starting a server did not give me a good first impression,
and joining an existing instance can be risky as I've mentioned before.
I really want Element to be the winner, but considering all of the above,
I will sadly not be jumping to Matrix anytime soon.

This leaves me trying to pick between Revolt, Guilded, TeamSpeak and Telegram.

I *sooo* want to pick TeamSpeak.
The option of hassle-free self-hosting
that lets people use other servers is the best way of doing self-hosting
for casual users in my opinion,
and one that sadly is not offered by any other app.
However, TeamSpeak lacks two features which are **way** too big to gloss over.
I have to leave it for the unlikely scenario that
I will need a separate voice call app because of our main communicator
not offering a good enough service.

Telegram is tempting because of its decent privacy,
but I don't think I can get over the Fisher-Price feel it has
(notably, Element is not much better in this regard).

This leaves us with the unfair match between Guilded and Revolt.
A fully dependent solution made by a large company who sells your data
vs an open project with focus on privacy,
but one in the early stages of development and made by a group of students.
Both are rather accessible too.
Unfortunately the lack of video conferencing is a major holdback with Revolt.
It puts the app into the same category as Element,
where I'd prefer to use it but it's kinda not ready yet.

That leaves us with Guilded;
the obvious winner that fits like a glove feature-wise,
but in terms of my goals is no different from Discord.
If Discord disappeared today,
Guilded would be the most likely to replace it when it comes to the wider userbase.

As it stands though, Discord is here to stay,
and I won't be trying to convince my friends to
jump to Element, TeamSpeak or Revolt until one of these apps catches up with its feature offering.
