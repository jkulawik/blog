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

{% include csv-table.html data=site.data.chat-apps %}

Tooltip example

*[Tooltip]: This is a tooltip

* VC
: Voice chat / video chat
* Multichannel
: Whether chatrooms are grouped and managed together, or the app is based on separate group chats, like in a phone app or in IRC.