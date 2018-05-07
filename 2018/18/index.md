## 2018 Week 18

### The delivery is strategy

[Dan](https://twitter.com/dasbarrett) spent the week doing data strategy work with some of the programme managers. He also met with [David Smith](https://twitter.com/SmithDavidM) (Deputy Director of the [Parliamentary Computational Section](https://pds.blog.parliament.uk/)) and Steve Wise (from the House of Commons Library) to talk about 'tactical projects' and governance.

### Community

[Michael](https://twitter.com/fantasticlife) had a meeting with Emma and Paul at the [History of Parliament Trust](http://www.historyofparliamentonline.org/) to chat through some of the details of publishing the Rush data on (historical) Members of the House of Commons. It went well despite a hog whimpering hangover. There is a plan. Or two plans and a decision to be made.

### One world, one web, one team

[Matthieu](https://twitter.com/cognithive) explored [VocBench](http://vocbench.uniroma2.it/)'s capabilities with [Liz](https://twitter.com/greensideknits) from the Indexing and Data Management Section in the House of Commons Library. They think that having the management of the [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri) backed by a SKOS-y graph will offer interesting new perspectives.

### Domain modelling

Our Liz has been thinking some more about how we add constituency level demographic statistics to the data platform. She found some info on statistical modelling in RDF. [Silver](https://twitter.com/silveroliver) and Michael think it's probably a bit complicated for what we require right now, but they need to peer at it a bit more. She also had a chat with Michael about future opportunities for subject indexing statistical datasets. Once we have the controlled vocabulary in the data platform and tools for indexing, there are some interesting opportunities in applying concepts to statistics.

[Anya](https://twitter.com/bitten_) and Michael met with Jane, Jack, Jenna, [James](https://twitter.com/thevinternet) and [Jen](https://twitter.com/benwoodhams) for one last (coughs) look at the [flow charts for Statutory Instruments](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples). These now include additional arrows to describe relationships where something or some things must have happened to allow another thing to happen. They also cleared up a few remaining questions around the procedure ontology and [SI](https://en.wikipedia.org/wiki/Statutory_instrument_(UK))s in general. Last week I typed that every week I type they think they're almost there now. They absolutely do think they're almost there now. Definitely. Absolutely.

### Data platform

Most of the effort this week was also concentrated on the tracking of SIs. Wojciech, [Chris](https://twitter.com/chrisalcockdev), Raphael and [Samu](https://twitter.com/langsamu) stared intently at screens and discussed the differences between a work package and a workpackagable thing and whether the work package was subject to a procedure or whether the workpackageable thing was subject to a procedure. At length.

Anya and Michael chatted to Samu about how the data would be entered and what we'd need to capture in the short term. Chris just got on with building it.

Samu and Raphael submitted a pull request to [dotNetRDF](http://www.dotnetrdf.org/) to add support to serialise graphs in [GraphML](https://en.wikipedia.org/wiki/GraphML) format. GraphML is an XML-based format to describe graphs that's compatible with many graph visualisation and analysis tools. The goal is to allow people to request our data in an additional format which is popular in network analysis. Raphael has made a [Jupyter Notebook](http://jupyter.org/) to [visualise an SI procedure as a directed graph](https://nbviewer.jupyter.org/github/lcyraphael/parlpublic/blob/master/Procedures_network_analysis.ipynb?flush_cache=true).

[Matt](https://twitter.com/mattrayner) has also been busy with pull requests, adding functionality to fetch and parse a Request-Id header, which has made it to the latest release of the [Application Insights SDK for Ruby](https://github.com/Microsoft/ApplicationInsights-Ruby). It takes us a step closer to unifying client and server side logs which should help us better understand user behaviour.

### Corporate data

Amongst the upheaval caused by the move of the Parliamentary Computational Section from Millbank to some madman's castle in Whitehall, Lew's monitors got stolen. Then turned up. Dan says it was like Columbo. Michael disagrees because he has [strong reckons about Columbo](http://smethur.st/posts/66087518).

### Strolls

Anya and Michael took a birthday stroll with Robert to the [Coleman Coffee](https://www.tripadvisor.co.uk/Restaurant_Review-g186338-d10219719-Reviews-Coleman_Coffee_Roasters-London_England.html) shop. Oatcakes were eaten. Chocolate milkshake was drunk.

They also popped into the [backstage bit at the Dorfman theatre](https://www.nationaltheatre.org.uk/your-visit/sherling-backstage-walkway). It's ace. You should go if you're ever in that London.

### Did anybody talk about whether sexual fantasies, ontologically speaking, might best be modelled with a foaf:primaryTopic of foaf:Agent or a foaf:primaryTopic of skos:Concept with a foaf:focus of foaf:Agent? And whether the objectification of pornography might weaken or nullify the foaf:focus? And whether the foaf:focus and foaf:Agent even exist given a solipsistic worldview?

Yeah. That's a thing that [happened](https://twitter.com/fantasticlife/status/991783646699950080).

### Waving goodbye to Millbank

Our new home is mad. From the outside it looks like someone decided to build a castle, then went down B&Q. On the inside there are bits that look like a minor league stately home (where the project managers seem to be), bits that look like an out of town office in Basingstoke (where we are), and bits that look like an abandoned mental hospital. Where the ghosts are. And the mouses.

### Things that caught our eye

* [Against metrics: how measuring performance by numbers backfires](https://aeon.co/ideas/against-metrics-how-measuring-performance-by-numbers-backfires)

* Liz points at [Excel vs R](https://www.jessesadler.com/post/excel-vs-r/). More for the discussion at the start than the intro to R. She thinks she's been thinking in Excel for a long time.

* [Statistical Data and Metadata eXchange](https://sdmx.org/?page_id=2561)

* [Data Documentation Initiative Alliance RDF specifications](https://www.ddialliance.org/sites/default/files/DDICharter2013.pdf) [PDF]

* [HTML Color Codes](https://htmlcolorcodes.com/)
