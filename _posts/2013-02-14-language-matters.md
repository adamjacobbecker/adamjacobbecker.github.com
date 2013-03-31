---
layout: post
title: Language matters
abstract: >
  I am wholly of the belief that programmers shouldn't define themselves by the language they code in. Not only is one's choice of language far less important than their ability to write clear, concise, and structured code, but I also can't see how anybody could avoid writing code in all but the language they prefer. For me, working on civic technology, it's pretty much a necessity that I can contribute to projects of different languages, not to mention working across the stack from backend to front.
---

I am wholly of the belief that programmers shouldn't define themselves by the language they code in. Not only is one's choice of language far less important than their ability to write clear, concise, and structured code, but I also can't see how anybody could avoid writing code in all but the language they prefer. For me, working on civic technology, it's pretty much a necessity that I can contribute to projects of different languages, not to mention working across the stack from backend to front.

But for someone who's arguing that the language doesn't really matter, I'm still going to propose that **choosing the right programming language can go as far as to make or break your project.**

And it's not the fact that forcing programmers to use curly braces around method declarations is going to drive them to insanity. No, it's that certain languages give you access to much better tools. Much, much better tools. Like giving a chainsaw to a person trying to cut down a tree with a breadknife. That much better.

When we got our team together for RFP-EZ, we had an little internal debate about which language we would use. I had been writing PHP for years, but I  had just fallen in love with the Ruby world a few months earlier and wanted to go the typical Rails route. My teammates were convinced (and quite possibly, rightly so) that deploying a Rails app would be too difficult to do with government hardware, and that we should just stick to the tried-and-true PHP. In the end these requirements prevailed, and we wrote the app in PHP using the new Laravel framework, but the months that followed were frustrating. I found myself searching hopelessly for features and libraries that existed in Ruby but not in PHP. I found myself spending hours writing features that shipped free with Rails, or could be accomplished with a great RubyGem. Things like building serializers for use in APIs, or simply *rendering a form correctly and easily*. The kicker? Testing libraries for PHP pale in comparison to their Ruby counterparts.

I think a lot of this can be attributed to the fact that Ruby is a flexible language, one that lends itself well to mocking and stubbing and monkey patching, but just as important is that the group of smart folks writing great tools in Ruby vastly outnumbers those writing tools in PHP. I guess my point is the same as my answer to Clay's initial interview question of "why do you like Ruby so much more than other languages?", which is that the community around the language is truly remarkable.

In our discussions, the number we threw around regarding "just how long it would take for us to navigate deploying a Rails app inside government" was 2 weeks, but I'd say that the time we lost by writing our app in PHP was at least double that. I had to write my own classes to do fragment caching. Jed and I spent entire days trying to properly set up testing libraries and asset management pipelines.[^1] For a language that has been around for 18 years, PHP is seriously lacking great tools for modern web development. And when the tools do exist, it takes hours to cobble them together in a working manner.

When choosing the technology stack for your next project, try to not let antiquated requirements affect your decision. There's a reason that web development is so much more awesome now than it was 10 years ago, and if you decide to use different tools than the ones you prefer, chances are that you'll pay for it later.

[^1]: *I'm aware that choosing a more mature PHP framework could have provided some of these things, but there are still tons that just don't exist.*