---
title: Multi-lingual, after a fashion
author: Rick Gilmore
date: '2015-07-22'
slug: multi-lingual-after-a-fashion
categories:
  - teaching
tags:
  - open science
  - GitHub
  - R Markdown
  - R
---

I'm giving a talk at the [International Conference on Development and Learning/Epigenetic Robotics](http://www.icdl-epirob.org/) meeting in Providence in a few weeks. The talk offered me the chance to put into practice some of the software tools I've been trying to master. The goal was to create a presentation that used open source software components, version control, and included the actual code used to generate as many of the figures as possible. You can see the talk draft at <http://gilmore-lab.github.io/ICDL-EpiRob-2015>. Yes, it is in HTML, and thus can be viewed just like any other web page. That was the goal. How I got there is a story of many languages.

I use [R](http://www.r-project.org/) for my statistical analyses, and I have become particularly fond of the [RStudio](https://www.rstudio.com/) environment. RStudio supports a set of tools that enable a researcher to write a data analysis report in a text file. The text file includes headers and subheaders, comments about the ongoing data analyses, executable R code and even links to external images or web pages. The text file is in a scripting language called [R Markdown](http://rmarkdown.rstudio.com/). [Markdown](http://daringfireball.net/projects/markdown/) is simple mark-up language that has gotten popular recently. R Markdown is RStudio's implementation of it. I'm writing this blog post in Markdown, as it happens. To make a set of slides, I used the [ioslides](http://rmarkdown.rstudio.com/ioslides_presentation_format.html) output option. This allows me to write code like the following:

    ## Slide 1 Header
    * First bullet
    * Second bullet
    
    <img src="http://www.opp.psu.edu/planning-construction/projects/nittany-lion-shrine/pre-work-site/nittanylion.jpg/image"/>
    
    Now, I want to add two numbers.

    ```{r}
    # This is some R code to add two numbers. Woo-hoo!
    x <- 2
    y <- 3
    z <- x + y
    ```
    ## Slide 2 Header

The text inside the three back-ticks is R code. The part that starts with `<img src=` is [HTML](https://en.wikipedia.org/wiki/HTML). The nice thing about a text file like this is that I can use a version control system to keep track of my edits. If I try some hare-brained thing that doesn't work -- and this happens surprisingly often -- I can roll-back the clock and undo my mistake. I use the [Git](http://git-scm.com/) version control system. Git requires me to issue commands like `git add new-file.Rmd` to tell git to keep track of a file and `git push origin master` to update my shared software repository on the web. I use [GitHub](http://github.com/gilmore-lab) for this purpose. 

So, I edit my R Markdown file, then have RStudio turn that file into an HTML file that can be viewed on the web. Then, if I like the new version of the talk, I ask git to "commit" or save this version along with a message that reminds me what changed in this version from the last. Then, I push the revised version to GitHub, both for safe-keeping, and so that my collaborators can keep up with what I'm doing.

Finally, if I want to make the talk itself available on the web, I ask GitHub to turn my HTML file into a web page. The great part is that I can store the [code and data that generated my whole talk](https://github.com/gilmore-lab/ICDL-EpiRob-2015/tree/master) AND the resulting human-friendly [web-page](http://gilmore-lab.github.io/ICDL-EpiRob-2015/#1), in the same place. That way if I forget how or why I did something, or one of my collaborators really likes a particular figure but wants it to be tweaked, or I want to share my hard-earned knowledge with someone else, I'm good to go. Everything I did to make the talk is there. It's a huge savings of time. Plus, it fosters the spirit of open sharing that is a big part of other aspects of my professional life like [Databrary](http://databrary.org).

The downside to all of this is that I've had to acquire a working knowledge of several different mark-up and scripting languages: R, R Markdown, HTML, CSS, Unix, git, and yaml. Yes, some of these I haven't described in this post. I've also had to learn how to navigate GitHub. I enjoy this, but not everyone does. And, because the learning curve is so steep, the joys -- and they are real joys -- and benefits are unlikely to be shared that widely. Yet. I think that will change in the near future. In the meantime, I'm consoling myself that I am multi-lingual after a fashion, as long as the entity at the other end of the line is a computer.
