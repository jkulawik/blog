---
layout: post
title:  "C++ kinda sucks"
# subtitle:  "A thinly-veiled love letter to Golang"
tags: [programming]
---

C was my first programming language. And then C++.
After a brief encounter with Java, I've mostly programmed in Python for several years.

For a while I believed that starting with Python was a better idea,
but I've come to accept that it was a ridiculous one and that C and C++ are indeed the best place to start.

Having learned Golang (a language which combines the power of C++ and has a developer experience that bests even Python)
and now working on some corporate C++ projects with large codebases behind them,
I can't help but wince at the many pitfalls of C++ that go way beyond [its famous memory leaks](https://www.tomshardware.com/software/security-software/white-house-urges-developers-to-avoid-c-and-c-use-memory-safe-programming-languages).

## Syntax

One of my core principles with engineering is making things intuitive wherever possible.
[Keep it stupidly simple](https://en.wikipedia.org/wiki/KISS_principle), if you will; I believe those principles should be applied to most things in existence, including language syntax.

Which is why I find C++ syntax rather annoying.

range loops
{} brackets
brackets around if statement
&& || instead of and or
semicolons for each statement
streams; the `>>` syntax is kinda an eyesore. I don't get why we need separate operators for this instead of a flexible function.
In fact, custom operators, while really powerful, can be also very evil.

Honorable mention although it's not really syntax: allowing assignments in if statements,
i.e. debugging your code for 3 hours before realizing you wrote `if(i = 0)` instead of `if(i == 0)`.

Lowercase vs mixed case; typing and reading speed

While I dislike Python's dynamic typing (and other quirks, like no visible difference between declaring a variable and writing to it),
it figured out the most human-readable syntax I've ever seen.

*Sidenote: You can probably imagine that I'm not enthusiastic about trying Rust.*

To further exacerbate this issue, C++ has less consistency with code style than any other language.

## Formatting style

In what is a prime example of [bikeshedding](http://catb.org/jargon/html/B/bikeshedding.html),
each time you work in a group on a project which uses a language with no set style guides,
people will flinch at their differing styles of formatting.

To name a few particularly annoying ones:
* Spaces (or lack thereof) around various statements
* Naming conventions and mixing them (e.g. `PascalCase` usually used in projects while the standard library uses `snake_case`)
* Breaking statements into multiple lines
* Placement of opening brackets:

{% highlight cpp %}
void function(){
    return;
}
// vs.
void function()
{
    return;
}
{% endhighlight %}

* Hungarian notation and its derivatives.
I get where it comes from; you don't always see what type something is and where it comes from.
But working with `lptstrThing` is not easy on the eyes (something that C++ already sucks at).
If I see a `float afTimeStep` in a function declaration, do I really need a prefix telling me it's a float argument?
Why prefix object classes with a `C` when usually it's pretty obvious that it's an object?
These get particularly bad when they start mixing. E.g. `cLuxMap *apMap`.
It just makes things needlessly confusing when a descriptive name would suffice.

While C++ is by far not the only language with this issue,
it is probably the one that gathered the biggest number of differing and mixing styles.
Diving into a new codebase is usually a pain already, but re-learning to read C++ makes it so much worse.

And then on top of that you get macros!

## Macros

One of those ideas that seems great on paper and if you ignore the impact on how the language users write code.

To cite another comment I saw online;

> With macros, every C++ project becomes its own programming language.

Need I say more?

## Dependencies

The usage of specific header files instead of some kind of a module/packaging system
makes it pretty annoying to acquire all necessary dependencies.
If you don't know where a header file comes from (which is typically the case),
good luck finding it.

## Linking and compiling

Full disclosure: I am too lazy to learn how to properly link C++ code.

However, at a time in which essentially every major programming language handles imports for you,
should I really need to get a PhD in linking C++ to compile my code?
Perhaps this complexity offers some amazing power in some department I'm not aware of,
but to me this is an antiquated part of the language that adds tons of annoying overhead for businesses and hobbyists alike.

Many C++ build systems have been created to address this issue,
but I keep seeing C++ engineers say they're mostly crap and you should stick to Makefiles.
Regardless, fighting the linker is the last thing I want to be doing when I have an assignment to finish.

When it comes to compilation proper, the amount of spam that comes out of the compiler is terrible.
Showing each class and variable namespace and C++ version (akin to `std::__cpp11::string`)
and the same info messages 20 times makes makes troubleshooting a nightmare.

## Conclusion

