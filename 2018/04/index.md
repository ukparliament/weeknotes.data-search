## 2018 Week 04

### Community

[Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) went along to a Data Stories workshop organised by [the ODI](https://theodi.org/). It was lovely as ever to see our [Tony](https://twitter.com/psychemedia) and delightful to bump into [Jeni](https://twitter.com/jenit). After a few presentations and a short tour of [some artworks](http://culture.theodi.org/vending-machine/), they emerged blinking into tepid sunlight feeling none the wiser.

[Raphael](https://twitter.com/RaphaelLeung) went along to an [event](https://www.statslife.org.uk/events/eventdetail/1065/-/what-is-a-data-scientist-s-responsibility-to-wider-society) at the [ONS](https://www.ons.gov.uk/) on data science and ethics, which he enjoyed greatly.

### Corpcomms

Someone put words into Yammer. I know this because an email told me.

### One world, one web, one team

[Dan](https://twitter.com/dasbarrett), perhaps unsurprisingly, went to some meetings.

There was one about the process of commissioning business systems for Commons 'procedural' areas which saw a demo of the new Historic Hansard which is due to be integrated into [current Hansard](https://hansard.parliament.uk/) at some point in the not too distant future. Until then, [Historic Hansard]((http://hansard.millbanksystems.com/)) remains in its usual place. There was also talk about business systems work on [Statutory Instruments (SIs)](http://www.parliament.uk/business/bills-and-legislation/secondary-legislation/statutory-instruments/) and committees.

Dan also went to the website product roadmap meeting. He met with [Aidan](https://twitter.com/aidan_morgan), [Dan](https://twitter.com/DigitalDanCook) (portfolio manager) and [Rebecca](https://twitter.com/rebeccaelton1) (Director of Portfolio) and talked about the big corporate data plans and data strategy that he has to make happen. Somehow.

Bryony and [Victor](https://twitter.com/_victorhwang) popped by to see Anya, [Silver](https://twitter.com/silveroliver), Michael and [Ben](https://twitter.com/benwoodhams) and talk about how the [question and answer model](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) might translate into question and answer pages. It felt like they got somewhere.

### Domain modelling

Anya, Silver, Michael and Ben ploughed on with the SI modelling work. They drew out a [process flow document](https://github.com/ukparliament/domain-models/blob/master/SIs/flow.pdf), which is possibly the 200th time someone has attempted this. It's still probably wrong and definitely missing some House of Commons stuff. But they're encouraged that it has very few component types. That said, so does DNA...

Matthieu popped by in the morning to chat about plans to migrate the Indexing and Data Management Section (IDMS) [taxonomy](http://www.data.parliament.uk/dataset/thesauri) to the new data platform. The plan so far is to use [SKOS](https://www.w3.org/2004/02/skos/) to handle concepts and their relationships. But the transitive nature of [skos:broader](https://www.w3.org/TR/2005/WD-swbp-skos-core-spec-20051102/#broader) and [skos:narrower](https://www.w3.org/TR/2005/WD-swbp-skos-core-spec-20051102/#narrower) present problems. There was a good conversation about the nature of broader and narrower in taxonomies and some push back on the idea that they were designed to capture any kind of real-world ontological truthiness. It's boxes in boxes on shelves. That's fine. More chats are needed but Michael finally feels he has his finger on something roughly like the problem.

### Data platform

[Jianhan](https://twitter.com/jianhanzhu)'s [post](https://pds.blog.parliament.uk/2018/01/24/accessing-semantic-data-with-odata-web-interface/) on our new [OData](http://www.odata.org/) service continued to do good business.

There was an [encouraging tweet](https://twitter.com/ldodds/status/956182855398428672) from [Leigh](https://twitter.com/ldodds) who knows much about such things.

Our Tony chipped in with [some mild trolling](https://twitter.com/psychemedia/status/956222458016788480) which lead to a useful back and forth with Jianhan. Jianhan attempted some 'excellent customer service' but in the end we had to conclude that OData just isn't Tony's cup of tea. Something a little more gonzo will be required here.

Jianhan tends to agree that the client side tools for OData are still not very strong. In his view, the best client side library is [the C# one](http://odata.github.io/) but support elsewhere may be lacking.

That said, Tony did make some progress using a Python OData library. His progress so far is, as ever, [on Github](https://gist.github.com/psychemedia/d41abc807c753df2908fe0019674731c).

Staying with OData, Sara has been exploring ways of using [regular expressions](https://en.wikipedia.org/wiki/Regular_expression) and the OData service for search term grouping. We could, for instance, use the OData interface to query the triple store and retrieve Members' names. The list of Members' names could then used to create a regex rule for the group 'MPs'.

For those with an interest in committees we're delighted to announce that Chris has now added [formal body chairs](https://ukparliament.github.io/ontologies/formal-body-affiliation/formal-body-affiliation-ontology.html#d4e47). At least to the staging database.

Also in committee related work, almost all the things that the Members' Names Information Service (MNIS) calls 'Departments' are now in the staging triple store. It's a bit of a fuzzy set of actual departments, other government organisations and some parliamentary offices. We've typed all of these as [groups](https://ukparliament.github.io/ontologies/agency/agency-ontology.html#d4e391), with any that are found on the [Register of Government Organisations](https://government-organisation.register.gov.uk/) typed as GovernmentOrganisations. The stuff from the 'Departments' table that isn't actually a group has been excluded, by a new approach to orchestration based on exclusion.  MNIS considers 'Leader of the Liberal Democrats' to be a 'Department' for reasons that are unclear to us. Using an exclusion list allows us orchestrate data live from imperfect sources.

Raphael revisited a project looking to suggest topics to IDMS. He also implemented a package explaining classifiers.

### Search

Dan spent some time playing with [search on the new shop](https://www.shop.parliament.uk/search?q=whisky), which isn't 'one true search'. He thought it interesting how much better 'one true search' is if you're looking for whisky shot glasses but spell it whiskey or scotch. We feel there are opportunities here for the future. Though what kind of philistine would drink whiskey from a shot glass escapes us.

Dan, [Jamie](https://twitter.com/oddtype) and [Samu](https://twitter.com/langsamu) also did some footling around with the new website search. Footling may be strong here.

### Measuring things

Liz met with Tom from the Chamber and Committees team. They want to explore relationships between evidence submitters across committees and what social media can help them understand about influence and targeting communications. It sounded good. She encouraged them to think about the questions they want to answer and start simple; describing the data they've got first (it's not been accessed at scale before), and assessing quality before thinking about network mapping. Also to start by building confidence in using data, maybe just reflecting some simple stuff back to committees.

Liz and Cassie (from the House of Commons Library) are looking at whether we can embed reports or tiles (or whatever they're called) into the [Second Reading](https://secondreading.parliament.uk/) blog. This is part of the work to improve constituency statistics reporting and develop better self-service information.

Saffiyah, Liz and Sara met with the User Research team to see how we can collaborate better and more frequently. Saffiyah also met with [Alex](https://twitter.com/alexedwardh) to see if we can access the Search and Indexing triple store to get data to help make KPIs for the Indexing and Data Management Section (IDMS) of the House of Commons Library.

### Corporate data

[Matt](https://twitter.com/matiasgermanico) is currently working on a couple of people data initiatives. One's looking at how we might digitise the very, very many forms that are currently paper-based. Whilst also looking at how we might update the underlying processes. The second is trying to find new ways to perform all the people data matching and syncing. And get cleaner, more useful data as a result.

David made a significant improvement to the integration for the office move system. Field mappings were tested and verified. The project is now almost ready for release.

Noel had a meeting with the Learning and Development people about the data that's currently sent to the learning platform and how that matched up to their reporting needs. A plan was agreed in principle to supply them with reports.

Lewis continued his investigation around new types of data integration solutions. Did I just type solutions?

### Excellent customer service award...

...appears to go to Dan this week. He picked up a request from a student doing research around election results, pulled off a [Cruyf-like turn](https://en.wikipedia.org/wiki/Cruyff_Turn) and hit a pin point cross to [Oli](https://twitter.com/olihawkins), who brought down the ball and flicked it to [Carl](https://twitter.com/carlbaker). Back of the net. Total customer service.

### Are topics fashionable?

My god, are topics fashionable. You can barely turn a corner without some 'multidisciplinary website product team' shouting topics at you. Suddenly everyone is talking about topics. Topics topics topics topics topics. Browse by topic. Search by topic. Topics. These things come in phases. Next week we could be back to calendar views.

### Did anyone say blockchain?

Aidan, Jamie and Dan mentioned Bitcoin briefly, which is dangerously close. Thankfully no-one said Ron Paul or weeeed so we think we're still safe.

### Strolls

Strolls have taken something of a back seat since we discovered we have neither reliable metrics nor KPIs. A sub-committee has been formed to investigate this predicament. How can one stroll without reliable metrics or KPIs? Or indeed user needs? We'll get back when the report is published.

### Michael would like to thank...

...the many people who expressed condolences on the sad loss of both [Siobhan](https://twitter.com/fantasticlife/status/934436448958160896) and [Marquis](https://www.youtube.com/watch?v=YchlTWWVNk8) in the same week. Hard times.


### Things that caught our eye

* [Linked data templates](https://atomgraph.github.io/Linked-Data-Templates/)

* [Wikidata hackathon in London](https://www.eventbrite.co.uk/e/wikidata-hackathon-in-london-all-levels-of-experience-welcome-tickets-42426460686?aff=efbevent)

* [Dave on measuring things](cognitive-edge.com/blog/a-sense-of-direction-2-2/)

* [The Era of Quantum Computing Is Here. Outlook: Cloudy](https://www.quantamagazine.org/the-era-of-quantum-computing-is-here-outlook-cloudy-20180124/)

* [The AI Hierarchy of Needs](https://hackernoon.com/the-ai-hierarchy-of-needs-18f111fcc007)