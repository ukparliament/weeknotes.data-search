## Week 12: 13-10-2017

### Dator day

Data day #33 happened. The room was... bijou. The planning with the website team session was constructive. Much, much better than last time. Really much better.

Chris from business systems came along for the first time. [Dan](https://twitter.com/dasbarrett) came to grudgingly accept [it's not like the old days anymore](https://www.youtube.com/watch?v=8BJvVV-fnls). Robert tried handwriting. Michael came [dressed as his granddad](https://www.google.co.uk/search?q=clegg+last+of+the+summer+wine&source=lnms&tbm=isch&sa=X&ved=0ahUKEwio76K2v-3WAhVH1RoKHeUlDBoQ_AUICigB&biw=1252&bih=764).

We agreed we'll:

* Focus technical work on stable identifiers to make it easier for other people to work with our data and open up [beta.parliament.uk](https://beta.parliament.uk/) to search crawlers.

* Provide assistance to Angela with the interim data source for committees.

* Provide assistance to [Ben](https://twitter.com/benwoodhams) with Lords' inflation (don't ask).

* Do whatever data and search work is required around Northern Ireland postcodes and constituencies.

* Continue to work on government roles. Which seems to be going well on all sides.

* Continue to investigate sources of division data.

* Help to break down the oral contribution stories.

### Showing and telling

Tuesday, as ever, was show and tell day. [Samu](https://twitter.com/langsamu) gave an overview of the fixed query API improvements (the bits of the API that drive the beta website). [Raphael](https://twitter.com/raphaelleung) presented on machine learning before heading off for his [GDS](https://gds.blog.gov.uk/) data science accelerator graduation. General applause, Raphael.

Wednesday was the all staff briefing. [Dia](https://twitter.com/DN78) talked through the Data and Search 101 presentation. Which was very clear and seemed to go down well.

### One world, one web, one team

[Matt](https://twitter.com/mattrayner), the backend lead for the website team, gave a talk about the architecture of the [beta.parliament.uk](https://beta.parliament.uk) [Rails](https://en.wikipedia.org/wiki/Ruby_on_Rails) application. Most of the data and search team went along to find out how our data becomes web pages.

Dan gave [Jamie](https://twitter.com/oddtype) and [Jeanette](https://twitter.com/clementgraphics) moral support at the digital portfolio board where they presented work on the new website. Dan had a cameo with a live demo of current website search. Jeanette helpfully drove the tabs.

Dan went to one website stand up this week, and a backlog review session. [Aidan](https://twitter.com/aidan_morgan) definitely went to more than one stand up. [Michael](https://twitter.com/fantasticlife) thinks he went to one but, much like the Sundays, [can't be sure](https://www.youtube.com/watch?v=yARVs1ZNLjU).

### Domain modelling

[Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver) and Michael spent Tuesday turning last week's [Written Questions and Answers domain model](https://github.com/ukparliament/domain-models/blob/master/Written%20questions/written-questions.pdf) into a [first pass data model](https://ukparliament.github.io/ontologies/written-question-and-answer/written-question-and-answer-ontology.html). They spent some time with Sally Carter, the House of Lords gatekeeper for written answers, and the proposed model seemed to make sense. It's quite different from how things work at the moment but would have the advantages of saving effort, reducing errors, having fewer documents and more linky data, and making a better, more linky website. Time will tell.

Anya and Michael met with Ben, [Colin](https://twitter.com/colinpattinson) and [Ed](https://twitter.com/ewhitur) to prioritise which bits of the domain model they should be working on next. The results are in the [Doing, Doing next and To do columns on Trello](https://trello.com/b/Z1nrm0Vr/parliament-ontology).

### Data quality

[Chris](https://twitter.com/chrisalcockdev) has been working on a Lords' inflation tool (still don't ask) for Ben. It started life as a massively over engineered Sharepoint / Access odyssey and ended up as a single page spreadsheet.

Michael spent some time with Angela running through the Red Book database and trying to document it. Red Book is the system used by the House of Commons to manage Select Committee data. From work so far it looks to be a similar shape to the Committee Office Database (a similar system used in the House of Lords) with evidence sessions belonging to zero or one inquiries and inquiries belonging to zero or one committees. More work is needed. 

### Data platform

Work to import and publish data about government roles (departments, positions and incumbencies) is now complete.

The Member photo import to the data platform has been deployed and is now running.

### Search

The search product team had their first retrospective and planning for sprint 5. [Caroline](https://twitter.com/carolinekippler) helped out. The team went through the backlog and agreed on the prioritised items.

To anticipate possible new search features, work has been done to categorise Parliamentary material published on the web by inferring attributes from the huge variety of inconsistently structured URLs. The work is generally referred to as search hints. [Raphael](https://twitter.com/raphaelleung) has continued the work initiated by Samu and has been adding regular expression rules to capture currently indexed Parliamentary sites. At time of writing there are over 1,000 rules. Exclamation mark here.

Raphael took Dia through search hints. Dia was happy and impressed.

Robert, Samu and Raphael also met to chat about the progress on search hints. All is on target. Robert met with Liz in preparation for analysis on search once the beta is officially included in the public index. Robert also met with Lopa to hear more about “webmaster” things and beta preparation.

Robert and Colin met to chat about Members and search. A pleasant time was had.

### Measuring things

[Matias](https://twitter.com/matiasgermanico) started to explore the JIRA API with the goal of building reports from the data. So far it's going good, except for the fact it has a maximum result set limitation. Work continues.

Sara and Liz met with Elise from the House of Commons Library to talk about some research she is doing using the European survey on political attitudes. She's interested in finding groups of people based on their attitudes. They discussed approaches to analysis, gave her a few pointers that are hopefully helpful, and chatted about how she might test and verify findings using a different year's survey results.

Aidan, Liz, Dia, Jamie, Trine and Lopa met to discuss tools and next steps in establishing the ability to run A/B tests for search.

Sara began setting up the analysis for A/B testing the display of document URLs in the search results page. This involves creating the measures we want to track and defining baselines to compare to the test results.

### Machines that do learning

Back in September, Jianhan submitted evidence to the House of Lords [Select Committee on Artificial Intelligence](http://www.parliament.uk/ai-committee). All the written evidence is [now published](http://www.parliament.uk/business/committees/committees-a-z/lords-select/ai-committee/publications/). Jianhan's contribution [is here](http://data.parliament.uk/writtenevidence/committeeevidence.svc/evidencedocument/artificial-intelligence-committee/artificial-intelligence/written/69472.html).

[Phil](https://twitter.com/philbgorman) from the Indexing and Data Management Section of the House of Commons Library went with Raphael to the GDS accelerator graduation / wrap-up event. He's planning to pass on notes to the data science people in the library. Raphael thought his presentation went okay. He's writing a PDS blog post and there'll be a GDS blog post in a few months to see where the projects ended up. 

Angela from the website development team has been accepted on to the next data accelerator. 

### Capability

Robert and Dan had a chat about using the GDS digital academy as part of Julie’s capability work. Both training and recruitment were covered.

### Aidan's truly terrible week

Aidan had a truly terrible week. There's no way to make this sound fun so:

* various procurement activities (software licences, events, courses, purchase orders, invoices)

* chasing up hardware orders

* trying to get an ADSL line for the team

* talking to Programmes and Projects Office (or is it Projects and Programmes?) about risks and benefits of the various streams of Data and Search and continued work on business cases

* assisting with preparations for Search Product Team retrospectives and sprint planning

### Did anybody say blockchain?

Colin said blockchain. But jokingly. So that's fine.

### Things that caught our eye

* [Deeply Interwingled Laws](https://blog.law.cornell.edu/voxpop/2017/10/06/deeply-intertwingled-laws)

* [Bootstrapping (statistics)](https://en.wikipedia.org/wiki/Bootstrapping_%28statistics%29)

* [Models of collaborative tagging](https://en.wikipedia.org/wiki/Models_of_collaborative_tagging)

* [Why Isn’t Agile Working?](https://hackernoon.com/why-isnt-agile-working-d7127af1c552?source=linkShare-4cd140afefc2-1507885727)

* [Rapid rise and decay in petition signing](https://epjdatascience.springeropen.com/articles/10.1140/epjds/s13688-017-0116-6)

* [Three very different sources of bias in AI, and how to fix them](https://joanna-bryson.blogspot.co.uk/2017/07/three-very-different-sources-of-bias-in.html)

* [Data is not the new oil](http://www.bbc.co.uk/news/entertainment-arts-41559076)


