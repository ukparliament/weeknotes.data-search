## 2018 Week 27


### Dator day

Wednesday was [data day](https://twitter.com/dasbarrett/status/1014490065274318851). Which is now half a day. Your author was dying of heat exhaustion in Sheffield so couldn't go. And nobody wrote a summary, so I can't say what happened. [Dan's ticks](https://twitter.com/dasbarrett/status/1014542579289985030) may hold some clues.

I do know that Connie and Angus (information architects and ex-colleagues of [Alison](https://twitter.com/oliala) at [NICE](https://www.nice.org.uk/)) came along. And that they discussed search and associated challenges. And some potential approaches to introducing a more structured approach to data in large and complex organisations. Thanks Connie and Angus!

### Parliament in the area, [we’re international, we’re continental](https://www.youtube.com/watch?v=pNfHoPIxhXM&t=1m9s)

On Friday, [Anya](https://twitter.com/bitten_), [Samu](https://twitter.com/langsamu), [Michael](https://twitter.com/fantasticlife) and Robert (who is of the internet but not on the internet) had a phone chat with the [Scottish Parliament](http://www.parliament.scot/) about taxonomies and subject indexing and search and building websites. And, erm, user needs. Unfortunately a can of beer exploded in Michael's bag which distracted him somewhat. So he has no idea if anything was agreed. The bag seems to be recovering though.

### Community

Alison went along to [Teacamp](https://teacamplondon.com/2018/07/03/july-teacamp-brexit-and-the-national-archives-with-johnlsheridan/) where [John Sheridan](https://twitter.com/Johnlsheridan) gave a very informative talk on the duties of the [Queen's Printer and Keeper of Public Records](http://www.nationalarchives.gov.uk/about/our-role/executive-team/jeff-james/). He also spoke about what the [European Union (Withdrawal) Act 2018](http://www.legislation.gov.uk/ukpga/2018/16/contents/enacted) sets out with regard to publishing legislation (note 'publishing', not 'printing' here), and some of the user needs around this (legislation relevant to UK, provenance etc). John highlighted the excellent working relationship he's built up with counterparts at [EUR-Lex](https://eur-lex.europa.eu/homepage.html?locale=en), the challenges of mapping from EU legislation templates to UK ones and how the resultant EUR-Lex archive on [legislation.gov.uk/](http://www.legislation.gov.uk/) is the envy of EUR-lex for the different ways in which the legislation can be searched and viewed. He also talked about [statutory instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) and praised our [SI tracker service](https://beta.parliament.uk/statutory-instruments) and the speed with which it was built.

### One world, one web, one team

Our Liz caught up with [Trine](https://twitter.com/StealthGeekUK) to talk through the survey guidance she's working on. They talked about the 'ways of working' survey data that Liz has been munging into a shape that makes it easy to build consistent graphs. The main themes they covered were:

* Including questions about analysis methods and presentation before designing as they might influence scale and point on the scale.

* How to aggregate data to cope with expected low response rates.

* The importance of testing the output for spelling errors etc. before doing it for real to reduce data cleaning later.

* Aiming for measurable behaviours rather than high level mood assessment to reduce the room for interpretation and current mood influencing the answer given.

They picked out many more specifics to support the key messages in the guidance. Liz is planning to put Trine in touch with Katy from the 'ways of working' programme. She thinks it would be nice to develop and validate the guidance with people outside the [Parliamentary Computational Section](https://pds.blog.parliament.uk/).

### Domain modelling

Anya and Michael escaped the world of [procedure and flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples) and took a trip to the People's Republic of Sheffield to visit [James](https://twitter.com/jamesjefferies). They have a bit of side project with the [History of Parliament Trust](http://www.historyofparliamentonline.org/) to put data related to the social background of Members of the House of Commons on the web. The data has been collected and analysed by [Professor Michael Rush](https://socialsciences.exeter.ac.uk/politics/staff/rush/) over a number of decades. Some of it is in Access, some of it is on bits of card. The plan is for James to build an application to expose and edit the data, the History of Parliament Trust to take over the maintenance of the application and Anya's team in the House of Commons Library to take the stuff that's currently on cards and explain it to computers. The latter part is intended to happen during the quieter periods of summer recess but James isn't due to start work until autumn. So Michael’s made lots of linked spreadsheets to hold the data until James is ready. Once Anya showed him how. It was, as ever, lovely to see both James and Sheffield.

On Thursday, Anya and Michael went to visit the team working on [Research Briefings](https://researchbriefings.parliament.uk/) to talk through progress with the [domain model](https://github.com/ukparliament/domain-models/blob/master/document/document.pdf). So far they've split out a bit of a model to deal with [publishers](https://ukparliament.github.io/ontologies/publisher/publisher-ontology.html) and a bit to deal with [contributions](https://ukparliament.github.io/ontologies/contribution/contribution-ontology.html) (though this needs work). They still need to do the actual document bit.

### Data platform

With [Historic Hansard](https://api.parliament.uk/historic-hansard/index.html) now folded into the rest of [Hansard](https://hansard.parliament.uk/), we can start to point users to that and begin to plan for the decommissioning of the [hansard.millbanksystems.com](http://hansard.millbanksystems.com). Hopefully [via the medium of redirects](https://gds.blog.gov.uk/2012/10/11/no-link-left-behind/).

### On search. And indeed indexing

[Sara](https://twitter.com/sarafreis) has been looking at matching search terms used on the Parliament website with concepts from the Indexing and Data Management Section's [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri) in the hope that we'll better understand any 'language barrier' between website users and Parliament. For the period between 1st and 7th April 2018:

* 661 concepts were used by IDMS to index parliamentary material.

* 8321 unique search terms were used in website search.

* 40% (265) of concepts used that month matched a search term.

* 24% of search terms matched a concept.

Which doesn't seem to account for people searching for things outside that month. But I can't be sure.

Sara, Liz and Matt met to discuss their analysis of search hints, and to look into how we can provide maximum URL coverage with a minimal number of hints. While we have a list of over 1000 unique hints, we can provide a hint to over 97% of search results with only 60ish hints.

### Strolls

Way too hot for strolls again this week. Although Friday was Raphael's leaving do. So the Data and Search team headed to [St James's Park for a picnic](https://twitter.com/dasbarrett/status/1015231618523566081). Goodbye and good luck Raphael.

### Things that caught our eye

* [From inboxing to thought showers: how business bullshit took over](https://www.theguardian.com/news/2017/nov/23/from-inboxing-to-thought-showers-how-business-bullshit-took-over)

* [Toxic Technology: the growing legacy threat](https://medium.com/@daverog/toxic-technology-the-growing-legacy-threat-b95ad098a339)

* Dan read [Use the tools that you need to do good work](https://digital.canada.ca/2018/06/27/tools-to-do-good-work/) and dreamed of Canada

* [Local Digital Declaration](https://localdigital.gov.uk/declaration/)

* [Digitising health statistics](https://stacks.wellcomecollection.org/1-million-tables-and-counting-7e7e6c9f76e)