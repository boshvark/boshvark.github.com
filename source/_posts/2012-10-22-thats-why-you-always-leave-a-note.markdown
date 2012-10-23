---
layout: post
title: "That's why you always leave a note"
date: 2012-10-22 23:50
comments: true
categories: programming
---
One of the nicest things you can do as a programmer is to leave detailed notes
for the future programmers who must maintain your code. Especially since the
most likely maintainer of your code is you.

If you've done anything complicated or non-obvious, leave an explanation of
what you did and _why you did it_. If your implementation is incomplete or
suboptimal, leave a detailed note about what should be done next. This is not
a substitute for actual communication with members of your team, but it makes
things so much nicer for the next person who touches the code.

I've gotten in the habit of leaving myself a note whenever I need to stop what
I'm doing, even if I only expect the interruption to last a few minutes. (When
does that ever happen?) Sometimes the note is just a short sentence about what
I was doing. Two nights ago, at 2am before going to bed, I left the following
paragraph in the code.

{% codeblock I am so thoughtful. lang:cpp %}
    START HERE --- (not here in the code really ...)
    // I just finished updating this to work with the new QuizEngine API.
    // Things are not compiling, so get them compiling again with all the
    // QuizEngine changes.
    // Also, make sure we can load from an Anagrams quiz database, and that
    // the QuizForm is calling the correct code to update the database as the
    // quiz progresses.
    // Later, update things to work with Anagrams With Hooks, Hooks, and (oh
    // god help us) Word List Recall.
    // Oh, and rip out all the XML saving code too.
    // Oh yeah, and don't forget to save Search Spec to the quiz database. And
    // probably some other thing I'm forgetting, like ... well, I forgot. Oh
    // yeah, Source or whatever the Cardbox Ready thing is called.
{% endcodeblock %}

Today as I jumped back into the code, my present self thanked my 2am self for
being so thoughtful. Obviously I was not fully coherent, but I was able to
dump the contents of my brain before powering down. This saved me a lot of
time I otherwise would have spent figuring out what the heck I was doing.

One thing to note about this comment: it doesn't compile. I consistently use
the all-caps phrase "START HERE", and I usually put it outside a comment. The
next time I try to compile, big red errors will force me to read my note.
Whenever you can easily force yourself to do the right thing, do it.

And that's why you always leave a note.
