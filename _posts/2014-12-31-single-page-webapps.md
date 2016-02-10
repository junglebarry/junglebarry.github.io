---
layout: post
date: 2014-12-31 16:35:54
title: "Why I like AngularJS"
categories: tech web
tags: [tech, web, javascript, spa, angularjs]
---

This year at [Whisk][whisk], we've been leaning heavily on AngularJS - an [extremely popular][octoverse] framework for developing Single Page (web) Applications, or SPAs for short. I've watched our team make giant leaps with AngularJS, and some of those leaps are due to the framework itself, but others are due to the SPA paradigm. In this post, I'll discuss why AngularJS is proving to be a  game-changer for web development.

AngularJS is a powerful and - as many have opined - complicated framework for building web applications. It can be used to build pure Single Page (web) Applications (SPAs), and this is the context in which I use it. However, AngularJS can also be coupled with a more traditional server-side HTML framework, like [Play][play-angular] or Rails, where much of the HTML is generated server-side, then augmented by AngularJS on the client. I have little experience with the latter use-case for AngularJS, and will be somewhat biased in my discussion towards the SPA context.

AngularJS is a pure Javascript web framework. However, like many other frameworks, it provides the following concepts:

* View and controller separation
* URL structures and routing
* HTML templating
* data binding, between underlying Javascript models and HTML

Being a Single Page Application framework, it reframes this familiarity for client-side development:

* Native client-side HTML template manipulation
* Native support for JSON data

I'll discuss why these attributes make development easier, with reference to my historical perspective, and why the SPA approach make sense now.

## Out with the old

Back in days of yore, I spent a lot of time writing applications in server-side web frameworks. For context, when I started doing this, I was concerned about whether my code was going to work acceptably in Internet Explorer 6, and IE7 seemed like the promised land. We developers wanted to build interactive web applications with dynamically updating content, unconstrained by the boundaries of "the page".

In this model, server-side code (mine was written in Racket) generates the HTML forming the entire HTML page. This page is transmitted to the client (browser), and the "dynamism" was achieved by applying Javascript code to the rendered HTML. 

These were not merely different languages, but different ways of thinking. Coding within this context is *slow*, because the programmer is perpetually changing mode from server-side to client-side. Reasonable tools (e.g. jQuery) were available for each mode, but there was a boundary between them - the rendered HTML page - and that boundary was a source of perpetual pain.

## In with the new

Single Page Applications offer us a different boundary. Since SPAs are written Javascript, they have native support for JSON, so can operate directly on the output of JSON web-services.

In a single-page AngularJS application, it's natural to use JSON as a data model. What's more, Angular makes it easy to transparently use JSON API responses as model data. With this new capability, we no longer need to make a fully-rendered HTML page the boundary between server and client.

SPAs let us redefine the boundary between server and client. In a single-page AngularJS application, it's natural to use JSON as a data model. What's more, Angular makes it easy to transparently use JSON API responses as model data. 




For me, there have been two big factors that have led us away from server-side HTML with AJAX. First, native mobile applications - with their own programming languages and user interface toolkits - arrived

Second, and as a response to native mobile 

The first was the advent of native mobile applications - predominantly targetting iOS or Android. While native mobile platforms support HTML, they also have their own UI toolkits. Many native apps prefer communicating in raw data, HTML. The world fell in love with the JSON web-service, and rightly so. JSON+HTTP became a de facto standard for mobile apps, but webapps were still stuck in the old AJAX mentality. 

Native mobile apps set a much higher expectation with users, and web technology had to make significant gains to remain competitive. The second factor, 

The paradigm shift for SPAs is to provide a capable client offer is to move away from transmitting ready-rendered HTML (as AJAX) and towards sending data.

For me, the big changes that Single Page Applications offered 



 

## The business case for AngularJS

Well, this one is easy: AngularJS applications are extremely fast to develop, once you know what you are doing. The reasons for this are straightforward:

* The application is concerned with rendering



A couple of factors contribute to 
, once you know what you are doing. Moreover, the pattern of programming 

First,

### Dealing with JSON; or: forms no more

One 

## Directives


## Dependency Injection


## Two-way data binding


## What's wrong with AngularJS

In short, it is simply too complicated. The learning curve is famously steep, and even once you've learned and applied most of the lessons, you still find yourself engaged in a dance with circular dependencies or the digest cycle.

The prototypical example is the difference between providers, services, and factories. These are variations 



The SPA pattern is certainly not for every application.

AngularJS is certainly not for every application - 

[whisk]:         https://whisk.com
[octoverse]:     https://octoverse.github.com/
[play-angular]:  https://typesafe.com/activator/template/modern-web-template
[ng-directives]: https://docs.angularjs.org/guide/directive
[html-form]:     http://www.w3.org/TR/html401/interact/forms.html#form-data-set