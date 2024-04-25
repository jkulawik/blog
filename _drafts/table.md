---
layout: post
title:  "Table"
tags: []
---
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa

{% highlight python %}
def bubble_sort(items):
    """ Implementation of bubble sort """
    for i in range(len(items)):
        for j in range(len(items)-1-i):
            if items[j] > items[j+1]:
                # Swap!
                items[j], items[j+1] = items[j+1], items[j]
{% endhighlight %}

```
code test
```

`inline code`


|App             |Group VC    |Multichannel|Custom emoji|Networking   |Pricing |FOSS|Normie design|
|----------------|------------|------------|------------|-------------|--------|----|-------------|
|Telegram        |yes         |yes         |yes         |centralized  |free    |no  |yes          |
|Mattermost      |paid feature|yes         |yes         |decentralized|freemium|no  |no           |


{% include csv-table.html data=site.data.chat-apps %}


*[VC]: Voice chat / video chat
*[Multichannel]: Whether chatrooms are grouped and managed together, or the app is based on separate group chats, like in a phone app or in IRC.
*[Normie design]: Many apps have the annoying interface style with huge profile pictures and chatroom icons, and speech bubbles in chats.
*[Networking]: Whether the app is centralized, decentralized, or decentralized and federated.
*[FOSS]: Free and open-source
