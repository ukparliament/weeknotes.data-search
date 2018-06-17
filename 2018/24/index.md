## 2018 Week 24

### Working software

After three (maybe four?) months' work, the [Statutory Instrument tracker](https://beta.parliament.uk/statutory-instruments) that’s been occupying so much of our time and brain space has finally gone live. From a Data and Search perspective it’s probably the most interesting thing we’ve worked on to date and lots of the team have been involved. [Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver), [Michael](https://twitter.com/fantasticlife) and [Samu](https://twitter.com/langsamu) have chummered long and hard over domain models. [Chris](https://twitter.com/chrisalcockdev) and Samu have turned their scribblings into physical data models. Raphael and Samu have made [visualisations of procedures](https://procedures.azurewebsites.net/Procedures/4/graph) in both two and three dimensions. Jayne has entered business data until her fingers bled. Wojciech has written orchestrations to drag Jayne's work into the data platform. And Jenna, [James](https://twitter.com/thevinternet) and Samu have been writing [SPARQL](https://en.wikipedia.org/wiki/SPARQL) to drag out the data and make a website. Jenna, James and Raphael all helped Jayne with some data integrity issues. Mike, as ever, supported everyone and cleaned up any mess we left in our wake.

It's still very much a first iteration. We need to get the [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) right before we can properly list and decorate SIs. We still need to implement the [laying model](https://ukparliament.github.io/ontologies/laying/laying-ontology.html) to list items by when they first hit Parliament. And we still need a working sitting day calendar to calculate end dates for prayers and approval motions.

But all in all, we're pretty chuffed. There's a massive iceberg of thinking and work propping up what is, for now, four page types. And a whole bunch of stuff that becomes possible in the future.

For those interested in a more visual approach to explaining parliamentary procedure, Samu has made [a bookmarklet to flip between workpackage pages and their visual equivalents](https://twitter.com/langsamu/status/1007667248272760832).

### Showing and telling...

...was in the capable hands of [Jianhan](https://twitter.com/jianhanzhu) who [took us through the work he's been doing to extract data](https://www.slideshare.net/UKParliData/unlocking-the-indexing-and-search-data-goldmine) entered by the Indexing and Data Management Section of the House of Commons Library into the Search and Indexing triple store. All for the purposes of populating the written [question and answer](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) model with decent data.

### Community

Anya and Michael went down to Exeter to visit [Professor Michael Rush](https://socialsciences.exeter.ac.uk/politics/staff/rush/). One of Michael’s main research areas is the social background of politicians and, as a side project, he's compiled a massive database of 9,578 (and counting) Members of the House of Commons. Anya and Michael are working with [Paul](https://twitter.com/pseaward1) from the [History of Parliament Trust](http://www.historyofparliamentonline.org/) to take the data and make it available (and editable) online. The last three [intakes](https://en.wikipedia.org/wiki/General_election#United_Kingdom) have not yet been captured in the database and only exist as a [card index](https://twitter.com/fantasticlife/status/1006897041002278913). Luckily the House of Commons Library have volunteered to backfill the data during the quieter periods of summer recess. Many cards were read and compared to the database schema. A plan was hatched to capture the information in some linked spreadsheets, to be imported into the database once the website code is written. Splendid.

[Dan](https://twitter.com/dasbarrett) met with a group from the [ONS](https://www.ons.gov.uk/) 'Integrated Data Division' and talked to them about how we work. Like, agile and all that stuff. It was really good and they were very receptive. He also recommended the work of many of their colleagues at the ONS. [Jo Lloyd](https://twitter.com/JoannaLloyd1) (ex [Parliamentary Computational Section](https://pds.blog.parliament.uk/), now ONS) set it up as she'd always thought that data day was great. Thanks Jo.

### One world, one web, one team

[Jamie](https://twitter.com/oddtype) went to Tothill Street and sat with IDMS to try and get his head around their toolset. Martin and Steve took him through a whistle-stop tour of OASIS, Indexing and [Parliamentary Search](http://search-material.parliament.uk/). Jamie reports that everything that Michael ever said about "[stapling](https://pds.blog.parliament.uk/2016/09/09/modelling-parliaments/)" now makes perfect sense. OASIS (the Odds And Sods Information Service (really)) was a completely new one to Jamie. It's been allowing IDMS to create source reference data for years, where existing systems or processes have not made data available. He also learnt some immediately applicable things about the workflow of title creation for written questions.

Jamie also met with [Oli](https://twitter.com/olihawkins) from the House of Commons Library to discuss Oli's new Data Science role and related matters. The data visualisation theme has been bubbling away for some time now but, apart from the odd conversation, there's been little in the way of joined up activity. Liz's work on the [Constituency Dashboard](https://commonslibrary.parliament.uk/local-data/constituency-dashboard/) is one visible recent outcome. Oli talked about facilitating more of this work for his team's bespoke web based data visualisations.

We'd like Oli to start using the [UK Parliament GitHub](https://github.com/ukparliament) account to increase visibility (amongst PDS) of the work. We’ll also be able to plug this in to our hosting infrastructure to remove administrative tasks such as operations and billing from Oli’s workload.

Jamie and Oli agreed that a parliament.uk sub-domain will be the best approach for now. Couple this with a little bit of [pym.js](http://blog.apps.npr.org/pym.js/) (hat tip to the visual.ons team) and we hope to bring even more life to the [Commons Library blog](https://commonslibrary.parliament.uk/).

Liz would like to thank Samu for showing her round Github. She's now put a new version of [beta website crawl](https://github.com/ukparliament/ontologies/blob/master/crawled-urls.csv) online. Samu explained how git manages differencing and they've changed the format to make that better in the future. They've also made the file size smaller. The crawl was last run in March. The latest run found 4,500 additional pages. Liz is looking into how we might report on additions and deletions to show some sort of growth over time. This needs a bit more thought.. The context here is how people find all these pages. Samu pointed out that crawling might take a fair bit of time in the future, when we may well have 1.5 million pages of questions and answers. Webmaster tools might help here. Or the [Wayback Machine](http://archive.org/web/). Both of which have APIs.

[Alison](https://twitter.com/oliala) spent some time chatting with David about space data and with [Liz Marley](https://twitter.com/greensideknits) from IDMS about indexing. On Wednesday, she attended [PMQs](https://en.wikipedia.org/wiki/Prime_Minister%27s_Questions) and picked a pretty good day for it. No-one is quite sure yet as to how we’ll model mass walk-outs from the chamber. She also had an informal catch up with ex-colleague Connie Hedeler from [NICE](https://www.nice.org.uk/) who is keen to do more knowledge sharing and may be a candidate for one of our data days.

### Domain modelling

Anya and Michael spent time with some people from the [House of Lords Library](https://www.parliament.uk/business/lords/work-of-the-house-of-lords/lords-library/) taking a third pass at their [domain model for publishing things like Research Briefings](https://github.com/ukparliament/domain-models/blob/master/document/document.pdf). Nothing much changed from their original sessions with House of Commons Library and [POST](https://www.parliament.uk/post) people. So that was reassuring.

Tuesday was the final (we think) domain modelling session for the SI tracker. Jane, [Jack](https://twitter.com/jackpdent), [Ben](https://twitter.com/benwoodhams), Alison, Anya and Michael gathered in Tothill Street to talk through the proposed [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) and [enabling powers](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e327) and [statutory day counts](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e365). They got to something everyone seemed happy with. They hope [John](https://twitter.com/johnlsheridan) will be happy too. They've lost count of how many SI related meetings they've had but they've been good and we'll miss them. Thanks Jane and Jack for bearing with us. Thanks Ben for the Maltesers. 

### Data platform

Jayne from IDMS emailed Mike to ask some questions she and Joe Strawson had about the data platform and the SI web pages. Her description of how she enters data and how it ends up displayed on the website unearthed some new questions about the workflow, the data model and the use of the past tense in step naming. It's a good example of end to end support and development working directly with users. Without this the questions may never have been discussed, almost certainly lost between teams.

Our colleague [Phil](https://twitter.com/philbgorman) from the House of Commons Library, came up with a great use case for our [OData](http://www.odata.org/) endpoints. He used them to update a [basic Twitter bot](https://www.twitter.com/parlibot) that tells people which Government and shadow cabinet roles a Member has had. The bot replies with positions and start dates, in chronological order. It currently requires users to input a Member's name exactly, including correct capitalisation, but he's hoping to work on it and include an option for committee positions too. The [code of the bot is on GitHub](https://github.com/Mognar/memberposts/edit/alternate/Membersposts.py), in case anyone out there wants to fork it.

### On search. And indeed indexing

We’re currently missing some information around the process of data entering Search and Indexing for IDMS to index, so can’t yet accurately describe timescales. Liz talked to Samu, Mike and [Alex](https://twitter.com/alexedwardh). She learned we can get slightly closer by using the log data for the queue of items waiting to be picked by Indexing. Mike showed Liz the dead file queue (files that don't make the cut), and Alex started work on writing a daily count of these.

IDMS flagged an issue with a number of duplicate written questions in Parliamentary Search. When a tabled question is answered it should be hidden from the search index, to be replaced by the answered version of the question. For some reason, both versions were showing up in search results. Alex wrote a script to reindex multiple records in the Indexing and Search triplestore, which seems to have fixed the problem

### Corporate data

Dan properly started his new 'Service Owner - Interaction Management' gig with some meetings and a programme board. Just like the olden days. He also [wrote about his job](https://medium.com/@dasbarrett/making-changes-f3753bd26c0c) which he recognises might be vain. But aren't we all.

### Capability

[Julie](https://twitter.com/juliebyrne) ran two workshops this week about career paths and talent management. Dan went along and thought they went well. He thinks the career path stuff, in particular, is looking great. What's a career, others asked.

### Employee of the week award...

...goes to Jayne Sunley in IDMS, who's been manically [actualising](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e22) [steps](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e272) by adding [business items](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e193) to [work packages](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e284). All for the purposes of tracking SIs. At least for now, the SI tracker is basically Jayne. Like the [Wizard of Oz](https://www.youtube.com/watch?v=-RQxD4Ff7dY&t=47s), but proxied by computers.

### Strolls

No strolls reported but Anya and Michael took the opportunity offered by a trip to Exeter to visit the seaside. Ice cream was eaten and the [second round of the air hockey tournament](http://www.admiralslots.co.uk/venue/harrisons-amusements-dawlish/) took place. This time, Michael whipped Anya's ass.

### Things that caught our eye

* [High digital ambitions for our policy department](https://mhclgdigital.blog.gov.uk/2018/06/11/high-digital-ambitions-for-our-policy-department/)

* [A rough guide to central vs local government digital](http://philrumens.blogspot.com/2018/03/a-rough-guide-to-central-vs-local.html)

* [The Herzog August Library in Wolfenbüttel, Germany turned some of their medieval collections into RDF](http://markupuk.org/webhelp/ar07.html)

* [Folks from the Scottish Government and Swirrl talk about statistics.gov.scot](https://www.dropbox.com/s/r4rqu9a1bkynn7w/Scotland.mp4?dl=0)