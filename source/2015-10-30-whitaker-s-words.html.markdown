---
title: Whitaker's Words
date: 2015-10-30 16:56 PDT
tags:
---

Well, I haven't been posting here much (or at all) have I? Well, I'll start now. Maybe. But I am writing here now anyway. [Whitaker's Words](http://lysy2.archives.nd.edu/words.htm) is an interesting old command line program for analyzing the morphological form of latin words, as well as providing simple definitions. For example, here is what it outputs for the word "caesaris":

> caesar.is            N      3 1 GEN S M  
> Caesar, Caesaris  N (3rd) M   [XLXBO]  
> Caesar; (Julian gens cognomen); (adopted by emperors); [C. Julius ~ => Emperor]  
> *

So, it tells us that it is a noun, third declension, in the singular genitive, with a short definition and a couple other things. This likely is rather uninteresting if you have no interest in Latin, but if you do, it can be quite a useful tool.

I noticed that, though there is an android app called Whitaker's Words, it is not really the same thing. It uses the dictionary from words, but does not do the morphological analysis, which is the main point. For dictionaries, there are better options. So I (not right now, but in September) wrote an Android app that wraps the actual words program, providing all of the functionality. Compiling was a little complicated, since it was written in ada. Naturally the Android NDK only supports C and C++, and I can't really seem to find a cross compiler for ada targeting ARM processors. I ended up using an arm chroot with qemu and building it there, after failing at attempts to build a cross compiler, but eventually got a usable binary. After that wrapping the program was fairly simple, since it is a command line tool and, though interactive, can also just be used by passing words as arguments.

You can find the result on [Google Play](https://play.google.com/store/apps/details?id=com.ids1024.whitakerswords) with the [source code](https://github.com/ids1024/whitakers-words-android) available on Github. Hopefully people will find it useful, which does seem to be the case based on the five star ratings it has gotten. It is free, open source, ad-free and requires no permissions, because when these are not the case it annoys me (excluding permissions when they are clearly needed, of course) so I would be a hypocrite to do otherwise.

Well, that is all I have to say for now. Stay tuned for another post tomorrow, the next day, or in a millennium or two!
