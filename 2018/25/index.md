## 2018 Week 25

This weeks edition was guest edited by [Alison](https://twitter.com/oliala).

### Showing and telling...

This week was David's turn to show and tell. In his talk - "My visit to a data integration conference" - he spoke about researching data integration tools, culminating in an exhilarating trip to [INTEGRATE 2018](https://www.biztalk360.com/integrate-2018/). He learned a lot and so did we. Thanks David.

### Community

[Michael](https://twitter.com/fantasticlife), [Anya](https://twitter.com/bitten_) and Robert were meant to meet Maryam Ahmed, who's a data scientist at the BBC and has previously done work analysing Hansard. Unfortunately she couldn't make it, which is sad, but they consoled themselves by talking to [Jamie](https://twitter.com/oddtype) about step names and web design instead.

### One world, one web, one team

[Dan](https://twitter.com/dasbarrett) has been been settling into his additional 'Service Owner' job this week, which has seen him going to stand ups, sifting and interviewing a contractor developer and meeting with the folks from Restoration and Renewal to learn about their plans. He also  met with [Jeanette](@clementgraphics) and [Steve](https://twitter.com/steve_bromley) to try to help make user research a more intrinsic part of the programme, and has looked at how he can join various initiatives together.

He also found time to attend a couple of workshops ; the first involved  people from across the department starting to break down the "What do we mean by service?" question for the work that Rebecca is leading.
The second was about agreeing, for the purpose of high-level tracking, what milestones projects and programmes across the organisation share and featured expert advice on unique identifiers. (Thanks all).

Anya and Michael went along to see Jane and [Jack](https://twitter.com/jackpdent) and some other clerks to talk about all things Brexit and Statutory Instruments (SIs) and the tracking thereof.

Alison spent a morning with the Indexing and Data Management Section (IDMS) indexing team in Tothill Street, chatting thesauri and quality control and an afternoon with Ed and James in Millbank House, learning the finer points of committees, evidence and their associated systems. She also spotted a painting of Malvern on a meeting room wall there, which made her happy.

[Matthieu](https://twitter.com/cognithive) did a lot of talking this week; he talked about [Vocbench](http://vocbench.uniroma2.it/) and [skos](https://www.w3.org/2004/02/skos/) controlled vocabularies with Alison, he talked about web components with Jamie and about windows core deployments with Wojciech. He even found time to talk about about in-memory graphs with [Samu](https://twitter.com/langsamu) as well as contribute to the reification discussions.

Aidan might have finally cracked the case of using Ontology Manager over [DirectAccess](https://en.wikipedia.org/wiki/DirectAccess). IDMS use this desktop software to modify their controlled vocabularies, but
when working remotely using DirectAccess, a kind of VPN, they've experienced problems connecting to the server component that hosts the vocabulary data.
After several months of troubleshooting (working with Mike and other colleagues in Parliament), Aidan thinks he has identified the cause. After laborious network traffic analysis, discussions with Samu and with the vendor, he found that the software relies on a version of a low-level networking protocol [IPv4](https://en.wikipedia.org/wiki/IPv4) that is not supported by DirectAccess. He's recommending issuing other laptops with earlier operating systems to these colleagues to restore their remote access.

Kunal worked with Joe Foster from Information Systems on testing possible future improvements to how Hansard reports on proxy voting and how that information might make it into Indexing & Search.


### Domain modelling

Anya solved our "too many things being called statutory day" problem  by renaming StatutoryDayCount to DayCount https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e301

Michael accidentally credited Jack with this breakthrough. The word MEN was used. Repeatedly. #hepeating

Jamie also made a late, evidence-based attempt to take credit for this breakthrough. This has so far been ignored. #hepeating

We now have what we think is a working legislation model (or enough for the SI tracker)

Given the procedure, laying and legislation models we think everything is covered for the SI tracker. but we'll still run past the [National Archives](http://www.nationalarchives.gov.uk/) - just in case.

Michael had a flashback to [information and ripples](http://www.cityofsound.com/blog/2004/07/ripples_or_the_.html) and tried to draw badly some [user circles](https://twitter.com/fantasticlife/status/1009802788145188865). He may have succeeded.


### Data platform

[Alex](https://twitter.com/alexedwardh) revisited a script with Matt that he began working on a little while ago to streamline the process of merging daily Solr output JSON files. Written in Python, the script takes arguments for a date range and downloads the relevant files from Azure Blob Storage. It then merges the JSON files, trims unneeded columns and converts to CSV. This is then uploaded back onto Azure Blob Storage ready for analysis.
Matt remembered his Python skills and managed to fix the issues with the script.

Wojciech, Matthieu and Samu spent some hours considering strategies for provenance; as we evolve our data management editorial/administrative user interface tools such as those currently being used by the Indexing and Data Management Section (IDMS) to create Statutory Instrument procedure data, we need to think about how we keep track of changes. This will help people in Parliament who enter and change data to track their own work but enable quality assurance so we can be confident that we can always find and revert mistakes.

More importantly, if we had an audit trail of changes to data, we could make it public (apart from private personal data, obviously). This would contribute to public confidence regarding the quality and authority of our data.

Discussions included:

- statement level [reification](https://www.w3.org/TR/rdf-primer/#reification) of [RDF](https://www.w3.org/RDF/) - a way of making statements about other statements
- using the [PROV ontology](https://www.w3.org/TR/2013/NOTE-prov-primer-20130430/#intuitive-overview-of-prov) - a data model for provenance interchange on the Web
- possible architectural styles for capturing audit information of resource mutation ([proxy](https://en.wikipedia.org/wiki/Proxy_pattern)/[interceptor](https://en.wikipedia.org/wiki/Interceptor_pattern) pattern), and
- possible storage scenarios (named graphs, separate repository, separate server)

Our Liz had good discussions with various people about transferring website measurements into the Microsoft environment, using AppInsight tracking and Azure services to help move and process data. We want to produce a consistent view of both what we are measuring and measurement outputs that are accessible in a variety of formats for reuse.

Our Performance Analysts will have access to AppInsight Analytics so they can learn how to query the data, and allow us to explore how we can make it a comparable service to Google Analytics (mainly spreading more tracking around). Our Liz and [Sara](https://twitter.com/sarafreis) will help them query the data platform using [OData](http://www.odata.org/) to look up what the IDs refer to, and help them become more familiar with what's there, using that endpoint. Data analysts and performance analysts  are planning to get together to discuss overall measurements for the website, and we'll use this as an opportunity to practice querying and to consider how we could validate the measures we come up with.

Matthieu, when he was not talking to people, was learning to love [C#](https://en.wikipedia.org/wiki/C_Sharp_(programming_language)) and Visual Studio. Live Unit Testing development flow is apparently a treat.

Thanks to some great work by Wojciech, the [UK Parliament API is now fully described by Swagger](https://twitter.com/langsamu/status/1010143705167290368)
He also put to good use the datasource change notification service Chris created some time ago and caught multiple changes to data we hold about Lords (jubilant arrivals and unfortunate departures).

[Jianhan](https://twitter.com/jianhanzhu) introduced an improvement to our [identifier generator service](https://www.slideshare.net/UKParliData/data-platform-id-generation).

Although the likelihood of identifier collisions with our eight characters and (currently) ~1 million resources is negligible, Jianhan reduced this to zero by checking each new generated identifier against the existing data to filter duplicates. Although this obviously increases the time it takes to create each new Id, we think it is worth it. As we move this new feature into production (the live environment), we'll track the actual performance degradation.

Last but not least, Usman, Jamie and Samu (and to a degree Jenna and James) spent some hours troubleshooting the workpackages page not working on beta.parliament.

Our first guess was that either web developers or data developers introduced a problem with a recent release.

We eliminated it being a Query API problem, then narrowed it down to a data entry or import problem.

Jamie looked at the data source and found duplicate identifiers: a recent workpackage was "the same" as a business item and a laying.

We removed the offending data from the service as well as the data source and will introduce it back next week with the same identifiers (minus duplication).

### On search. And indeed indexing

Sara and Matt went to the IDMS Indexing meeting that takes place every other Thursday, where team members discuss cases where indexing should be revisited for consistency. These discussions usually result in the introduction of new terms to the thesauri or data tasks where records must be manually re-indexed.


### Corporate data

Lewis continued work this week on gradually improving our KPI reporting infrastructure using Power BI.


### Employee of the week award...

is still Jayne Sunley in IDMS, still manically [actualising](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e22) [steps](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e272) by adding [business items](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e193) to [work packages](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e284) for the greater good of SI tracking.

### Strolls

Not a single stroll or trip to the seaside reported this week, despite the Summer sunshine. Tough times.

### Things that caught our eye

* [Space Syntax Ltd summary of Tim Stoner talk on "The new responsibility of architecture”](https://twitter.com/space_syntax/status/1009412696276717569)

* [Shallow by design by Michael Owen](https://medium.com/@1mikeowen/shallow-by-design-bf87d1a6bf67?source=linkShare-4cd140afefc2-1529614696)

* [Resources for Implementing European Legislation Identifier](https://eur-lex.europa.eu/eli-register/resources.html)













```
