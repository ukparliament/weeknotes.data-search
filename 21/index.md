## Week 21: 15-12-2017


### Dator day

Wednesday was data day. The first half was a bit tough but we burnt through the [agenda](https://twitter.com/dasbarrett/status/940990081741082625) in the afternoon. This appears to be a theme. Maybe skip mornings?

Anyway, lots of variety and steady progress on most fronts. It was agreed that our top development priorities at the moment are:

* Getting committee data from the Members' Names Information Service (MNIS) into the data service.

* Getting question and answer data into the data service.

* Migrating [data.parliament.uk](http://www.data.parliament.uk/) to the cloud.

And some other notes:

* Pages for government departments / organisations / answering bodies are still necessary and a precursor to lots of other potential linkages.

* Data and Search work for opposition roles has been done.

* Early day motions look like a possible candidate for modelling next.

* Our investigative work to see how deposited papers might appear in web search yielded slightly odd results. Further investigation is needed.

### Corpcomms

It was the night before Christmas and nothing did stir, except for the bloke who was trapped in Yammer.

### Community

[Ben](https://twitter.com/benwoodhams) did some (very belated (sorry)) video editing from the last [Newspeak](https://www.nwspk.com/) event. He's planning to start editing the vids from our trip to [ODI Leeds](http://leeds.theodi.org/) shortly. They should all be ready to go live about the same time. Sadly.

### Excellent customer service badges...

...once again go to Mike who we're fairly sure got another thank you from another PhD student. It would be a disappointing week if he didn't.

### Domain modelling

[Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver) and [Michael](https://twitter.com/fantasticlife) met with [David Beamish](https://en.wikipedia.org/wiki/David_Beamish) to idiot / sanity check some of their modelling work around [house membership](https://ukparliament.github.io/ontologies/house-membership/house-membership-ontology.html), [elections](https://ukparliament.github.io/ontologies/election/election-ontology.html), [political blocs](https://ukparliament.github.io/ontologies/political-bloc/political-bloc-ontology.html), [formal bodies](https://ukparliament.github.io/ontologies/formal-body-affiliation/formal-body-affiliation-ontology.html), [tabling](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html), and [questions and answers](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html). No major quibbles were raised and the sanity box was largely ticked. The tabling model still needs more work. Supplementary oral questions also need modelling. But not before Christmas.

### Are Lords inflated?

The Lords are now mostly inflated (still really don't ask). Ben has some work to do around giving non-"great see" bishops individual seats linked to incumbencies rather than bishoprics. A note to clarify that this will never include the [Bishop of Man and Sodor](https://en.wikipedia.org/wiki/Bishop_of_Sodor_and_Man). Unless you're playing widdershins. I did say don't ask.

In practical terms, it means we should shortly see lists of Peers present in [previous Parliaments](https://beta.parliament.uk/parliaments). We still need to work on 'incumbency interruptions' to fix the 'wrong number of Lords' problem. And finally do the people names thing properly.

On the subject of Peers, Ben spent most of Monday to Wednesday as the official Peer Wrangler for their photo sessions. Photos should be flowing into the platform and out to the web fairly soon. [Creative Commons](https://creativecommons.org/) licensed as ever. Fill your boots.

### Data platform

[Jianhan](https://twitter.com/jianhanzhu) continued to work on the data platform [OData](http://www.odata.org/) API service. This has now been deployed and can be used to explore our data via an assortment of tools from Excel to web browser. Like much else, the [code is now on GitHub](https://github.com/ukparliament/OData).

[Samu](https://twitter.com/langsamu) has been working with Jenna and [Jamie](https://twitter.com/oddtype) from the website team to integrate content publishing into the data platform. There's now code deployed on staging to get blobs of content from a [headless CMS](https://en.wikipedia.org/wiki/Headless_CMS) and make them available through standard data platform APIs. [Chris](https://twitter.com/chrisalcockdev) helped out by getting the CMS vendor to fix a bug in their API. 'Content' should start to appear on beta.parliament shortly.

Matthieu finished performance testing the database cluster. We're told it's now performing like lightning. A report in the form of a [post is on our blog](https://pds.blog.parliament.uk/2017/12/15/performance-testing-a-graph-database/). Not this one; our other one.

### data.parliament migration

We made decent progress on migrating data.parliament from its current hosting environment to the new one. As soon as some network changes get made, we can go live.

### Parliamentary material search

After two weeks of testing and trying different things (with help from Samu, Wojciech and Mike) [Alex](https://twitter.com/alexedwardh) now has a cool system in place to automate [Solr](http://lucene.apache.org/solr/) queries and notify users based on results. These queries are usually used to search for inconsistencies and errors in data that can then be fixed, but they're currently being carried out manually by [Phil](https://twitter.com/philbgorman) on a daily / weekly basis. Which is time consuming. There are now 7 automated tasks set up which run the queries daily then send out emails or create calendar events to alert users depending on what results are returned. A lot may be tweaked in the future including the methods of notification. But it's a good starting point that can be further built on and improved.

### Measuring things

We've got pretty bored with measuring things. Instrumentation is dead to us. Just running on pure instinct here. And raw talent. And [hypertext](https://en.wikipedia.org/wiki/Hypertext).

### Corporate data

[Dan](https://twitter.com/dasbarrett) wrote a paper for David (our Deputy Director) and [Emma](https://twitter.com/_allenemma) about a new approach to 'corporate' data in 2018.

### Capability

[Aidan](https://twitter.com/aidan_morgan) met with Samu, Michael and Anya to put together job descriptions for the new positions due to be advertised early in the New Year. Do check back later if you fancy being a developer or a data architect or just a person who helps make web things. Preferably the latter.

### Did the machines learn owt?

We're slowly coming to the conclusion that they may have a different learning style to that provided by more traditional education. Or they're dumb as rocks. One or t'other.

### Did anyone say blockchain?

Alex fooled almost everyone by [saying cryptocurrency but definitely not saying blockchain](https://www.technologyreview.com/s/609771/a-cryptocurrency-without-a-blockchain-has-been-built-to-outperform-bitcoin/). Well played Alex.

### Strolls

Dan and Robert took a stroll and had lunch. Ben and Robert also went strolling and drank coffee. Ben smoked fags. To no-one's surprise, Robert didn't.

Robert and Michael did less strolling and more eating, stopping off at [Coleman Coffee Roasters](http://wearewaterloo.co.uk/business/coleman-coffee-roasters) for plates of oatcakes and cheese. Other purveyors of oatcakes may be available and just as good. Seems unlikely.

### Fresh! Baby! News!

Kunal celebrated the arrival of a baby girl. Next stops: school and work. It doesn't get better, kid.

### First Noel

In which our Noel got named as [Hillingdon's Special Constable of the year](https://twitter.com/mpshillingdon/status/941655113835401216). Result. \o/

### Things that caught our eye

* [SPARQL / OData Interop](https://www.w3.org/2013/04/odw/odw13_submission_4.pdf) [PDF]

* [OData2SPARQL: Consuming SPARQL/RDF with OData RESTful interface](http://inova8.com/bg_inova8.com/odata2sparql-consuming-sparqlrdf-with-odata-restful-interface/)

* [OData: Is it the universal query language for RDBMS, RDF, and other datastores?](http://inova8.com/bg_inova8.com/odata-is-it-the-universal-query-language-for-rdbms-rdf-and-other-datastores/)

* [Estonia, the Digital Republic](https://www.newyorker.com/magazine/2017/12/18/estonia-the-digital-republic)

* [Semantic web: time for pragmatism rather than zealotry?](http://inova8.com/bg_inova8.com/semantic-web-time-for-pragmatism-rather-than-zealotry/)

* [Visual Studio Tools for Artificial Intelligence](https://www.visualstudio.com/downloads/ai-tools-vs/)

* [Covertband: Activity Information Leakage using Music](http://musicattacks.cs.washington.edu/)