---
title: Devilish details
author: ""
date: '2019-04-24'
categories: [open science, ethics, data sharing, pre-registration]
---

I've found myself at odds recently with colleagues who, like me, view themselves as advocates for open science.
This post attempts to clarify what I see as the crux of our disagreements.

## We don't own our data

Most researchers feel a strong sense of ownership about our data and often, properly so I think, feel especially protective of our research participants.
The fact remains, however, that despite our essential role in determining what data get collected from whom and how, we researchers have the weakest claim to actually *owning* the data we collect.

In the U.S., if my work is funded by a grant from the Federal government (e.g., NSF or NIH), then that award is actually made to *my institution*, not me.
In fact, if I am unable to fulfill the obligations of the award, my institution may, and often will, appoint another person to do so.
If my work is funded by another source, that source is likely to have implemented similar provisions.
So, in reality, while researchers have a primary stewardship role over research data, it likely belongs to our institution.

In other contexts, the EU, for example, strong arguments have been made that *research participants* actually own their data.
I am sympathetic to these arguments and believe that empowering individuals to grant researchers specific permission to use their data is the best path toward a future of ethical data use.
Implementing that vision at-scale poses substantial challenges I believe academic researchers can eventually meet.
The point of convergence is that researchers don't own the data we collect.

Not owning the data nevertheless means that we researchers must still think carefully about how best to protect it, our participants, and our institutions.
As a practical matter, even though our institutions (or research participants) may own the data, we are the ones best positioned to determine what happens to those data when our project ends.
In other words, the responsibility for determining the future life, if any, of our research data is one we can't meaningfully shirk or easily ignore.
At the same time, because the data aren't really ours,  considerations about any personal or career risk associated with sharing data can't be at the center of the discussion.
Instead, our obligations to research participants, our institutions, and funding agencies must take precedence.
This means that fear of being scooped probably isn't sufficient justification to withhold sharing data.

## Sharing data publicly without restriction is unnecessary and poses unforseen risks

I believe that some of my colleagues who are skeptical about data sharing understand the practice to mean sharing data in publicly accessible ways.
These skeptics argue that they don't have permission to share data that way, and thus doing so would violate research ethics.
I agree.

In fact, I go further.
I am worried that we woefully underestimate the risks of participant reidentifiability associated with combining public and private data sets, even when research data have been stripped of conventional identifiers.
Imagine if Bernie Sanders and Donald Trump had taken intro psych classes and the 'deidentified' data were publicly available to anyone today.
Doesn't it seem likely, certain even, that large well-funded teams of data scientists would be scouring the internet in order to try to expose Bernie's answer to this survey question or Donald's score on that cognitive test?

We can't predict the future, but we can try to shape it.

Rather than make open, public sharing of data about human beings the expected norm, I suggest we build on an existing track-record of sharing these sorts data with restricted audiences.
The Inter-university Consortium on Political and Social Research ([ICSPR](https://icpsr.umich.edu)) at the University of Michigan has been storing and sharing data with restricted audiences for almost 60 years.
The U.S. Census has developed procedures for allowing restricted access to individual Census survey responses in highly secure and protected environments.
The [Databrary](https://databrary.org) data library that I co-founded and co-direct has created a data library for openly sharing video and audio recordings with a restricted community of researchers.
There are numerous examples of data sets shared by the U.S. government (e.g., NDAR) that have various restrictions on who can access data and for what purposes.

These examples illustrate that open data sharing need not be synonymous with public data sharing.
The ICPSR and Census examples especially show that even the most sensitive data can be successfully shared with responsible researchers.

Yes, restricted sharing with researchers affiliated with institutions of higher learning or academic medical centers is 'elitist' to some degree.
But the checks and balances these institutions provide -- research ethics training, research review committees, research supervision, secure data storage infrastructure -- protect research participants in ways that public data sharing schemes simply cannot, at least not now.
I think this form of elitism is justified in the name of protecting research participants.
Or at the very least, that restricting data about human participants should be the norm unless and until we can be highly confident that public sharing truly poses minimal risk. 

Thus, I conclude the following:

- Virtually all data about human research participants can be shared in some form.
- The standard for sharing data about human research participants should be to use a data repository that restricts access to specific individuals for purposes subject to external review.
- All researchers who collect data about human research participants should be collecting permission to share information from their participants so that any data sharing activities are in accord with participants' wishes. There are readily available [templates](https://www.databrary.org/resources/templates.html) researchers can adapt for seeking sharing permission. Going forward there is no reason for 'failure to secure permission to share' to be a meaningful impediment.

Now, some may argue that the cost of securing permission to share and storing data in restricted repositories versus publicly accessible places must be weighed against the benefits.
I don't disagree that costs and benefits must be weighed, but it is often hard to weigh them objectively.
Instead, I think it is safer to say that we have a longer history of and familiarity with restricted data sharing and more information about the costs of preparing data to share in these sorts of settings.
So the surer bet in the long-term is to build on what has already been working.
The risks of widespread public data sharing are a 'known-unknown', in Donald Rumsfeld's categorical scheme, while the risks of restricted data sharing are 'known-knowns'.
I do not share Mr. Rumsfeld's politics, but I find his thinking incisive and useful  in this context.

One final point in favor of restricted sharing in centralized repositories is metadata standardization.
If we view data sharing as an investment in future scholarship, then sharing data in standard ways that others can combine, reuse, and build upon is essential.
By design (e.g., Databrary, government-sponsored data repositories) or long-standing practice (ICSPSR), data repositories provide standard metadata elements that make data more readily discoverable and reusable.
Of course, curating data to meet these metadata standards takes time, but the payoff comes in accelerated resuse and discovery.

So, data about human participants should be shared (with permission) in data repositories that restrict access and support standardized metadata, and all of us who do research with human participants should be seeking explicit permission to share in these ways.

## Sharing data, materials, and analysis scripts is more important to open science than pre-registration

I greatly admire the efforts of the team at the [Center for Open Science](https://cos.io) in bringing preregistration and registered reports into widespread scientific discussion and making them a much more common practice.
There is no question that drawing clearer, brighter lines between confirmatory and exploratory analyses improves the quality of scientific inference and mitigates questionable research practices.

That said, I get the biggest and hardest push-back from colleagues about preregistration when discussing open science practices.
One reason is that many people find the process of pregistration difficult, frustrating, and onerous.
Yes, there are lots of templates to choose from, and yes, many of the details are already in our IRB protocols or grant proposals.
But even so, the benefits of pre-registration seem small relative to the high costs, especially to skeptics.

For these reasons, and innate pragmatism, I spend more of my energy talking-up data sharing.
Data are more interesting to me personally and probably more useful in evaluating the impact and importance of a given piece of work than a detailed preregistration plan.
One of my graduate school mentors told me that he reads a paper's methods and results first, and only after that decides whether to read the introduction and conclusion.
Frankly, if the data aren't interesting or the effects clear, I don't care that much what the authors predicted or how they tortured the data.
And by extension, if the effect is strong, it's unlikely to matter much whether the authors predicted it or not.
Further, I've found no convincing retort to the skeptics who ask me why I think someone actually followed their preregistered procedure.
In short, I think that most studies on human participants are under-powered and that we need to vastly increase the quantity of shared data in order to address problems of estimating true effect size distributions.
While I may not really know whether a researcher followed the protocol reported in a manuscript or in their preregistration, I can evaluate the size of the reported effect and hopefully combine it with other datasets...if the data are shared.
When push comes to shove, I'd rather authors commit to open data sharing and carry through on their commitments than encourage people to preregister but have them stop short of sharing.

So, while I'm completely happy endorsing the virtues of preregistration, I'm going to keep asking authors of papers I review, most of which are not preregistered, to share their data.
That's because I think data, materials, and analysis code sharing is ultimately more important to advancing discovery than preregistration.
And 'learn more faster' is not only Databrary's tagline, is my personal motivation for adopting open science practices.
That ultimate goal can get lost in the sometimes devilish discussions about specific details.
