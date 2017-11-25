## Week 18: 25-11-2017

### [Leave the Capitol](https://www.youtube.com/watch?v=GpMoRS_9bcM)

Yet another reminder that our [5th Parliament, data and democracy meetup](https://attending.io/events/parliament-data-and-democracy-meetup-5) is on Wednesday 6th December, this time at [ODI Leeds](http://leeds.theodi.org/).

Speakers lined up are our [Dan](https://twitter.com/dasbarrett), [Cristina Leston-Bandeira](https://twitter.com/estrangeirada) (Professor of Politics at the University of Leeds), [Tom Forth](https://twitter.com/thomasforth) (Head of Data at ODI Leeds) and [Edward Wood](https://twitter.com/edwardwood99) (Director of Research in the House of Commons Library).

More in the way of interesting talks, nice people and [free beer](https://en.wiktionary.org/wiki/free_as_in_beer). Come along. Bring a friend.

### International, continental, Parliament in the area

[The boss](https://twitter.com/dasbarrett) managed to cadge a last minute trip to Geneva to attend an [IPU](https://www.ipu.org/) working meeting on the establishment of a centre for innovation in Parliament. He seems to be having a [fine time](https://www.youtube.com/watch?v=MYwNLlTt3AQ) and looks [proper dandy](https://twitter.com/dasbarrett/status/934111032162832387).
 
### Community

[Alex](https://twitter.com/alexedwardh) produced data for the [House of Commons Library subject indexing terms](http://www.data.parliament.uk/dataset/thesauri) and their usage frequency for [Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife). There are a huge amount of subject IDs and uncontrolled terms in the Search and Indexing [triplestore](https://en.wikipedia.org/wiki/Triplestore), so Wojciech helped to write a script that chunks the queries based on [Parliamentary sessions](http://www.parliament.uk/about/how/occasions/calendar/) so we didn't accidentally break anything. Unfortunately, after consolidating all of the usage frequency counts, the data didn't quite match up because some records in the triplestore don't have a session attached to them. Oops. [Liz Marley](https://twitter.com/greensideknits) was able to produce a list of subject types that do not have sessions. This was used to find and consolidate the missing data. Except 'Deposited Papers' and 'European Scrutiny and Information' because they're huge datasets and there's no nice way of chunking them. Yet. Work continues.

This is here because it's a step forward in our attempts to link House of Commons subject headings to [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page). If you're interested in that, you're probably best off reading [last week's weeknotes](https://ukparliament.github.io/weeknotes.data-search/17/).

Liz, Robert, [Samu](https://twitter.com/langsamu) and Michael had a call with Chris Pennock and Justin Moore from Google about standardisation of data models around elections and election results. And other associated stuff. There were no concrete outcomes but the intent was good. Michael notes we need to chat to [NIST](https://www.nist.gov/) about the work they're doing here.

Anya, [Silver](https://twitter.com/silveroliver) and Michael went over to see [Ganesh](https://twitter.com/gansenthi) (ex of this parish) at [GDS](https://gds.blog.gov.uk/) to talk about domain models and URLs for making [gov.uk](https://www.gov.uk/) more navigable. Michael introduced the GDS front team to the GDS [registers](https://gds.blog.gov.uk/2015/09/01/registers-authoritative-lists-you-can-trust/) team and felt quite smug about it. It was a really, really good day ending with full whiteboards and beer. Not very Parliament but it's all part of the same jigsaw and there's really no such thing as a website. We need to make these things join like [Voltron](https://www.youtube.com/watch?v=2kkJDHRYxWM).

Anya and Michael met with [Nick Halliday](https://twitter.com/nickmhalliday) from the [NAO](https://www.nao.org.uk/) to chat about data models and challenges. Again it was good. Things are better when we get out more. They also talked about registers and [convening some public sector types to chat about duplication in the lists they manage](https://twitter.com/nickmhalliday/status/934111187591204865).

### Data day

Wednesday was [data day](https://twitter.com/aidan_morgan/status/933378211991511042). [Ellie Craven](https://twitter.com/ellayanor) and [Arnau Siches](https://twitter.com/arnau_siches/) from [GDS](https://gds.blog.gov.uk/) came along to chat about registers that Parliament might need and registers that Parliament might produce. We agreed to start simply with a register of [houses](https://beta.parliament.uk/houses) because that's only two things and isn't subject to too much churn. We also talked about registers of members, committees and the House of Commons Library subject headings.

People from the website team came along and some stuff was agreed:

* The decision was made to ‘let the [bots](https://en.wikipedia.org/wiki/Web_crawler) in’ so that [beta.parliament.uk](https://beta.parliament.uk/) can be indexed by Google, Bing et al. [Jamie](https://twitter.com/oddtype) will look into questions about ownership and administration of Google Tag Manager.

* The data and search team will work with the Guide to Procedure team to help refine and model content types. This is part of bringing support for structured content into the data platform. Data models will be aligned to ontologies and instance data will be aligned to House of Commons Library subject headings.

* Jamie will arrange for Samu's tracking code snippet to be added to all beta pages.

* Michael needs to chat with [Ed](https://twitter.com/ewhitur) and Angela about modelling committee staff and associated privacy concerns.

* The old website search will be turned off in the next two weeks.

* Work will continue on making Deposited Papers searchable. Letting search bots into selected bits of data.parliament will be the first step.

### Corpcomms

You'll really need to check Yammer for this.

### One world, one web, one team

[Aidan](https://twitter.com/aidan_morgan) spent more time with the Indexing and Data Management Section in the House of Commons Library. He had some meetings to discuss next steps for the Data Toolkit work, and priorities for support, including looking at automation of some of the regular tasks that the team perform.

He also spent time with Mike and the Business Systems team so he can start to understand the infrastructure and data flows that relate to Indexing, Search and subject index management systems.

Michael helped with a service assessment for one of the new web services. More curates eggs; more eggs.

### Domain modelling

Angela and Michael continued with the autopsy of Red Book (a database used by the House of Commons for managing committee data). More work is still needed.

### Data platform

[Chris](https://twitter.com/chrisalcockdev) and Samu explored ontology alternatives to "ClassType" classes and are considering reintroducing [restriction classes](https://www.w3.org/TR/owl-ref/#Restriction) to the ontology to avoid combinatoric explosions. Trust me, nobody wants combinatoric explosions.

[Jianhan][https://twitter.com/jianhanzhu] continued to work on the [OData](https://en.wikipedia.org/wiki/Open_Data_Protocol) service which now covers OData expand, count, and navigation property functionality. He worked with Samu on using OData test suites to test the service conforms to the standard.

[Ben](https://twitter.com/benwoodhams) has almost completed work on Lords' Inflation (still really don't ask). Expect floating baronesses over Westminster shortly. The next step is to get a seal of approval from [David Beamish](https://en.wikipedia.org/wiki/David_Beamish). Chris has been working on extensions within the platform but needs the final go ahead from Ben before proceeding with work to import the data.

### Search

[Dia](https://twitter.com/DN78) worked on the first draft of the search strategy, vision and the goals. The plan is to align them to [Parliament's digital strategy](https://www.parliament.uk/mps-lords-and-offices/offices/bicameral/parliamentary-digital-service/digital-strategy-for-parliament/).

[Raphael](https://twitter.com/raphaelleung) worked on running the [Berlin SPARQL Benchmark (BSBM)](http://wifo5-03.informatik.uni-mannheim.de/bizer/berlinsparqlbenchmark/spec/), which measures the performance of storage systems that expose SPARQL endpoints.  He's testing it against endpoints set up on our services, building on Matthieu's performance testing. He'd like to find out the key variables (specifically different inference rulesets) that affect the performance of the triplestore setups that are available to us. He's using non-parliamentary data from a recognized benchmark. He spelt recognised wrong.

Michael wrote [a post about our general approach to search](http://smethur.st/posts/176135866). And browse. S'ok. If reading this is your thing you should read that. Definitely.

### Measuring things

Sara has been analysing application insights data, particularly the photo API requests. Samu and Matthieu made changes to the tracking code on the website that enables sharing analytics across subdomains. Which, in the case of photos, are served from api.parliament.uk. Once the tracking code is changed, we will be able to correlate page views with photo requests. We can then track if an API call was made from the beta website or from external users.

### Capability

Aidan got approval for an ADSL line for the team, to help support development and DevOps activities.

### Did the machines learn owt

Did they heck.

### Did anyone say blockchain

Nope. Unlike the machines, we're not thick.

### Strolls

No strolls were reported. Expect productivity hits in a month. Or so.


### What's Samu watching?

Samu watched [The Future of Programming](https://www.youtube.com/watch?v=ecIWPzGEbFc), a talk by [Bob Martin](https://en.wikipedia.org/wiki/Robert_C._Martin), a signatory of the Agile Manifesto. Uncle Bob talks about the past, present and future of programming and programmers, about the gender divide in the industry, about what "agile" was really supposed to mean (in the sixties and the nineties) before it was hijacked by "project managers", about NASA programmers working in six week iterations when automating the trip to the moon, and about how programming needs to mature if it's to claim the universal leadership role that's its birth right. \o/

Also from Samu: [A Mother’s Confession: A SONG WITH FOOTNOTES by Amanda Fucking Palmer](http://amandapalmer.net/amothersconfession/)

### Things that caught our eye

* [Combinatorial explosions explained with ice cream](https://medium.freecodecamp.org/combinatorics-handle-with-care-ed808b48e5dd)

* [RDF2Vec: RDF Graph Embeddings and Their Applications](http://www.semantic-web-journal.net/system/files/swj1643.pdf) [PDF klaxon]