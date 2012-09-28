---
layout: post
title: Open Source Software and the US Federal Government
---

Earlier this month, the White House released the source code powering its "We The People" website, a platform that allows citizens to petition The White House on issues ranging from "Greater Protections for Same-Sex Couples" to "Ale to the Chief: White House Beer Recipe". While it wasn't the first open-sourced project from inside the federal government, it was an important milestone, being the first repo online at github.com/**whitehouse**.

On the heels of [whitehouse/petition](https://github.com/WhiteHouse/petition) came [whitehouse/wh-app-ios](https://github.com/WhiteHouse/wh-app-ios) and [whitehouse/wh-app-android](https://github.com/WhiteHouse/wh-app-android), the source code for the White House's mobile apps. Even cooler was when www.wh.gov/developers went live, on it the quote, *"We believe in using and contributing back to open source software as a way of making it easier for the government to share data, improve tools and services, and return value to taxpayers."* It's far from the time to declare victory, but how *awesome* is it that someone in the Executive Office of the President wrote that sentence? Of course, the real work is to make this a trend that spreads across all of the federal agencies, and not just the current hotness being touted by the White House.

So I'm hoping that the recent work we've been doing as part of the [Presidential Innovation Fellowship](http://wh.gov/innovationfellows) can serve as a step in the right direction. We made the decision when we first formed our team that we'd be developing RFP-EZ [publicly on GitHub](https://github.com/presidential-innovation-fellows/rfpez), but I think that in the past 2 months we've gone even further, breaking up our project into multiple, smaller modules, each of which is immensely more valuable to the open-source community than RFP-EZ would be as a whole.

In fact, here's a list of some open-source projects that have come from our work in just the past 2 months:

1. [SOW Composer](https://github.com/presidential-innovation-fellows/sowcomposer) - Templatizes the process of writing Statements of Work. The templates live in the repo, so this can be used for virtually anything that warrants a SOW. We've already got two major cities that are deploying their own instances of SOW Composer, which is a super-rare and awesome example of collaboration across different levels of government.

- [FormTimer](https://github.com/presidential-innovation-fellows/FormTimer) - FormTimer records how long your forms take to fill out, and sends that information to a node server and/or Google Analytics. There's this thing called the [Paperwork Reduction Act](http://www.archives.gov/federal-register/laws/paperwork-reduction/) that makes this a vital tool for government websites, but why the heck wouldn't you use it on your site too?

- [USAxGITHUB](https://github.com/adamjacobbecker/USAxGITHUB) - A simple page for viewing the US Federal Government's open-source activity, which uses YQL to make calls to the GitHub API. This can be used to aggregate any number of github organizations' activity onto one dashboard.

- [github-sentences](https://github.com/adamjacobbecker/github-sentences) - Converts the GitHub Events API to human-readable sentences. Used in USAxGITHUB.

- [jquery-birdseye](https://github.com/adamjacobbecker/jquery-birdseye) - My personal favorite, a plugin for moving-map search, like on Yelp or Airbnb, built with jQuery and Leaflet.

- [mongoose-api-query](https://github.com/adamjacobbecker/mongoose-api-query) - A plugin for creating a complex search API with Node and MongooseJS.

So there you have it, 6 open-source projects in 2 months, and the best part was that it barely took any extra effort on our part. Sure, we may have spent a couple days refactoring and writing READMEs, but the benefits of modularization are totally worth it. With any hope, this can start to become the norm, and in the coming years you'll see more and more official US Government accounts and repositories online. Heck, you're the ones paying our salaries, so it would only be fair.

For more reading:

- [The White House's Digital Government Strategy](http://www.whitehouse.gov/digitalgov)
- [Dashboard of the US Government's entire activity on GitHub](http://ada.mbecker.cc/USAxGITHUB)
