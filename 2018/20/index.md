## 2018 Week 20

### More visions

Not so many people had visions this week, but [Dan](https://twitter.com/dasbarrett) did have a couple of catch-ups with Robert where they spoke about all things data and search and strategy. Great stuff, says Dan. 

### Liberating the library

Following up on last week the [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) community has now [manually matched 3672 of our thesaurus subject headings to Wikidata things](https://tools.wmflabs.org/mix-n-match/?#/catalog/1229). Which is ~8% of the total. Not bad going for a week.

### Showing and telling

[Sara](https://twitter.com/sarafreis) and Liz showed and told. They gave an overview of the analysis work on parliamentary material that's been subject indexed with the [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri) by the Indexing and Data Management Section of the House of Commons Library. This data hasn’t been easily available in the past and has the potential to be used as feedback for indexers to improve the quality and consistency of their work. The showing and the telling were well received (although a telly would be an improvement on the projector) and questions were asked. They're planning to spend more time digging into this area, to look at the usage and relatedness of subject headings, which will hopefully drive some of the website work around 'topical' concepts and concept cooccurrence.

### Community

We've been pretty big on community this week. On Wednesday, [Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver), Robert, [Michael](https://twitter.com/fantasticlife) and [Chris](https://twitter.com/c_fryer) (from the [Parliamentary Archives](https://www.parliament.uk/archives)) went along to [The National Archives](http://www.nationalarchives.gov.uk/) for a joint session on records and data with TNA and [Wellcome Trust](https://wellcome.ac.uk/) people. It was a good session with lots of shared areas of concern and a couple of fairly concrete things we want to work on.

The first is more Parliament / TNA focussed, with a commitment to collaborate on a UK wide legislation model that won’t give [John Sheridan](https://twitter.com/johnlsheridan) sleepless nights.

The second is a meeting to discuss reference data: where organisations have [lists of things](https://github.com/ukparliament/ontologies/blob/master/list-of-lists.csv), where those lists are duplicated and who we think the appropriate custodian should be. Lists of government departments, positions and incumbents being a perennial bugbear here. Michael is trying to organise something and invites have been extended to the [ONS](https://www.ons.gov.uk/) and [NAO](https://www.nao.org.uk/). If you think you might have lists of public sector things that you shouldn't really be maintaining, or indeed should be, do [get in touch](mailto:smethurstm@parliament.uk). It's definitely all more town planning than skyscrapers but then the useful work usually is.

In other [register](https://www.registers.service.gov.uk/) related news, Dan's been doing a little more digging (plotting?) on how we might publish a register of [Members](http://beta.parliament.uk/people/members) of both [Houses](https://beta.parliament.uk/houses). Stay tuned.

On Thursday, Anya, Robert and Michael met some people from the [Electoral Commission](https://www.electoralcommission.org.uk/) to talk about the [House of Commons Register of Members' Financial Interests](https://www.parliament.uk/mps-lords-and-offices/standards-and-financial-interests/parliamentary-commissioner-for-standards/registers-of-interests/register-of-members-financial-interests/). The Electoral Commission take "data" from Parliament but have to enrich what we provide to make it meaningful. More structured data would reduce the need for rekeying and reduce their workload. So we're keen to work with them and understand their use cases. They've also put us in touch with the [Independent Parliamentary Standards Authority](http://www.theipsa.org.uk/) to see if they have similar needs for better structured parliamentary data.

In even more community news, Dan had a good meeting with [Dr Ruth Dixon](https://twitter.com/ruth_dixon) on Monday. Ruth is doing a year-long research project with the [House of Lords library](https://www.parliament.uk/business/lords/work-of-the-house-of-lords/lords-library/), and was looking at how to get XML versions of bills out of [data.parliament.uk](http://www.data.parliament.uk/). Which is currently pretty painful. Can we make it better? We would like to think so.

### Domain modelling

In [last week's episode](https://ukparliament.github.io/weeknotes.data-search/2018/19/), I typed, "They did tidy up some of the legislation model, though Michael still thinks it looks wonky / broke." [John Sheridan](https://twitter.com/johnlsheridan) happened to be reading and [a conversation ensued on Twitter](https://twitter.com/johnlsheridan/status/995231601301884930). Michael received a message from John saying that the proposed legislation model was giving him nightmares and making him lose sleep. Which came with an offer to collaborate. Which we've taken him up on. We now have copies of some of the TNA models which Silver is currently drawing up. Hopefully next week we make a start on something sane that doesn't upset John.

On Tuesday, Silver and Michael met with [Oli](https://twitter.com/olihawkins) and Philip Brien from House of Commons Library research land to start on a model for [research briefings](https://researchbriefings.parliament.uk/) and similar documents. For a one hour session with two people, it felt like they got through a lot and have managed to draw up [a very basic picture](https://github.com/ukparliament/ontologies/blob/master/document/document.png). They still need to do more work with both libraries and dig a little deeper into [POST](https://www.parliament.uk/post) publications. But it's a start.

Just about every week I type something about [procedure flow charts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples) with the optimistic claim that, "they think they're almost there now". We do often think this, but we're just as often disappointed. IDMS spent last week adding [procedure](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e238) data according to the flowcharts. This week they've been busy adding [workpackage](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e284) data to actualise the procedural steps. [Samu](https://twitter.com/langsamu)'s been looking at the workpackage [visualisations](https://procedures.azurewebsites.net/WorkPackages/72/graph) Raphael made and has spotted a number of precluded routes that we've failed to spot. Things like, Parliament having decided to agree to a motion, there's currently nothing in the procedure data to preclude them from disagreeing. Which feels obvious. But not when your face has been pressed up against the glass for weeks. So we don't think we're nearly there now. We probably think we'll never be there.

On a more positive note there was a good meeting between the IDMS folks who are mincing the pork, the Data and Search folks who are making the sausages and the web folks who are packaging them. So we feel we have a better grip on the ends and the middle. Though, as Robert might say, it's all just balloon squeezing. But with visualisations.

### Data platform

Liz and [Mathieu](https://twitter.com/cognithive) have been hatching a plan to generate report style data from [VocBench](http://vocbench.uniroma2.it/) (our preferred option for future management of the IDMS controlled vocabulary). Ideally, they'd like to export the audit history and use it for reporting on when new concepts are added, amended etc. All this information is currently compiled into Word documents by IDMS so anything would be an improvement. They've been in touch with the lead developer for VocBench and this is on his roadmap. In the meantime, he's given Mathieu some tips on writing [SPARQL](https://en.wikipedia.org/wiki/SPARQL) that should help here.


### On searching and indeed indexing

Liz and [Alex](https://twitter.com/alexedwardh) had a chat with Joe Foster about the processes involved in slurping material out of business systems and into the search and indexing triple store. They're interested in what information is 'available to index' and when. Unfortunately data about when material enters the triple store isn't captured, so it isn't currently possible to accurately assess the data transfer. Ideally they'd like to be able to describe what it looks like now (delays in receiving information, typical time scales for indexing etc.) so there's a baseline to compare against as and when we make changes to the data and processes involved. Work continues.

### Corporate data

Dan held the first of two workshops with Lew, [Mat](https://twitter.com/matiasgermanico), Noel and David to get on top of things before Mat leaves. They looked at the priorities for data integration for the next year. The main things to come out of it for Dan were:

* We've got some fairly urgent work to do to update integrations that rely on end-of-life components.

* We should start to use Logic Apps for new things.

* We're going to have to work with Technology colleagues to get past some of the current network configurations that make moving to a new model impossible.

### Strolls

Again, we saw very little in the way of strolling this week. Though Anya, Silver, [Ben](https://twitter.com/benwoodhams) and Michael did stroll to Soho to meet [Ganesh](http://twitter.com/gansenthi) (ex of this parish). There was more talk of SIs and registers. They called in at the [Toucan](https://www.tripadvisor.co.uk/Restaurant_Review-g186338-d720848-Reviews-Toucan-London_England.html) and tried to buy a round of [Poitín](https://en.wikipedia.org/wiki/Poit%C3%ADn). But the landlord couldn't sell them any. Because it is now illegal. Or so we were told. Presumably under an SI or some such. Someone should really build a tracker.

### Things that caught our eye

* [Scientific debt](http://varianceexplained.org/r/scientific-debt/)

* [Wes Anderson Palettes](https://wesandersonpalettes.tumblr.com/post/109980167015/peter-fuck-the-itinerary)

* [Why a Flat Organizational Structure will Fail as You Grow](https://getlighthouse.com/blog/flat-organizational-structure-fails/)

* Dan read a Wikipedia page about the [Cuisine of New Orleans](https://en.wikipedia.org/wiki/Cuisine_of_New_Orleans) and now wants to visit. If anyone knows of any Louisiana based data conferences, do shout

* [Terrible tag line, decent city](https://tc18.tableau.com/)