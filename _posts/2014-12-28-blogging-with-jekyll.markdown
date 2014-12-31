---
layout: post
title:  "Blogging with Jekyll and GitHub Pages"
date:   2014-12-28 12:10:01
categories: tech whisk
tags: [tech, whisk, crdt, scala]
---

I've never really caught the blogging bug. Mostly, this is because of friction, which may seem odd - surely it's just writing? Well, no. It's blogging engines, customisation, installing plugins, themes, etc. Hopefully, all that is changing.

I spend a sizeable proportion of my time documenting designs and plans, and my tool of choice for this is [Markdown][markdown]. I love Markdown with all my heart, and wish it were more widely supported in Regular People's Tools: mostly Google Docs and Word. Still, many blogging engines support Markdown, so I cannot claim it as friction - at least not directly.

I spend almost all of my time in or accompanied by [Sublime Text][sublime-text]. I love Sublime Text with all my heart: it's fast, powerful, and behaves predictably for me as I switch projects, syntaxes, and paradigms. I know Sublime very, very well, and if I'm writing a blog, I want to write it in Sublime. Since many blog engines are hosted, that's not always an option.

Much of my time - and indeed much of my mental effort - concerns *programming*.  At [Whisk][whisk], I work on both back-end code in [scala][scala] and front-end code in [AngularJS][angular-js] and Javascript - well, [Coffeescript][coffeescript], at least. If you spend this long thinking about these things, inevitably you will also want to write blog posts about them. Native, high-quality support for code examples is a paramount concern for me when blogging. Again, this exists elsewhere, but I did say "native".

Drafting and publishing blog posts has also been a source of friction for me. Most of my code and design work is kept in some form of shared, cloud-based document storage. In particular, at Whisk, we use [git][git]: our closed-source product code resides in [Bitbucket][bitbucket]; our open-source code lives in [GitHub][github-whisk]. I host [my own code][github-junglebarry] on GitHub, too. I love git, and am fond of both Bitbucket and GitHub. At Whisk, we've built infrastructure around git for continuous integration and deployment, such that git provides a natural mechanism for drafting and publishing code. It makes perfect sense that this mechanism should translate equally well to blog posts.

The final piece of friction for me is hosting. I have installed Wordpress and hated it. I hate all the business about setting up servers, databases, plugins, etc. just for a *blog*. I have used hosted blogging engines and hated them, too. Mostly that's because of theme rigidity and web-based editing. I want something where there is almost no setup, and I can start writing content quickly.

The solution to my problems is widely known, but was recommended to me by [Dave Gurnell][dave-gurnell] and [Noel Welsh][noel-welsh] of [Underscore][underscore], during my recent trip to [Scala eXchange][scala-exchange]. So far, I think it's a perfect fit. What's more, it took about an hour to get everything up and running - plus the obligatory four hours faffing with colours to recreate my [Cobalt Sublime Text theme][cobalt].

My blogging engine is [Jekyll][jekyll], which is a hosting engine for static content. I can write posts in Markdown, and Jekyll offers excellent support for code embedding and syntax highlighting.

Even better, Jekyll has been anointed for use with [GitHub Pages][github-pages], which means I get the full GitHub toolchain for hosting, plus [Jekyll][github-jekyll] support for drafting and publishing posts. This fits my workflow very nicely indeed. The hosting is also free (although I'd be quite happy to pay for this).

As a consequence, I shut down my long-dormant hosting account at [Lunarpages][lunarpages], which left me a little sad: Lunarpages have been nothing short of superb over the ten years I've used their services and support. However, it does free me up to use one of my favourite services, [CloudFlare][cloudflare], for DNS and site management. I'm familiar (and happy!) with CloudFlare as it has served us very well at Whisk. It's a doddle to use - even for something simple like blog DNS - and offers much more atop for more complex web applications.

In short, I'm now writing a blog in my favourite editor, in my favourite syntax for writing, and my hosting arrangements are those I use day-to-day for drafting, publishing, and deploying code. I can no longer complain about friction... I guess I'll have to think up some new excuses for my sporadic blogging output.

[markdown]:           http://daringfireball.net/projects/markdown/syntax
[sublime-text]:       http://www.sublimetext.com/
[whisk]:              https://whisk.com/
[scala]:              http://www.scala-lang.org/
[angular-js]:         https://angularjs.org/
[coffeescript]:       http://coffeescript.org/
[git]:                http://git-scm.com/
[bitbucket]:          https://bitbucket.org/foodient
[github-whisk]:       https://github.com/whisklabs/
[github-junglebarry]: https://github.com/junglebarry/
[dave-gurnell]:       http://davegurnell.com/
[noel-welsh]:         http://noelwelsh.com/
[underscore]:         http://underscore.io/
[scala-exchange]:     https://skillsmatter.com/conferences/1948-scala-exchange-2014
[jekyll]:             http://jekyllrb.com/
[github-pages]:       https://pages.github.com/
[github-jekyll]:      https://help.github.com/articles/using-jekyll-with-pages/
[lunarpages]:         http://www.lunarpages.com/
[cloudflare]:         https://www.cloudflare.com/
[cobalt]:             http://colorsublime.com/theme/Cobalt