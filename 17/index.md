## Week 17: 17-11-2017

### [Leave the Capitol](https://www.youtube.com/watch?v=GpMoRS_9bcM)

Another reminder that our [5th Parliament, data and democracy meetup](https://attending.io/events/parliament-data-and-democracy-meetup-5) is on Wednesday 6th December, this time at [ODI Leeds](http://leeds.theodi.org/).

Speakers lined up are our [Dan](https://twitter.com/dasbarrett), [Cristina Leston-Bandeira](https://twitter.com/estrangeirada) (Professor of Politics at the University of Leeds), [Tom Forth](https://twitter.com/thomasforth) (Head of Data at ODI Leeds) and [Edward Wood](https://twitter.com/edwardwood99) (Director of Research in the House of Commons Library).

More in the way of interesting talks, nice people and [free beer](https://en.wiktionary.org/wiki/free_as_in_beer). Come along. Bring a friend.
 
### Community

On Wednesday [Anya](https://twitter.com/bitten_), [Liz](https://twitter.com/greensideknits), Robert and [Michael](https://twitter.com/fantasticlife) took a trip to Cambridge to meet [Andrew Gray](https://twitter.com/generalising). They plotted and sketched on how we might align the [Parliament Thesuri](http://www.data.parliament.uk/dataset/thesauri) to [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) concepts. There is now a plan to give Andrew a spreadsheet of the thesauri ID(s), the preferred term, any scope notes, the class of the thing (person, organisation, something else), any non-preferred terms and the number of times the concept has been used to tag content. Andrew will then run an auto-match script against Wikidata and Liz and team will check and add Wikidata identifiers against our taxonomic concepts. Andrew will then take approved matches and add Thesauri IDs to Wikidata.

They also spoke about longer term plans to map non-taxonomic Parliamentary things to Wikidata. Eventually we'd like to see Wikidata carrying identifiers and linking to Parliamentary concepts (taxonomic and non-taxonomic), the Parliament website publishing [sameAs](http://schema.org/sameAs) links to Wikidata, and users able to lookup Parliamentary things from Wikidata IDs (see the [lookup url pattern here](https://github.com/ukparliament/ontologies/blob/master/urls.csv)). It will all help to make the Parliament website and data more interlinked and more interoperable with the wider web. And in a spirit of enlightened self-interest, establishing equivalence between Parliamentary things and Wikidata things will couple us to the [Google Knowledge Graph](https://en.wikipedia.org/wiki/Knowledge_Graph) which uses Wikidata for descriptions of core concepts. So Parliamentary material should be more discoverable via web search. At some unspecified date in the future. Given we're making a website and not a CD-ROM, this is a good thing.

On Tuesday Anya, [Silver](https://twitter.com/silveroliver), [Samu](https://twitter.com/langsamu), [Chris](https://twitter.com/chrisalcockdev) and [Raphael](https://twitter.com/raphaelleung) met with [Jonathan](https://twitter.com/jonathantweed) and [Alice](https://twitter.com/superprotta) from the [Wellcome Trust](https://wellcome.ac.uk/), [Nicholas](https://twitter.com/njh) from the BBC and [Andy](https://twitter.com/mr_dudders) from the [ONS](https://www.ons.gov.uk/). They chatted about publishing open data in general, about [JSON-LD](https://en.wikipedia.org/wiki/JSON-LD) in particular, and about spotting publishing patterns even where the underlying technology is very different.

Dan committed the team to looking at [Deposited Papers](https://www.parliament.uk/depositedpapers) after some [constructive criticism](https://twitter.com/owenboswarva/status/929715010498125825) on social media from [Owen Boswarva](https://twitter.com/owenboswarva).

[Aidan](http://twitter.com/aidan_morgan) met with Ed Ricketts to talk about planning for future external events.

Chris and Raphael wrote a post about our [recent trip to Open Data Camp in Belfast](https://pds.blog.parliament.uk/2017/11/15/open-data-camp-in-belfast/). It's good, you should read it.

### Corpcomms

Dan and [Julie](https://twitter.com/julietouring) would like it to be known they're putting more effort into Yammer. I don't know either.

Julie also spent some time with Ed Ricketts talking about the engagement strategy around everything we do in Development.  Which was apparently interesting.

And [Dia](https://twitter.com/DN78) met the same Ed to discuss where we can take the data 101 presentation around Parliament.

### One world, one web, one team

In Ceremony Watch (TM) Dan, Aidan and Michael went to assorted stands up for the assorted bits of the website. [Pazuzu](https://en.m.wikipedia.org/wiki/Pazuzu) remained un-summoned.

Aidan continued to attend stand-ups with the Hybrid Bills team so future features requiring work by Data and Search could be understood earlier. The main collaboration between teams currently centres upon Committee types, associated staff rosters and setting up interim data sources to hold the required information.

Dan met with Bryony, Callum, and Jenna from the Members' activity website product team to talk about existing data and systems. Robert also met with them to chat about the [They Work For You API](https://www.theyworkforyou.com/api/). And related matters. It says here.

On Thursday Chris, Mike, and Wojciech also met Jenna and Bryony to discuss Members' activities discovery work.

Team:Samu worked with the Business Systems team to help them launch a new application. Mike made sure the data is correctly structured and that all the data pushing and pulling from the new system into [data.parliament](http://www.data.parliament.uk/) and our Indexing and Search application is correct.

Aidan spent his first day sitting with the Indexing and Data Management Section in the House of Commons Library. He's planning to work there for a day a week helping to plan future.

Aidan also did some procurement stuff. Which is what business people call buying things. Although it seems to be harder for business people than normal people. Oddly.

### Domain modelling

Anya, Silver and Michael continued to peer at questions and answers. What was a written question and answer model for Parliamentary Questions is now an attempt to cover both [oral and written PQs as well as urgent questions and business questions](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html). It still needs idiot / sanity checking.

### Data platform

On Wednesday Samu met with [Jamie](https://twitter.com/oddtype) and [Matt](https://twitter.com/mattrayner) for a technical meeting with a vendor we're assessing for providing content management as a service to the new website. Jamie led the discussion with the vendor's solution architect. Samu thinks it's looking really good and he's excited about integrating 'content' to our data offering.

### Search

We went live last week with the migrated search systems which were shifted from our old cloud provider to our new one. We took advantage of the opportunity to, where possible, move to [PaaS](https://en.wikipedia.org/wiki/Platform_as_a_service) solutions such as containers. We also updated web servers, operating systems, etc.
 
The move is showing cost savings of over 90%. Which is not to be sniffed at. We were also surprised by the performance improvement, which stands at around 2-3 times as fast. We now have control over things we previously didn't such as networking and security, and have access to metrics and monitoring which means we can pursue things like automated solutions to common problems.

Alex, Mike and Samu spent some time investigating an error report for Parliamentary Search (a search service available to internal users only) where searching between two dates ignores the 'from' part of the date filter. Making it half-useless. Unfortunately they couldn’t find any quick workarounds or hacks so they queried the index directly and exported the search results for the user as a short term fix. Samu realised that it would be possible for us to create something to query the index as a longer term workaround.

On Monday PDS hosted the Product People event. Dia presented the new website search and demoed the [dungerous doogs](https://beta.parliament.uk/search?q=dungerous+doogs) query. It went well.

Liz presented her work analysing search feedback at the Data and Search show and tell. Dia gave an introduction. There were some good questions that prompted discussion around how the analysis will be used with other testing (A/B testing) and API / performance analytics.

Raphael met with [Laurence](https://twitter.com/laurencegrinyer), [Franny](https://twitter.com/eff_shaped), and Joe from the search product team to discuss hints. He answered questions around some of the technical constraints and checked with Samu, Matt, Uzman and Robert before deploying hints to both branches of the Search API. It all works as expected and nothing's broken. At least nothing that anyone's noticed. Search hints should be surfacing on the website fairly soon.

Robert caught up with Dia, went to a search team retrospective and sprint planning, and met with the Content team to work out how we work with the new search console. Or whatever it’s called. Robert's Massive Dell was not running Windows 10 and apparently wanted to be. Some time was spent watching cogs turn. In other technology related news we repeatedly lost part of the internet.

Michael continued to chummer that the best way to improve search is to spend the time making the right [resources addressable](https://en.wikipedia.org/wiki/Web_resource) and improving browse and [crawlability](https://en.wikipedia.org/wiki/Web_crawler). He has a strong feeling that the search roadmap and the browse roadmap need to be better aligned because they are not different things.

### Measuring things

Robert went along to an introduction to research methods session run by Franny. He strongly believes in life-long learning.

Saffiyah did some work in our new analysis tool looking at downloads for search sessions and some other parameters. She also met with Joe Foster to discuss the House of Common Library Enquiries database.

Matthieu took Aidan through the dashboard they've built to monitor billing for our cloud hosting. Aidan can now grab information to help with financial management and play around with creating his own dashboard views. Aidan wins a Dashboard Stage 1 badge and a Linked In endorsement for putting graphs on tellies.

### Snoopware

Conversations on the subject of analytics and privacy continued over email. Michael snowballed the cc list. Thanks to [Max](https://twitter.com/emax), [Ben](https://twitter.com/benwoodhams), [James](https://twitter.com/floppy), [Reuben](https://twitter.com/rdbinns), [Tony](https://twitter.com/psychemedia), [Mischa](https://twitter.com/mischat) and [Kate](https://twitter.com/kateahoc) for useful thoughts. This still feels important.

Anya and Michael went to visit [Nayeema](https://twitter.com/nayeemac) at the Department of Health to talk some more about analytics and user privacy. [Tea and cake](https://twitter.com/fantasticlife/status/931495661492686848) was served. Advice was sought and supplied. Thanks Nayeema.

### Machines that do learning

Young and dumb. We've got nothing here.

### Did anyone say blockchain

Nope. Or not in my earshot.

### Strolls

On Monday Dan and Robert went for a stroll around Westminster and spoke about search and work and life.

Anya, Robert and Michael took the opportunity of being in Cambridge to stroll round the [Botanical Gardens](http://www.botanic.cam.ac.uk/Botanic/Home.aspx). Which was most pleasant.

### Things that caught our eye

* [Sharing Goes Both Ways – No Secrets Social](https://blog.ouseful.info/2017/11/09/sharing-goes-both-ways/)

* [No boundaries: Exfiltration of personal data by session-replay scripts](https://freedom-to-tinker.com/2017/11/15/no-boundaries-exfiltration-of-personal-data-by-session-replay-scripts/)

* [The tech industry needs a moral compass](https://medium.com/doteveryone/the-tech-industry-needs-a-moral-compass-3ce1665a287f)

* [OData Version 4.0. Part 2: URL Conventions Plus Errata 03](http://docs.oasis-open.org/odata/odata/v4.0/odata-v4.0-part2-url-conventions.html)

* [Nemawashi](https://en.wikipedia.org/wiki/Nemawashi)

* [The Buzzcocks - What Do I Get?](https://www.youtube.com/watch?v=-EEPvXlTUnU)