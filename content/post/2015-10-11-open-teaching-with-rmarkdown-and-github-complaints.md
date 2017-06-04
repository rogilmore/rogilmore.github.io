---
title: Open teaching with RMarkdown and GitHub -- Complaints
author: Rick Gilmore
date: '2015-10-11'
slug: open-teaching-with-rmarkdown-and-github-complaints
categories:
  - teaching
tags:
  - open science
  - GitHub
  - R Markdown
  - R
---

In my last post, I sketched out my workflow for using [RStudio's](https://www.rstudio.com/) RMarkdown package to make HTML-based slides that I serve via GitHub and the [RawGit](http://rawgit.com) service. I'm still a fan, but there is trouble in paradise. Or, I should say that it's not yet paradise. So, in this post, I'll describe some of my complaints. My mom always used to chide me "if you don't have something nice to say, don't talk." So, I'm hoping she reads the first post and skips this one.

The biggest challenge is that many of the papers I'd like to link to are behind pay walls. So, if I decide to link directly to a journal article that supports some particular claim, I'm never sure whether the article will actually load in the browser. Penn State has agreements with most of the major publishers I want to link to. So, as a faculty member I'm usually able to view an online version of a particular paper if I access it directly or via a link from [Google Scholar](http://scholar.google.com). I know that to show me a given article, there's a whole lot of communication going on behind the scenes that's usually hidden from my view. What this means though is that if I put a URL inside an HTML `<iframe>`  or a direct Markdown-formatted link like `<http://www.nature.com>`, there's a better than even chance the resource won't load in my slide. That's true even when I am presenting from a machine that is securely authenticated to the PSU wifi service. So, to borrow a phrase, it should "just work", but it doesn't.

The failure to load problem is especially acute if I try to link directly to a data figure. I used to take screen shots of data figures, but that turns out to be a huge file management hassle. I'd rather link directly to the source. But, it's not straightforward to do so. Finding a figure's URL is not always easy although I've gotten pretty good at it. Some journals, however, don't actually serve articles with images and text as separate HTML resources. That means I can't link directly to a figure at all. 

In my humble opinion, **all** figures, tables, the reference list, and data from a published source should have distinct, unique URIs. Even better, I would like journals to take a page out of YouTube's book and provide HTML that can be cut and pasted into a document. This would embed the resource right in the document. Better still would be incorporating something that Wikipedia offers on some images -- HTML code that both links to a figure and provides human-readable citation text. Imagine being able to right click and have HTML code like that copied right to your clipboard. 

I'd paste that into an RMarkdown document, and think I'd gone to open science heaven. Or something.
