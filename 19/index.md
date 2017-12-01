## Week 19: 01-12-2017

### [Leave the Capitol](https://www.youtube.com/watch?v=GpMoRS_9bcM)

Your final reminder that our [5th Parliament, data and democracy meetup](https://attending.io/events/parliament-data-and-democracy-meetup-5) is on Wednesday 6th December, this time at [ODI Leeds](http://leeds.theodi.org/).

Speakers lined up are our [Dan](https://twitter.com/dasbarrett), [Cristina Leston-Bandeira](https://twitter.com/estrangeirada) (Professor of Politics at the University of Leeds), [Tom Forth](https://twitter.com/thomasforth) (Head of Data at ODI Leeds) and [Edward Wood](https://twitter.com/edwardwood99) (Director of Research in the House of Commons Library).

More in the way of interesting talks, nice people and [free beer](https://en.wiktionary.org/wiki/free_as_in_beer). Come along. Bring a friend.

### International, continental, Parliament in the area

Dan didn't get to follow up on the multiple international leads he got in Geneva because he spent lots of time talking to people about the website, corporate data, and dashboards (website like things that no-one ever clicks on for the avoidance of doubt).
 
### Community

Robert popped out to see [Libby Miller](https://twitter.com/libbymiller). Libby made a [terrible music box](https://twitter.com/libbymiller/status/931570611536703488). Robert supplied the box. 

[Michael](https://twitter.com/fantasticlife) met with Edward Wood and a PhD student from [King's](https://www.kcl.ac.uk/index.aspx) who's looking at social media engagement with Parliament. Several proxies for engagement were discussed.

[Anya](https://twitter.com/bitten_) and Michael met with [Stephen Betts](https://twitter.com/stephenbetts) from the [NYPL](https://www.nypl.org) to talk about libraries and archives and [searching and browsing](http://smethur.st/posts/176135866). Dan popped by to say hello.

### Corpcomms

Dan and Robert met in real life (and not on Slack or indeed on Yammer) to talk about Yammer. A plan emerged. A 'yam plan' if you will. I for one am not asking.

### Who is L Ron Hubbard?

Nobody knows mate.

### One world, one web, one team

[Aidan](https://twitter.com/aidan_morgan) and Dan were both low on ceremony attendance this week. Because of circumstances. Michael went to several. [Pazuzu](https://en.m.wikipedia.org/wiki/Pazuzu) was still un-summoned. [Cthulhu](https://en.wikipedia.org/wiki/Cthulhu) popped by but just sat there yawning.

Michael gave his talk on web and information architecture to a variety of designers and product managers and etc. Many [clouds got yelled at](http://i0.kym-cdn.com/photos/images/original/001/044/247/297.png).

Anya and Michael gave the website team an update on progress with the [question and answer model]((https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html). It seemed to go quite well. Anya has offered to give a couple of the team a tour round the Q&A system.

### Domain modelling

Anya and Michael continued to tidy up the domain model for Questions. And indeed answers.

On Thursday they were joined by Ned who was very helpful arounds questions of declarations of interest and 'tabling' in general. Thanks Ned. They've now pulled out [tabling into a separate model](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html). Though it's still in need of comments.

Anya and Michael also met with Robert to talk through work on the questions and answers domain model.

Angela and Michael did a little more work autopsying the House of Commons committee management database. They have 8 tables still to go. Coherence could not be said to be emergent.

### Data platform

[Alex](https://twitter.com/alexedwardh) wrote a couple of scripts to aid the task of manually processing missing Oral or Written Parliamentary Questions. Currently a lot of questions aren't being automatically processed due to a date issue within the question files. After having some issues at first, [Samu](https://twitter.com/langsamu) helped to make the code more functional, and after a (nearly) complete rewrite the scripts were ready for every-day use.

The first script works by scraping our public [Oral](https://publications.parliament.uk/pa/cm/cmfutoral/futoral.htm) and [Written](http://www.parliament.uk/business/publications/written-questions-answers-statements/written-questions-answers/?page=1&max=100) data sources to find the relevant UINs for a specific date. These UINs are then sent in JSON form with some other identifying data to [MyJSON.com](http://myjson.com/) (a public JSON store + API). The second script then accesses this JSON data and compares the UIN values against those in the private RDF feed. It then automatically downloads and renames the missing RDF files, ready for processing.

[Jianhan](https://twitter.com/jianhanzhu) continued working on the [OData](http://www.odata.org/) service which now supports most of OData query options.

[Raphael](https://twitter.com/raphaelleung) continued with the [Berlin SPARQL benchmark tests](http://wifo5-03.informatik.uni-mannheim.de/bizer/berlinsparqlbenchmark/). He contacted the triplestore vendor to confirm some behaviour that was causing issues in the test. 

[Chris](https://twitter.com/chrisalcockdev) gave Robert an education on assorted graph issues.

### Search

[Dia](https://twitter.com/DN78) and Robert wrote a first draft of 'a strategy note for search’ which they're trying to align with the [Digital Strategy](https://www.parliament.uk/mps-lords-and-offices/offices/bicameral/parliamentary-digital-service/digital-strategy-for-parliament/).

[Jamie](https://twitter.com/oddtype), Robert and Michael met to chat about search and browse and URLs and subsidiary resources and stuff.

The first step in making [Deposited Papers](https://www.parliament.uk/depositedpapers) searchable happened.

### Measuring things

Sara spent time analysing the A/B testing results for search. The analysis software has limitations when it comes to calculating certain statistical measures (median absolute deviation for example) or statistical tests (t-tests, power analysis). That said it allows you to run [R scripts](https://docs.microsoft.com/en-us/power-bi/desktop-r-scripts) which means we can do the analysis in a single environment. Apparently this is good.

### Corporate data

[Mat](https://twitter.com/matiasgermanico) helped the finance team with the integration of the backend of the new online shop with sales processing.

He met with Sam Jones and provided all the details on the EPMO (something about enterprise and projects and management and offices) dashboard.

He also started work on a new feed from the HR system to ensure that job information for the staff of the House of Commons is correct. Still in HR land, he created a first pass data integration to correct email addresses. Noel and Mat are working together on the testing and will both do the release.

Mat met with the asset management integration team to agree on how requirements for data integrations will be captured.

Mat raised the fact that the House of Lords finance system does not have any integration services on. As part of delivering a fully automated integration they'd would have to be turned on and tested.

### Capability

[Julie](https://twitter.com/julietouring), Sara, Mattieu, Chris and Dan went along to the Silicon Milkroundabout recruitment event. Lots of people registered an interest. Julie would like to say thank you to all who helped.

Julie and Aidan started the Dynamic Purchasing framework conversation.

### Did the machines learn owt?

Not strictly speaking.

Raphael started a series of write ups on the [NLP](https://en.wikipedia.org/wiki/Natural_language_processing) and supervised learning aspects of the data toolkit.

Michael tried to understand how much learning the machines might have done but the whole conversation turned into a taxonomy of data science and ML.

I think it's safe to say the singularity will not start here.

### Did anyone say blockchain?

[These folks certainly did](https://www.eventbrite.co.uk/e/blockchain-and-its-applications-for-democracy-tickets-39688862456). At Parliament, not so much.

### Strolls

Dan went for a stroll with Robert. This time it included stopping for lunch which isn't something that Dan usually does. He does eat, for the avoidance of doubt. It was great.

Anya and Michael took a walk down to Tate Britain but forgot to eat lunch. It was also great.

## Meta

Robert has suggested that weeknote numbering should really follow [common standards](https://en.wikipedia.org/wiki/ISO_week_date). Michael agrees but is conflicted because [COOL URIs DON'T CHANGE](https://www.w3.org/Provider/Style/URI).

### Things that caught our eye

* [Improving Palliative Care with Deep Learning](https://arxiv.org/abs/1711.06402)

* [A Brain Built From Atomic Switches Can Learn](https://www.quantamagazine.org/a-brain-built-from-atomic-switches-can-learn-20170920/)

* [No boundaries: Exfiltration of personal data by session-replay scripts](https://freedom-to-tinker.com/2017/11/15/no-boundaries-exfiltration-of-personal-data-by-session-replay-scripts/)