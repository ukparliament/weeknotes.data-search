## 2018 Week 38

### Has Jesus returned?

Not yet, but we wait in hope. A missive to the [data@parliament.uk](mailto:data@parliament.uk) inbox concluded with the words 'BIBLE YES! CONSTITUTION NOT! 2070: JESUS WILL RETURN.' Here in the [Parliamentary Computational Section](https://pds.blog.parliament.uk/) we are fully [rapture ready](http://www.rr-bb.com/). Though 52 years seems a long time to wait. But we will not be idle. We have data to munge and printers to fix. Any return of Jesus will certainly be covered here in weeknotes when, and not if, it happens. Stay tuned people.

### Community

Tuesday was a day trip day. [Anya](https://twitter.com/bitten_), Robert and [Michael](https://twitter.com/fantasticlife) took off on a firm's outing to Lewes. Where [Silver](https://twitter.com/silveroliver) lives. Unfortunately [Ben](https://twitter.com/benwoodhams) couldn't make it because he had a sore throat. Because he smokes too much. No sympathy here. Robert's sherpa skills went awry and the assembled party took a wrong turn, ending up in the countryside next to [a monument for some people who had been burned](http://www.sussexmartyrs.co.uk/the-history-of-the-memorials/). Not a pub to be seen. They sat in a field and started to put together a talk they're hoping to give at the [Service Design in Government](https://govservicedesign.net/2019/) and [UX in the City](https://uxinthecity.net/2019/manchester/) events next March. It [went brilliant](https://twitter.com/fantasticlife/status/1042048747063177216).

Thursday morning saw Anya and Michael head over to [Newspeak House](https://www.nwspk.com/) for a chat with [Joscha](https://twitter.com/OpenHypervideo) and [Philo](https://twitter.com/phivk). Joscha and Philo were over in Blighty for the [BBC textAV event](https://sites.google.com/view/textav) where they [talked about opening up parliamentary debates using forced time alignment between AV and written transcripts](https://twitter.com/OpenHypervideo/status/1042739191950573568). They'll be back in that London for [Mozfest](https://mozillafestival.org/) and are interested in forming a consortium of legislatures, broadcasters and civic tech types with an interest in opening up parliamentary AV. If this sounds like you, hit them up. As the young people might say.

That afternoon, Anya and Michael headed over to meet Silver at the [British Dental Association](https://bda.org/). Which is, quite frankly, a terrifying place for anyone with British teeth. For reasons lost, they'd agreed to do [a talk and a workshop](http://www.netikx.org/content/ontologies-and-domain-modelling-fun-honest-and-friendly-introduction-20-september-2018) for [NetIKX](http://www.netikx.org/) library type folks around something to do with ontologies. They decided to rip up the brief and told the assembled librarians to forget ontologies. And all their associated acronyms. To buy no ontology books. To avoid installing [Protégé](https://protege.stanford.edu/) if at all possible. And instead to concentrate on [domain modelling](https://en.wikipedia.org/wiki/Domain-driven_design) and knowledge acquisition. Particularly in complex domains. Silver [gave a talk](https://twitter.com/NetIKX/status/1042789960686993408), Michael stumbled sweatily through a workshop. No fruit was thrown.

In one of those strange coincidences that life sometimes throws at you, the NetIKX event brought us face to face with our reader. Thanks [Philip](https://twitter.com/PhilDRoberts). You make it all worthwhile.

### One world, one web, one team

Librarians Anya and Jayne met with Computational Section types [Samu](https://twitter.com/langsamu), Mike and Wojciech to chat about the data input tool for all things procedural. Or the Procedure Editor as Samu would say. Features were agreed. Once everyone had agreed on what the definition of feature was.

[Sara](http://twitter.com/sarafreis) met with folks from the Employee Pay and Pension Service and the Governance Office to discuss digital forms and the reporting thereof. She gave a brief tutorial on connecting to the data using [Power Query](https://en.wikipedia.org/wiki/Power_Pivot#M_Formula_language). She also wrote some instructions to share with the wider team. She tells us they seemed satisfied. 

[Alison](http://twitter.com/oliala) ran a second workshop looking at models for measurement, this time expanding horizons beyond our immediate data analysing friends to include creators, consumers and capturers of KPIs. New joiner Jamie R, Rosie, Glenn and Krzystof all went along. Alison says thanks all for being such active participants.

Alison ploughed through a fair few meetings. She met with Philippa to talk about [All-Party Parliamentary Groups](https://www.parliament.uk/about/mps-and-lords/members/apg/); informal groups for which Parliament doesn't keep membership lists. These lists are sometimes published by the APPGs on their own websites. She met with Kate to understand what information is captured and retained on catered events bookings on the Parliamentary estate and envisages a small domain model in due course. Together with Bridget she met Janis McAnallen from Strategic Estates to discuss space and location data. They're planning to [facilitate a workshop](https://www.youtube.com/watch?v=sv3LG6VVo8o) with Andy from [Restoration and Renewal](https://restorationandrenewal.parliament.uk/) to ensure alignment with the Data Strategy.

### Domain modelling

Not so much to report here except more comment editing happened. Slowly and painfully Robert took apart the comments and assembled them into new and better shapes. Thanks Robert.

In the absence of firm feedback, Anya, Robert, Silver and Michael took the decision to update the [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) to better reflect what they think [John](https://twitter.com/johnlsheridan) and [David](https://twitter.com/clerkly) were suggesting. So [procedural duties](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e248), [day count duties](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e213) and [laying duties](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e231) are now metaphorical strings attached to [enabling powers](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e526). Which feels nicer but more feedback is needed.

#### September [spawned a monster](https://www.youtube.com/watch?v=Xv8LdKp2Y-8)...

We have whined at some length about the [draft affirmative statutory instrument procedure](https://ukparliament.github.io/ontologies/procedure/sis/draft-affirmative.pdf) and how complicated it is when you start to include instrument withdrawal. All the same, what was agreed with House of Lords Jane and House of Commons [Jack](https://twitter.com/jackpdent) last week has been added to the data platform. Through squinted eyes and breaths of horror, Anya and Michael added 2 new steps and several new routes. They remain cross-eyed. I mean, [look at it](https://procedures.azurewebsites.net/Procedures/3/graph). What an absolute mess.

### Data platform

[Alex](https://twitter.com/alexedwardh), Mike and Wojciech continued to investigate an issue with the internal to external [data.parliament](http://www.data.parliament.uk/) file transfer process. A hairball in the pipelines had been causing the whole process to choke. Wojciech papered over the cracks with a little more catch and retry logic. So far it seems to be working.

### On search. And indeed indexing

Matt's been looking at how we might use data analysis to help the Indexing and Data Management Section in the House of Commons Library. At the moment they subject index [parliamentary questions](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html#d4e625) shortly after they're [tabled](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html). But changes in the [thesaurus](http://www.data.parliament.uk/dataset/thesauri) and the ebb and flow of topics discussed in Parliament mean they often revisit earlier work to check the indexing is still useful. Which can be time consuming. Matt's been looking at a couple of methods for assessing the changes made by indexers, reusing some of the techniques he's been investigating with Sara. Namely, [Latent Semantic Analysis](https://en.wikipedia.org/wiki/Latent_semantic_analysis) and [cooccurence matrices](https://en.wikipedia.org/wiki/Co-occurrence_matrix). Though so far, due to the intricacies and subtleties of the task, his efforts have not met with much success. [Machines 0 - Librarians 4](https://en.wikipedia.org/wiki/London_0_Hull_4).

Librarian Jayne and Computational Section Alex combined their brains to look at [paper petition](https://www.parliament.uk/get-involved/sign-a-petition/paper-petitions/) data in the Search and Indexing [triplestore](https://en.wikipedia.org/wiki/Triplestore). We've seen some issues with incorrect or missing links between petitions and their presentation in Parliament. Jayne figured out the correct proceedings for affected petitions and Alex wrote a script to bulk update the links. Great things happen when computational people and librarians [form like Voltron](https://www.youtube.com/watch?v=2kkJDHRYxWM).

### Corporate data

All quiet this week. There were [no alarms and few surprises](https://www.youtube.com/watch?v=u5CVsCnxyXg). Nothing caught fire and nothing [exploded](https://www.reddit.com/r/CatastrophicFailure/comments/3z7vj7/the_result_of_a_boiler_explosion_on_a_steam/). 

Lew went to a meeting about corporate systems integration and the data strategy. Not having to carry fire extinguishers around freed up his hands for long enough to fix a reporting integration for our support software. And he even managed to fit in some investigative work into some test failures in a new finance integration. Splendid stuff Lew.

### Aidan's truly terrible week (slight return)

[Aidan](https://twitter.com/aidan_morgan) has left the Data and Search team to plough a new delivery management furrow in development land. So we have a (relatively new) arrival in the shape of [Paul](https://twitter.com/paulwakely). Following in [Aidan's footsteps](/weeknotes.data-search/12/#aidans-truly-terrible-week), Paul has had a truly terrible week.

He continued meeting his new colleagues, trying to understand everything they are working on. He met with Rosie Hatton to talk about how the Data Strategy aligns with the wider Digital Strategy. He discussed some PowerBI needs with Frederico Maia, the Head of HR Shared Services. He spent a lot of time reading strategy documents and Restoration and Renewal slides. Paul used to work for the BBC so uses the word 'deck' here. He attended an all-day course on preparing business cases. A whole actual day. And then he had two of his front teeth pulled out. Poor lad.

### Capability

Our small but ever growing family of data analysts attended a [career path](https://www.youtube.com/watch?v=8JM8C49pf40) workshop run by [Julie](https://twitter.com/julietouring). They talked about possible [opportunities](https://www.youtube.com/watch?v=di60NYGu03Y) for people working with data stuff.

### Leavers and joiners

No baby news this week although, after some time away, [Chris](https://twitter.com/chrisalcockdev) has returned to us. Welcome back Chris.

And Jamie has joined our Liz's team as a new data analyst. There is almost no data we can't analyse now. Welcome aboard Jamie.

### Strolls

Anya, Robert and Michael took a much needed break from comment editing and headed across St James's Park in the general direction of Soho. Where they found an arcade and played air hockey. Michael beat Anya, Robert beat Michael and [Anya whipped Robert's arse 7-0](https://twitter.com/fantasticlife/status/1042448972483186688). So it was all quite inconclusive. Then they went for a milkshake. As they frequently do. The milkshake was superb, though they found the [outlet somewhat clinical](http://snowflakegelato.co.uk/boutique-page/soho/).

### Things that caught our eye

* Silver sent over [The quality of a design will not exceed the knowledge of its designer;
an analysis based on Axiomatic Information and the Cynefin Framework ](https://www.sciencedirect.com/science/article/pii/S2212827115007994) [PDF].

* Michael read [The Rise and Demise of RSS](https://twobithistory.org/2018/09/16/the-rise-and-demise-of-rss.html) and pined for the past.

* Matt points us at some [data visualisations created out of Play-Doh](https://www.amycesal.com/day-doh-viz-all/).