---
title: Open teaching with R Markdown and GitHub
author: Rick Gilmore
date: '2015-10-09'
slug: open-teaching-with-r-markdown-and-github
categories:
  - teaching
tags:
  - open science
  - GitHub
  - R Markdown
  - R
---

In keeping with my effort to move my research toward more open and reproducible practices, I decided to build all of my lecture slides in RMarkdown using [RStudio](https://www.rstudio.com/), make my syllabus and assignments in Markdown, and generate exams and quizzes using LaTex and its [Exam](https://www.ctan.org/pkg/exam?lang=en) class. The lecture slide workflow involves several steps:

1. Making slides in RStudio.
2. Exporting them to HTML.
3. Editing the syllabus file to add links to the HTML, RMarkdown, and sometimes PDF versions of the slides.
4. Committing the revisions to my local git repo and then pushing to the GitHub repos for each class.

I have existing slides in Keynote, PDF, and sometimes PowerPoint that I use to make my new slides. 

The workflow has many advantages and a few disadvantages. I'll talk about the advantages today, and the disadvantages in a future post. Version control is one advantage. It's easy to catch a mistake and fix it right away, or revert should I need to do that. Markdown also makes it easy to make text-based bullets. It's also (mostly) easy to incorporate materials from the web directly into my talk. So, if I want to embed a YouTube video like this one <https://www.youtube.com/watch?v=Te7e37XMtP0>, I click on `share`, then `embed` and then copy and paste the HTML in the box. In this case, YouTube makes it easy for me because the code specifies an `<iframe>` that makes the video appear as a separate window within my lecture slide. 

I particularly like the fact that I can link a separate, [BibTex](http://www.bibtex.org)-formatted, bibliography file, and have RStudio make nicely formatted in-text/slide citations and a references list at the end of my lecture slides. I can even make the in-text/slide reference a clickable hot link to the actual paper. Say that my bibliography file contains an entry to a fine paper like this:

    @article{raudies_visual_2014,
    title = {Visual {Motion} {Priors} {Differ} for {Infants} and {Mothers}},
    volume = {26},
    issn = {0899-7667},
    url = {http://dx.doi.org/10.1162/NECO_a_00645},
    doi = {10.1162/NECO_a_00645},
    number = {11},
    urldate = {2015-01-29},
    journal = {Neural Computation},
    author = {Raudies, Florian and Gilmore, Rick O.},
    month = nov,
    year = {2014},
    pages = {2652--2668}}

Then, by entering this bit of Markdown code -- `[[@raudies_visual_2014]](http://dx.doi.org/10.1162/NECO_a_00645)` -- my slide will have a clickable link directly to the paper after RMarkdown renders the HTML.

Another advantage is that I can embed figures, either by storing them locally or by linking to a figure on the web. I find that it's better to use HTML's `<img>` tag for both purposes rather than Markdown's `![fig-label](path-to-fig)` syntax. When this works, it's really, really slick. I can link to an image on the web, say the one at <https://nyu.databrary.org/party/308/avatar?size=56>. With this bit of code `<img src="https://nyu.databrary.org/party/308/avatar?size=56">` the figure appears in my talk like so:

<img src="https://nyu.databrary.org/party/308/avatar?size=56">

Next time I'll complain about how finding valid image URLs that resolve properly can be a challenge. But, for now, I'm touting advantages, among them are the fact that I can find and remember where I've stored images I like. In the past, I've been inconsistent about copying and pasting to my photo library metadata about the source URL from an image. It's also great not to have to manage a large number of images on my local machine. 

A final virtue of this approach is that GitHub's embedded Markdown (and RMarkdown) rendering features means that my simple course sites are easy to set-up and maintain and pretty easy to use, even for novices. Penn State is undergoing a transition in its course management system software, so I like having the flexibility to roll my own. Plus, I like the fact that my students can grab materials about our course from any web-enabled device. Of course, I had to figure out how to use the <http://rawgit.com> service to render raw HTML stored on GitHub.

I find myself wanting to add more and more links, especially to the sources of particular claims. This only opens up the scholarship involved in my field and makes the knowledge we've fought hard to accumulate more transparent. It also makes it easier for students to follow along in the footsteps of others. 

Thanks to [Christopher Gandrud](https://github.com/christophergandrud), the author of *[Reproducible Research with R and RStudio](https://www.crcpress.com/Reproducible-Research-with-R-and-R-Studio/Gandrud/9781466572843)* for the inspiration to try all of this in the first place.

If you're curious, check out the sites and let me know what you think:

- [PSYCH 260/BBH 203](https://github.com/psu-psychology/psych-260/blob/master/syllabus.md)
- [PSY 511](https://github.com/psu-psychology/psy-511-scan-fdns/blob/master/syllabus.md)

