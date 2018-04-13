## 2018 Week 14

### On visions and strategy and things related

[Dan](https://twitter.com/dasbarrett)'s week was mainly spent writing a first draft of the data strategy to be presented at next week's Data Steering Group.

In related strategy news [Anya](https://twitter.com/bitten_), [Samu](https://twitter.com/langsamu) and [Aidan](https://twitter.com/aidan_morgan) met to discuss the vision and strategy for the 'Data Toolkit and Vocabulary Management' work. Aidan will update the draft documents and be setting up a session to discuss in more detail.

With the assistance from Raphael, [Jianhan](https://twitter.com/jianhanzhu) and [Chris](https://twitter.com/chrisalcockdev), Aidan has been putting together a synopsis of the interim data sources currently in place and under development. This will form a part of the document Dan's writing.

### Showing. And indeed telling

Chris, Raphael, [Michael](https://twitter.com/fantasticlife) and Samu gave a joint show and tell about the work they've been doing on the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html), the [application they've developed](https://procedures.azurewebsites.net/) for the general purposes of tire kicking and some of the ways they've begun to visualise procedural and other data.

Some of the procedural clerks from both Houses turned up and the discussion that followed (about decoupling the data platform from business facing application development) was probably more interesting than the showing. Or the telling.

Previous weeknotes have pointed to Raphael's work on [2D visualisations of procedural data](https://procedures.azurewebsites.net/WorkPackages/5/graph) but they're starting to look really good now.

Samu made a [three.js](https://threejs.org/) [visualiser for graph data](https://api.parliament.uk/viewer/) and Chris added a few more features. [CORS](https://en.wikipedia.org/wiki/Cross-origin_resource_sharing) permitting, you can make a 3D visualisation of any [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework) graph on the web, something that we're unaware exists in such an accessible way anywhere else. [This is the OWL ontology visualised](https://api.parliament.uk/viewer/#https://www.w3.org/2002/07/owl). You can remove type statements to [make things more legible](https://api.parliament.uk/viewer/?notype#https://www.w3.org/2002/07/owl).

They work best if you have a very large touch screen and an ambition to be a less weird Tom Cruise.

A while back one of our colleagues from another department (name redacted) said that all the Data and Search team do is make flow charts. That isn’t even remotely true, but when we do make flow charts they are interactive and three-dimensional. So there.

### Community

Aidan met with [De Havilland](https://www1.dehavilland.co.uk/) who currently scrape Parliament's website (and those of other Parliaments and institutions) for data. They talked about the new platform, public APIs, upcoming work and long term goals. De Havilland are interested in starting to use our APIs and in joining our community events.

### One world, one web, one team

Michael spent some time with [Jamie](https://twitter.com/oddtype) and the Members website product team looking at proposed designs for written [questions and answers](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) and chatting about URLs. The only thing of any concern was identifying the position of the answering minister at the time of the response. Which given the state of our government positions data could be tricky.

On a similar note there was a brief email exchange with the [GDS](https://gds.blog.gov.uk/) [Regsiters](https://registers.cloudapps.digital/) team to discuss the need for a register of government positions (and incumbencies (and people)). Please someone make this and make it go backwards.

Samu met Callum to discuss the technical details of introducing [Research Briefings](https://researchbriefings.parliament.uk/) onto the [beta website](https://beta.parliament.uk).

### Domain modelling

The second cross-team design session for [Statutory Instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) took up a fair chunk of Tuesday. There were some good discussions about the timing of scheduled Business Systems development work and the need for a new procedure to deal with [proposed (aka baby) SIs](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e240). We also spent some time doing a collaborative review of the design mock-ups created by the SI Website product team against the [domain model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html).

Anya and Michael published a first draft of a very basic [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html). Like everything else, it will probably need to grow over time, but they think it gives us everything we need for immediate SI work. Anya still needs to check how Parliament currently handles [coming into force dates](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e88) and [coming into force notes](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e103), so those comments are still subject to change.

### Data platform

Wojciech made some tentative first steps toward [standardised documentation and machine readable specifications](https://www.openapis.org/) for our services on api.parliament.uk.

Matthieu dived deep into [SPARQL](https://en.wikipedia.org/wiki/SPARQL), hunting down a bug related to binding the existence of alternative property paths to a variable. The issue has been reported, now we're waiting for a fix. He duck taped an alternative path in the data for the time being, whilst marvelling at the flexibility of both SPARQL and RDF.

Matthieu's also asked for fixes to the HTTPS remote repository support in [VocBench](http://vocbench.uniroma2.it/). [Armando](https://twitter.com/starred75), the project lead was very prompt to answer and the matter is being investigated. Suspense is hitting peak levels everywhere.

Since it looks like a vendor special for Matthieu this week, he complied a wishlist, some of which you may want to support:
 
 * [Increase the size limitation of backups](https://feedback.azure.com/forums/169385-web-apps/suggestions/10036335-increase-the-size-limitation-of-backups-from-10gb)
 
 * [Even larger App Service plans](https://feedback.azure.com/forums/169385-web-apps/suggestions/33226270-xl-app-service-plans-we-need-to-scale-up)
 
 * [Support SPARQL in Cosmos DB](https://feedback.azure.com/forums/263030-azure-cosmos-db/suggestions/6738428-support-for-w3c-sparql-as-a-query-language)

### Search (and indeed indexing)

Liz tinkered with some data and made visualisations around search terms and concepts from our [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri). For now it's all quite basic. Just for fun, she made some graphs showing top terms used by class type. Which is interesting but not useful (she says).

Sara wrote a [R](https://www.r-project.org/) script that outputs all [concepts](https://ukparliament.github.io/ontologies/concept/concept-ontology.html#d4e316) used by the Indexing and Data Management Section in the House of Commons Library in the past month.

### Corporate data

In David's week the interface with the facilities management system is now working. Final testing on the interface to link people to their department(s) is scheduled to go live at the end of next week.

Lewis continued with development work on the House of Lords HR system integration.

[Matt](https://twitter.com/matiasgermanico)'s work on the Active Directory integration is now ready for testing. This will pick up data directly from AD and will provide updated phone number and network ID information to People Data. On the corporate reporting front, Matt has started linking sources from external spreadsheets to a single spreadsheet. Once it's updated it will hold all of the data in one place. So far he's linked 6 KPIs.

An integration for the online learning system was modified by Matt and some offline testing was done.
 
Noel is testing the finance side that handles transactions from the House of Commons Library. He's also provided assistance with Parliament's Financial Times and Times online email database list.

### Capability

Liz and Matthieu did a technical interview with the candidates for our vacant Data Analyst position. Dan and [Julie](https://twitter.com/julietouring) handled the panel interview part. Both bits went well.

### On not breaking the web

Dan asked team:Samu to revive the blog on our previous open linked data platform, which had stopped working sometime recently. Samu implemented a solution to redirect all requests to the old blog to the [Internet Archive Wayback Machine](http://archive.org/web/). He also reviewed related cloud infrastructure to identify resources that are not needed any more. Mike deployed the solution and Wojciech turned off the unnecessary computing resources. Money and electricity were saved.

Samu met [Chris Fryer](https://twitter.com/c_fryer) to discuss the recent [Historic Hansard](https://api.parliament.uk/historic-hansard/index.html) migration, the assorted problems it caused and how we could prevent similar problems in the future. They discussed why things like the migration are difficult to communicate in such a large organisation and how similar difficulties with other services might be prevented if there was [less focus on process and more on people actually talking to each other](http://agilemanifesto.org/).

Chris and Samu also discussed the potential for longer term cooperation, like the Data Service using Archive systems as a data source and the Archive adopting identifiers from the Data Service.

### Is it possible to get promoted?

Yes. Apparently it is.

### Did anybody get promoted?

Let's not get carried away here.

### Was sarcasm deployed?

You've got the wrong people, sunshine.

### Things that caught our eye

* [Mapping Mutations in Legislation: A Bioinformatics Approach](https://academic.oup.com/pa/advance-article/doi/10.1093/pa/gsy006/4883355?guestAccessKey=b9e4fc1e-995c-47e8-8fd5-de1c380b25bf)

* [ONS Integrated Data Conference](https://www.eventbrite.co.uk/e/integrated-data-conference-2018-tickets-43741014552)

* [An Interactive Visualization of Every Line in Hamilton](https://pudding.cool/2017/03/hamilton/)

* [The Write Stuff: how we used AI to help us handle correspondence](https://dftdigital.blog.gov.uk/2018/04/09/the-write-stuff-how-we-used-ai-to-help-us-handle-correspondence/)

* [Government by numbers: how data is damaging our public services](https://apolitical.co/solution_article/government-numbers-data-damaging-public-services/)