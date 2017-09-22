## Week 9: 22-09-2017

### Community

[Dan](https://twitter.com/dasbarrett) met with [Rob](https://twitter.com/fryford), [Henry](https://twitter.com/henryjameslau) and [Frank](https://twitter.com/frankman1000) from the [ONS](https://www.ons.gov.uk/) data visualisation team thanks to an invite from [Oli](https://twitter.com/olihawkins). All great stuff.

### Parliament in the area, we're international, we're continental. But we're still south of Glasgow

Dan, Robert, [Graham](https://twitter.com/grahampeek) and [Michael](https://twitter.com/fantasticlife) met with [Rachel Prosser](https://twitter.com/rachelprosser) from the New Zealand department for internal affairs to talk about "machine readable legislation". There was vague trepidation that this might turn into some kind of Skynet thing with legislation poking out, [AR](https://en.wikipedia.org/wiki/Augmented_reality) style into the world. Like a Matrix but powered by nannies.

But the conversation quickly split into two chunks:

* that it's neither possible nor desirable to make all legislation legible to machines (given interpretation and case law and common law and the preference for being judged by humans please) *but* some basic regulations could probably be captured. Questions like, I would like to sell this type of thing, would I have to pay VAT? Also provenance between official regulations (like traffic speeds) and consumer end points (like sat navs) and what fuzziness exists in current gaps. Rachel's looking for the simplest thing in order to kick off some proof of concept work.

* that if all legislation can't and shouldn't be made machine readable, it should at least be made more legible to citizens. And indeed lawyers. At the moment you can be looking at one piece of legislation that's been revised by a second piece of legislation and possibly a third and etc and have no idea what changes have been made without also reading all the revising legislation. Talk turned to hypertext and [transclusion](https://en.wikipedia.org/wiki/Transclusion) as is our wont and the idea of revisions being included in revised documents via hypertext transclusion. Rachel mentioned that New Zealand has an Act that functions almost as a glossary of terms; when any piece of legislation says X it means this. The UK does not have such a thing. We also chatted about [registers](https://gds.blog.gov.uk/2015/09/01/registers-authoritative-lists-you-can-trust/) as a kind of definition file that could be linked to and transcluded into legislation.

It was probably the most interesting meeting of the week and we came up with a list of other people who would probably have good reckons: [Richard Pope](https://twitter.com/richardjpope), [Paul Downey](https://twitter.com/psd), [Libby Miller](https://twitter.com/libbymiller), [Jeni Tennison](https://twitter.com/jenit) and [Rachel Coldicutt](https://twitter.com/rachelcoldicutt).

On a similar theme, Robert spoke with a clerk in the Journal Office about how we might move from document-first to information-first publishing.

### One world, one web, one team

Dan continued to attend assorted agile [ceremonies](https://www.youtube.com/watch?v=Ss1MbL4NYf0) across the department. The main one this week was the technical difficulty vs value to users session led by [Colin](https://twitter.com/colinpattinson). Collective thinking is definitely developing but we still need to do some work to make sure 'work to be done' is aligned with the high level user needs that have been identified.

Dan also went to [Emma](http://twitter.com/_allenemma)'s website road map delivery meeting. The main decision was to open up [the new website](https://beta.parliament.uk/) to [search bots](http://www.robotstxt.org/robotstxt.html) and the corresponding need to commit to stable IDs in 'weeks' (said [Jamie](https://twitter.com/oddtype)). Dan is going to set up a meeting to explain why we can't really filter search results for our current web content.

### Domain modelling

Michael continued to investigate Oli's candidate database via the medium of prodding it with a Rails app. There's been some murmuring that this might come in the direction of the Data and Search team so we wanted to check [our data models](https://ukparliament.github.io/ontologies/) can cope. On Wednesday, [Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver) and Michael met with Oli to chat through the details of his relational database. Some changes were made to the [Election Ontology](https://ukparliament.github.io/ontologies/election/election-ontology.html) to capture a few things that were missing:

* Individual elections now have a [declaration time](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e245).

* A [Boundary set](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e431) class was added.

* Some existing predicates were reversed to make it more legible.

* [Constituency Group](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e499) was moved from between [Constituency Area](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e477) and [Electorate](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e535) when Oli pointed out that population stats are recorded on a completely different cycle to elections.

* [Recorded date](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e337) was added to [Population](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e594).

Michael and [Samu](https://twitter.com/langsamu) met with Colin and [Steve](https://twitter.com/steve_bromley) to chat through user needs and constraints for adding voting records to member pages on the new website. Plans were made to initially target professional users.

Michael met with [Ed](https://twitter.com/ewhitur) to chat about committee data and what we do next.

Anya, Silver and Michael met Angela to check our modelling of select committees against the data in existing systems. We think we've captured everything worth capturing in the Committee Office Database (used in the House of Lords to keep track of inquiries and evidence sessions). We still need to check against Red Book (used in the House of Commons for similar purposes).

Anya and Michael continued to revise the [first draft of the government department model](https://github.com/ukparliament/ontologies/blob/master/_government-department/government-department.png) with help from Chris Watson from the House of Commons Library. Michael also gave a quick presentation to the website team on where we're at with modelling government departments and positions and incumbencies and some of the data quality issues we're seeing.

Anya, Silver and Michael also spent some time tidying our slides for the [Euro IA conference](http://euroia.org/) next week.


### Data quality

There was a preliminary meeting with people from the Ordnance Survey on Thursday morning to talk through some of the problems we've been having around location data. Mainly the absence of Northern Ireland postcode data, some missing links between [NUTS regions](https://en.wikipedia.org/wiki/NUTS_statistical_regions_of_the_United_Kingdom) and constituencies, and [postcodes that span multiple constituencies](https://democracyclub.org.uk/blog/2017/03/20/4314-times-when-postcodes-arent-good-enough/).

### Data platform

Samu implemented content encoding in the API that sits behind the new website. Data travelling from the data service to the new website (and other public consumers) is now compressed, resulting in faster queries and an improved user experience.

Chris set up a local instance of [Webvowl](http://vowl.visualdataweb.org/webvowl.html) for use when the main site is down (which it frequently is).

[Jianhan](https://twitter.com/jianhanzhu) gave a presentation of his work on accessing on-premise databases from the data platform. He also created a spreadsheet of external website links for members and populated it with data from the web team. This will be ingested by the data platform and served to the new website (and beyond).

### Search

The search product team spent some time analysing and clustering the feedback gathered since search went live.

Robert helped with some new search ‘support’ issues. Most of his week was spent looking over the search feedback, being told how to do that and then that happening. There was a lot of comment and analysis.

### Machines that do learning

[Raphael](https://twitter.com/raphaelleung) (and a bit of [Ben](http://twitter.com/benwoodhams)) went along to [THINK AI for the Public Sector](http://www.thinkdigitalpartners.com/event/think-ai-publicsector/). Michael poured some scorn.

### Measuring things

Liz showed a first draft workload report to one of the heads of section in the House of Commons library. The data is pulled out of the library enquiry service, automatically refreshing on a schedule via a gateway 8 times a day.

Sara published a report on Search API performance. She also met with Lopa to discuss performance analytics and to make sure the data and search team can access beta and current website datasets.

Tags have now been added to the website to track specific events (for example people choosing to revert to the old search). With these in place we can now follow individual user journeys.

### Excellent customer service awards

After spending a part of last week helping a political science PhD student from the [Federal University of Minas Gerais](https://en.wikipedia.org/wiki/Federal_University_of_Minas_Gerais) get data on gender representation in the House of Commons, Mike received a note to say, "You have no idea how much time and money you've saved me - I really can't thank you enough." Thanks also to the usual expert help from Joe Foster.

### Capability

Robert went along to [Julie](https://twitter.com/julietouring)’s capability reboot session which was much easier to understand than the search analysis. Especially thanks to the new improved Trello setup.

He also attended an Inclusive Recruitment Masterclass all day on Wednesday.

### Corporate data

Dan met with Rupert, king of the architects, to talk about getting a new architect for our internal, 'corporate' data work - what we do over the coming years and things of that nature.

### Did anybody say blockchain?

One person said blockchain ¯\_(ツ)_/¯

### Strolls

No strolls were reported. Stroll harder. Stroll smarter. Be cold, if not bold.

### Things that caught our eye

* [The Open Data Institute on why we need the Data Ethics Canvas](https://theodi.org/blog/why-we-need-the-data-ethics-canvas)

* [Knowledge and the Shock of Hypermedia: Thoughts From ISKO UK 2017](https://16blue.me/2017/09/18/knowledge-and-the-shock-of-hypermedia-thoughts-from-isko-uk-2017/)

* [That tweets may have enough indication of your mental health conditions isn't scary at all](https://www.aclweb.org/anthology/E/E17/E17-1015.pdf) [PDF]

* [Let's fund teams, not projects](https://defradigital.blog.gov.uk/2017/09/19/lets-fund-teams-not-projects/)