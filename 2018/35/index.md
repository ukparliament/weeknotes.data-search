## 2018 Week 35

### One world, one web, one team

In the absence of [Dan](https://twitter.com/dasbarrett) (and his [yo-yo](https://ukparliament.github.io/weeknotes.data-search/2018/34/#get-yer-yo-yos-out)) [Matthieu took on data strategy duties](https://twitter.com/cognithive/status/1035152530358067200). An open session was run. Models and measurement were discussed.

[Alison](https://twitter.com/oliala), [Samu](https://twitter.com/langsamu), [Matt](https://twitter.com/mattrayner) and [Jamie](https://twitter.com/oddtype) (and assorted other computational experts) reviewed the initial work on the Committee Information System API. It's being built by our colleagues in the Business Systems Development team with the Data Service (and therefore the new website) being the main client. It's all part of a major refresh of end-to-end Committees digital stuff planned for delivery in early 2019. The computational experts had some thoughts and suggestions about the underlying model, the technical implementation of the API and how we might collaborate. Jamie's planning to catch up with Head of Business Systems, Matt Stutely next week to turn thoughts into plans.

Alison grabbed Samu and Jamie to talk about the modelling work for [Visiting](https://www.parliament.uk/visit/). Parliament puts on lots of events that the public can book and attend but these are managed by an array of departments and systems. One of the main systems is due to be refreshed, so we're looking at how we can improve and unify the online experience for people wanting to visit [our palace](https://en.wikipedia.org/wiki/Palace_of_Westminster). They came up with a few options. The conclusion, at least for now, is to continue aggregating and refining the information on current events in the context of the models. Which, roughly translated, means: make a really nice spreadsheet. With a view to this information evolving into a new data source.

Martin Casey, the Business Partner for [Strategic Estates](https://www.parliament.uk/mps-lords-and-offices/offices/commons/teams/#jump-link-7), got in touch with our Liz to chat dashboards. Strategic Estates have been working on designing a dashboard with an external consultancy, and they now want to bring it in house. The current dashboard uses data from our internal learning and development system and [Microsoft Project](https://en.wikipedia.org/wiki/Microsoft_Project). So far it's all been built on spreadsheets. Liz explained that they could build their own dashboard with support from the [Parliamentary Computational Section](https://pds.blog.parliament.uk/), but she suspects that access to the learning and development system might prove tricky. We haven't yet seen the available reporting data, but have a feeling we won't be able to connect directly. <a href="https://www.youtube.com/watch?v=y9Gf-f_hWpU">There is light</a> though: it looks like there's a content pack for Microsoft Project, if they move online we should be able to query via [OData](https://www.odata.org/).

We're told that the back and front end teams released a new [search](https://beta.parliament.uk/search) architecture today. More precisely, that it's happening right now. As. I. Type. So far Slack is not exploding so we can only assume it's going well.

### Domain modelling

We entered our second week without a working copy of [LODE](http://www.essepuntato.it/lode). Which means we're still unable to generate HTML to match our [turtle](https://en.wikipedia.org/wiki/Turtle_(syntax)) files. [Published models](https://ukparliament.github.io/ontologies/) remain unchanged. At least in HTML form. Elsewhere Robert is attempting to write a turtle parser to fix this problem. Which would be splendid.

[Anya](https://twitter.com/bitten_), Jayne, [James](https://twitter.com/thevinternet), [Silver](https://twitter.com/silveroliver) and [Michael](https://twitter.com/fantasticlife) got together to chat about potential improvements to the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html). It was all very early on bank holiday Tuesday but brains fed on nicotine and caffeine ground sluggishly into gear. Three things got covered:

* Given we have dates and not times for [business items](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e193) and given that multiple business items can and do happen on the same day, ordering them on [work package](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e284) pages in a way that makes chronological sense, procedurally speaking, can be tricky. So far we've tried ordering by distance from the starting [step](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e272) in the procedural graph but there are often many paths to the same thing. And paths through the House of Lords tend to involve more steps than those through the House of Commons. We wondered if introducing a level of inheritance, bridging between similar steps in each House, would help solve this. So the 'approval motion tabled' step could have 'approval motion tabled in House of Commons' and 'approval motion tabled in House of Lords' as child steps. Which would at least help with some sense of symmetry. But we're not yet sure if the step ordering on work package pages takes into account "requires" routes. If it does, we may be able to add more "requires" routes to help order things. And if that fails, we're back to considering step inheritance.

* To differentiate between things that can happen only once in a work package (e.g. an [EVEL](https://en.wikipedia.org/wiki/English_votes_for_English_laws) decision) and things that can happen multiple times and in parallel (e.g. the tabling of non-fatal approval motion amendments) we introduced the concept of self-preclusion. A step is related to itself by a "precludes" route if it can only be [actualised](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e22) once. Which means, having happened, that step would no longer show up in the space of future possibilities. But some things - like debate scheduling - can happen many times and in series, and only if you cycle through a debate not reached step. We can't make debate scheduled self-precluding as it can happen again, but if we don't make it self-precluding it will always show up on the list of possible future things. The only way we can think this might be made to work is to introduce route level [logic gates](https://en.wikipedia.org/wiki/Logic_gate). But we're not quite sure what that would look like. And it would complicate things enormously. And it's not strictly untrue to say that a debate having been scheduled, one possible future event is for the debate to be scheduled. So for now we've decided to leave well alone. Cos it's hard and, at least for now, it's not really breaking things.

* We currently don't have a mechanism for linking the [tabling](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html#d4e231) of a particular motion or motion amendment to a subsequent withdrawal. At least, not within procedural data. So multiple Members might table non-fatal amendments to an approval motion, and they will probably be debated and decided upon. We're currently saying that a debate and a decision on a motion amendment is precluded if the motion is withdrawn. But if one of many motion amendments is withdrawn, this isn't true. There are other motion amendments on the table. So we need to remove the "precludes" roues between amendment withdrawal and decisions. And take into account business data when calculating any future possibility space.

Which is an <a href="https://www.youtube.com/watch?v=Zx1_6F-nCaw">awful lot of words to describe not much action</a>. Much like the meeting then.

Most of the rest of Anya, Silver and Michael's day involved sitting around with Robert practising a [talk we're due to give at NetIKX in September](http://www.netikx.org/content/ontologies-and-domain-modelling-fun-honest-and-friendly-introduction-20-september-2018). Michael attempted to run though a workshop thing but Robert decided workshopping Michael was more fun than idle participation. Tough crowd this.

Anya, Silver and Michael spent Thursday with [David Beamish](https://en.wikipedia.org/wiki/David_Beamish), idiot checking some of their recent models and dipping into timetabling and [order papers](https://en.wikipedia.org/wiki/Order_Paper). They ran through the procedure model, associated [statutory instrument](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) [flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples), the [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html), [laying](https://ukparliament.github.io/ontologies/laying/laying-ontology.html) and [tabling](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html). A handful of improvements were suggested and found their usual home on [Trello](https://trello.com/b/Z1nrm0Vr/parliament-ontology). More meetings with Table Office types to talk timetabling are planned.

Librarian Jayne and our [Alex](https://twitter.com/alexedwardh) spent a delightful couple of hours staring at flowcharts for [draft negative](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/draft-negative.pdf) and [made negative](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/made-negative.pdf) SIs and comparing them against the procedure data. Jayne developed an appreciation for why Michael may have dozed whilst doing the same exercise last week. It is very tiring work. Luckily, librarian Emma arrived bearing fudge so sugar carried them through. We're told they talked about dogs but it's not clear from Slack if they like dogs. Or hate them.

### Corporate data

["The car is on fire, and there's no driver at the wheel"](https://www.youtube.com/watch?v=XVekJTmtwqM)

But that was last week. This week Lew's been doing some [BizTalk](https://en.wikipedia.org/wiki/Microsoft_BizTalk_Server) maintenance, fiddling with performance improvements and setting up our test environments. Noel's been looking at outstanding tickets in our incident management system and checking if they're related to the fire.

### Customer service of the week award goes to...

...[librarian Jayne](https://www.youtube.com/watch?v=f3V-7DEAgdc). 

The nomination arrives from Alex who received a request from the [Knesset Archives](https://knesset.gov.il/archive/eng/ArchiveIntro_eng.htm) to provide session level Member activity counts for things like the number of [Private Members' Bills](https://en.wikipedia.org/wiki/Private_Members%27_Bills_in_the_Parliament_of_the_United_Kingdom) sponsored, the number of [written questions](https://www.parliament.uk/business/publications/written-questions-answers-statements/written-questions-answers/) tabled etc. Jayne kindly helped out. For which read: did the actual work. Alex tells us 'we' were able to provide everything requested out of [Solr](http://lucene.apache.org/solr/). Not all developers, man.

We're still stuck on the number of motions per member as this is all a bit tricky. But we continue to investigate. And feel sure Jayne will come up with the goods.

### Strolls

Not much in the way of strolls this week, although Anya and Michael did manage to clock up 22 miles in 2 days. Sore feet resulted.

Anya, Silver and Michael took a considerably shorter stroll down to Bellamy's, headquarters of the Parliamentary Pudding Section. An institution long famed for its commitment to quality steamed puddings and custard. The bread and butter pudding was less than lukewarm. The custard was slightly warmer but lumpy. Standards have slipped. You can certainly tell it's recess.

### Things that caught our eye

* [The Role of Visualisation in Data Analysis](https://www.youtube.com/watch?v=ZdPNBF6GWBw)

* [Shower With Your Dad Simulator 2015: Do You Still Shower With Your Dad on Steam](https://store.steampowered.com/app/359050/Shower_With_Your_Dad_Simulator_2015_Do_You_Still_Shower_With_Your_Dad/)

* [https://beta.layersoflondon.org/map/layers](https://beta.layersoflondon.org/map/layers)

* [Chicken Chicken Chicken: Chicken Chicken](https://isotropic.org/papers/chicken.pdf)