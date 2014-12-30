---
layout: post
title:  "Talk: Shopping around with CRDTs at Whisk"
date:   2014-12-29 11:44:54
categories: tech whisk
---

I recently gave a talk at [Scala eXchange][scala-exchange], entitled "Shopping around with CRDTs at Whisk". In the talk, I describe how we use [Conflict-free Replicated Data Types][crdt-wiki] to power the [Whisk][whisk] shopping list apps. The talk is intended as a practical introduction to CRDTs for a general developer audience.

In the talk, I cover:

* Offline and data synchronisation for mobile and web applications;
* The problems associated with data sync - concurrency;
* CRDTs - eventually consistent data-structures that avoid concurrency problems;
* How we use CRDTs at Whisk, behind an API that powers our mobile and web applications. 

It's couched in terms of Whisk's domain: (grocery) shopping lists, but that should be familiar enough to most people.

There's a screencast available [here][talk-skillscast]; the slides are available [here][talk-slides]. 

I'll revisit the topic in more detail in a series of blogposts in the near future. I'll also be following up on some of my feelings on Scala eXchange as an event (spoiler: I greatly enjoyed it).

[whisk]:           https://whisk.com
[crdt-wiki]:       http://en.wikipedia.org/wiki/Conflict-free_replicated_data_type
[scala-exchange]:  https://skillsmatter.com/conferences/1948-scala-exchange-2014
[talk-skillscast]: https://skillsmatter.com/skillscasts/5838-shopping-around-with-crdts-at-whisk
[talk-slides]:     http://www.slideshare.net/junglebarry/shopping-around-with-crdts-at-whisk