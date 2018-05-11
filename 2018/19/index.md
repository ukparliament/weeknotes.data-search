## 2018 Week 19

### More visions

[Samu](https://twitter.com/langsamu), [Matthieu](https://twitter.com/cognithive), Mike, [Aidan](https://twitter.com/aidan_morgan), our Liz, [librarian Liz](https://twitter.com/greensideknits), librarian Steve, other librarian Steve and librarian [Anya](https://twitter.com/bitten_) sat in a room in Tothill Street and had visions about the work of the House of Commons Library Indexing and Data Management Section and what we need to build to help them and more importantly to help Parliament. They were joined intermittently by [Michael](https://twitter.com/fantasticlife), [Jamie](https://twitter.com/oddtype) and [Matt](https://twitter.com/mattrayner). [Dan](https://twitter.com/dasbarrett) came onstage for a fiery encore. There was a summary of all that was said, which was surprisingly uncontentious and very linked to Dan's own vision of the data strategy. Which is still brewing. Lots of words were written.

Dan continued to have visions. He met quite a few people to talk all things data strategy and gave a talk to the Data Steering Group. Total Capitals. Really Important People. He also talked with colleagues from [DCMS](https://www.gov.uk/government/organisations/department-for-digital-culture-media-sport) about some cross-governmental work with international potential. In a roundabout way, it revisits the stuff we said we'd do on [registers](https://gds.blog.gov.uk/2015/09/01/registers-authoritative-lists-you-can-trust/) a while back.

### Liberating the library

Way, way back last November, before the sun had even risen, Anya, librarian Liz, Robert and Michael [took a trip to Cambridge](https://twitter.com/bitten_/status/931552786671472640) to chat to [Andrew Gray](https://twitter.com/generalising) about matching the [House of Commons Library thesaurus](http://www.data.parliament.uk/dataset/thesauri) to [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page). A plan was hatched to export enough data from Search and Indexing to allow Andrew to auto-match subject headings to Wikidata things. Unfortunately, despite best efforts, the split between our vocabulary management system and our subject indexing system(s) made it somewhat harder than expected for [Alex](https://twitter.com/alexedwardh) to export the right data. Finally, last week, he managed it and popped the lot in a Google spreadsheet. Which promptly crashed Michael's browser. So the [data is now on GitHub](https://github.com/alexedwardh/TermUsage/blob/master/OUTPUT.CSV), should it be of interest. Anyway...

...Andrew has now grabbed the data and ran it through the [Wikidata mix-and-match tool](https://tools.wmflabs.org/mix-n-match/?#/catalog/1229). It managed to auto-match around 4000 of the 41,686 concepts which are now sitting around, waiting for human approval before being imported into Wikidata. Andrew says:

> As of now 1858 (4.4% of the total) have been confirmed by hand and are in Wikidata. Another 4181 (10% of the total) auto-matched and are waiting to be manually confirmed and pushed to Wikidata.

> I've quickly skimmed the automatched ones and they look reasonably good - probably about 80-90% of them are correct matches, with the rest being homonyms of one kind or another. But it should be fairly quick to sort through.

Andrew also says:

> One unexpected benefit is that I've been able to use it as an authority list for things like regional tourist boards and NHS health authorities. We had entries for two or three of them but crosschecking against the thesaurus meant we could very easily create the remainder in a few minutes. So we're definitely getting some benefits from it as well at this stage.

The medium term plan at the Parliament end is to make public URIs at id.parliament.uk/concepts/:concept and link out from there (with something a little like [foaf:focus](http://xmlns.com/foaf/spec/#term_focus)) to Wikidata. And change the links in Wikidata to point to the new URIs. And allow users to look up House of Commons concepts via a Wikidata ID, something like beta.parliament.uk/concepts/lookup?source=wikidata&id=Q7416. And finally, actually expose the subject indexings of parliamentary material to the web. So you can go from a Wikidata thing to see what Parliament has said about it. Native to a web of data, as they used to say.

We'd like to thank Andrew and apologise for how long this has taken. And thank [Tom](https://twitter.com/tommorris) who's also been [beavering away](https://twitter.com/tommorris/status/994668681752862721), sense checking the matches. If you're a Wikipedian and would like to chip in, all help appreciated.

### Showing and telling

Matthieu was joined by librarian Liz, from the Indexing and Data Management Section in the House of Commons Library, to talk about our experiments with [VocBench](http://vocbench.uniroma2.it/), a vocabulary management tool with a [SKOS](https://en.wikipedia.org/wiki/Simple_Knowledge_Organization_System)-y, web-based workstream. They’re both pleased at how well working together has gone, and they even managed to make improvements to the vocabulary whilst preparing their presentation. Matthieu thinks [SPARQL](https://en.wikipedia.org/wiki/SPARQL) is a really powerful and versatile tool. Apart from performance concerns over some long-running queries (think 1-5 seconds), it's all [blue skies ahead](https://www.youtube.com/watch?v=aQUlA8Hcv4s).

Combining both vocabulary management and Wikidata, Michael and Matthieu have started a chat about adding Wikidata identifiers to subject index concepts via VocBench. We [form much like Voltron](https://www.youtube.com/watch?v=2kkJDHRYxWM).

### Community

Samu put together [a summary of our work so far](https://medium.com/@langsamu/api-parliament-uk-7b87597019a4), primarily for sharing with [Stephen Betts](https://twitter.com/stephenbetts) from the [NYPL](https://www.nypl.org/).

Our Liz, [Sara](https://twitter.com/sarafreis), Matt R, Dan, Matthieu, Aidan and Raphael had a call with David Sullivan from the [ONS](https://www.ons.gov.uk/). Davis talked about his work on training a machine learning algorithm to link keywords through [dimensional vectors](https://en.wikipedia.org/wiki/Dimensionality_reduction). Or, to put it another way, augmenting the ONS search with additional keywords so that relevant content is returned, without exact word matching. Apparently people search for murder instead of homicide. Who knew? It's good work with some interesting data to be shared.

Michael went along to a meeting with the [Statutory Instrument](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) product team and Claire Harvey from [the National Archives](http://www.nationalarchives.gov.uk/) to chat about assorted flows for SI data. Some talk of interlinking Parliament pages with [legislation.gov.uk](http://www.legislation.gov.uk/) pages happened.

On Thursday there was another meeting with the National Archives, [GDS](https://gds.blog.gov.uk/) and assorted government department people, also on the subject of SIs. Jane, Jack, [Jen](https://twitter.com/benwoodhams), Janya and Jichael went along. Jenna and James were elsewhere. Much paper was handed out. There were agenda items. Like a proper grown up meeting. More talk of interlinking happened.

### Domain modelling

Anya, Michael and [Silver](https://twitter.com/silveroliver) spent part of Thursday taking a second look at their [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) and how it might link to [work packages](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e284) in the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html). Until they realised they'd already done that work in the [formal body](https://ukparliament.github.io/ontologies/formal-body/formal-body-ontology.html) model, linking a workpackage to legislation via a [focus](https://ukparliament.github.io/ontologies/formal-body/formal-body-ontology.html#d4e319). They did tidy up some of the legislation model, though Michael still thinks it looks wonky / broke. More work needed.

### Data platform

[Jianhan](https://twitter.com/jianhanzhu) has continued work on ingesting written [parliamentary questions](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) into the data platform. He had been trying to grab source data from the Electronic Questions and Motions system. Yes, that is *Electronic* Questions and Motions. There is no steam power here. Unfortunately he ran into several problems en route::

* It only contains recent questions and not the 1.5 million we have in our computational systems.

* It doesn't have questions asked in the House of Lords.

* It doesn't have all the data added by IDMS such as question titles and indexing fields.

* It has a non-unique [UIN](https://en.wikipedia.org/wiki/UIN) rather than a unique [URI](https://en.wikipedia.org/wiki/Uniform_Resource_Identifier). And if you're playing along at home, you'll know names are not identifiers.

Given all this, Jianhan has now switched efforts to ingesting data from the [Solr](http://lucene.apache.org/solr/) index. Which presents its own problems. Member and answering body identifiers from the [Members Names' Information Service](http://data.parliament.uk/membersdataplatform/memberquery.aspx), which are present in source systems, are stripped out in Solr which only has Term IDs (the identifiers used in the controlled vocabulary discussed at some length above). Fortunately these are mostly mapped to MNIS IDs except...

...where hereditary Peers exist, they have multiple MNIS IDs but share a single Term ID. In order to know which particular Lord Featherstonehaugh the question was asked by, we need to compare when they were in the House of Lords with when the question was asked. So Jianhan has written a SPARQL query to disambiguate Peers, using their [parliamentary incumbency](https://ukparliament.github.io/ontologies/house-membership/house-membership-ontology.html#d4e312) start and end dates, and the [tabling date of the question](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html#d4e123).

65,481 written questions from the past year have now been ingested, of which 21,075 have a title. This is good enough for the web team to work with for now. Getting all 1.5 million written questions into the data platform will be a challenge, since getting just a year's worth has clogged up our ingest pipes. Jianhan's now planning to turn his attention to corrections to answers. He's currently ingested 583 corrections which link to a previous written answer. 

To support Jianhan’s work, [Chris](https://twitter.com/chrisalcockdev) has been making changes to the physical ontology to reflect question URIs as their unique identifiers, MNIS things having Term IDs, corrections etc.

Following on from Matt's recent pull request to the [Application Insights SDK for Ruby](https://github.com/Microsoft/ApplicationInsights-Ruby), we're now reporting logs from the beta website into our analytics. On the search side, we're joining individual requests to the API with individual requests to the website to get an overview of the full stack. There are plans to extend this across all pages on the [beta website](https://beta.parliament.uk/) in the not too distant future.

On the [data.parliament](http://www.data.parliament.uk/) front, we took our first tentative steps toward making our operational data publicly available. Mike has created an app that logs downtime and pipes it to a [public calendar](https://calendar.google.com/calendar/embed?src=4emj2l2b2q1tmp7jga0nmhrdf0%40group.calendar.google.com). You can now subscribe to our mistakes.

### On searching and indeed indexing

Alex has been working to add some smarts to the pipes that shunt data from the Search and Indexing triplestore (where the librarians subject index parliamentary materia) to the Solr instance that powers [parliamentary search](http://search-material.parliament.uk/). Previously the piping code would run irrespective of whether content had been added or not. Including during [recess](https://www.parliament.uk/site-information/glossary/recess/). Now it doesn't bother executing if no new content has been added. Which saves on files created and compute. He thinks someone should perhaps have made it work like this from the start.

### Corporate data

Lewis has been using our business analytics solution to create a proof of concept that shows we can save on data duplication by switching a reporting data source from SharePoint to Excel. Did I just type business? And analytics? And solution? I’m just going with what Wikipedia says here.

Noel has been analysing the people records that are placed into the 'Unknown' organisation structure and has developed a process to better identify the correct organisation for the records.

### Excellent customer service award…

...again has joint winners, as both Raphael and Mike grabbed an issue raised in the [data@parliament.uk](mailto:data@parliament.uk) inbox and ran with it. Thanks were offered from an MP and a bunch of academics in Oxford town. Not that [Oxford town](https://www.youtube.com/watch?v=W9oJZX4BaI8). The other one.

### Joiners and leavers

This week we welcomed [Matt Reed](https://www.linkedin.com/in/matthew-reed-b3b761105/), occupying a data analyst spot in our Liz's team. Nobody left. At least if they did, nobody told me.

### Things that caught our eye

We've been so busy we've barely noticed anything, but Matthieu did read [Tom Steinberg](https://twitter.com/steiny)'s piece about [why anyone might want to bother with user-centered digital government](https://civichall.org/civicist/why-even-bother-with-a-user-centered-digital-govt/). It's good. But we do point out we're not government. We're kinda like the opposite of government to be honest.