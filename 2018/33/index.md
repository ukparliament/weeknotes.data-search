## 2018 Week 33

### Is [Samu](https://twitter.com/langsamu) morality?

Our Samu is currently off on his holidays. In his absence we’re continuing to work under the assumption that his morality remains ontologically complete.

### Community

[Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) went over to [Newspeak House](https://www.nwspk.com/) to chat to [John Bryden](https://twitter.com/Jb_tweets) who's a new [fellow](https://www.nwspk.com/fellowship) in those parts. They sat on the terrace munching bagels and feeling quite good about life. John's looking at graphs of political connections and lines of influence, which gave everyone a chance to chat about [All Party Parliamentary Groups](https://en.wikipedia.org/wiki/All-party_parliamentary_group) and Michael another chance to chummer on about [complex user communities and information ripples](https://twitter.com/fantasticlife/status/1009802788145188865). And resurrect one of his old chestnuts about [using plagiarism detection for the epidemiology of information](https://www.slideshare.net/tristanf/gleaning-provenance-from-article-similarity). Michael's put John in touch with both [Tony](https://twitter.com/psychemedia) and [Andrew](https://twitter.com/generalising). Hopefully we'll chat again soon.

Anya promised John a parliament's worth of [House of Commons Hansard](https://hansard.parliament.uk/Commons) contributions and any accompanying subject indexing data. [Alex](https://twitter.com/alexedwardh) has started work on getting an export of all proceedings from the [55th parliament](https://en.wikipedia.org/wiki/List_of_MPs_elected_in_the_United_Kingdom_general_election,_2010) from [Solr](http://lucene.apache.org/solr/) and writing a [Powershell](https://en.wikipedia.org/wiki/PowerShell) script to iterate through linked child contributions to return records that are indexed differently to their parent proceedings. Nice work Alex.

Anya and Michael also spent some time looking at the card index files [Michael Rush](https://socialsciences.exeter.ac.uk/politics/staff/rush/) sent up covering the last three intakes of House of Commons Members. They’ve added some test data to the spreadsheet they’ll be working with for now, which went quite well. Except it seems that the handwriting of professors is really no better than than that of doctors. We expect to be scanning and emailing many cards shortly.

Anya and Michael had a phone chat with [Andy](https://twitter.com/mr_dudders) and [Dave](https://twitter.com/der42) about the [stats series model](https://ukparliament.github.io/ontologies/stats-series/stats-series-ontology.html) and how compatible it is with the [RDF data cube](https://www.w3.org/TR/vocab-data-cube/) model. Michael had spent some time with the data cube documents but his brain had failed to really map the spec to the examples. They now think they're slightly clearer on data cube but are still wondering if they need to make more changes to their model. Or just scrap it and use data cube. Michael's keen to get some time with [ODI](https://theodi.org/) types to help with this and is chatting to [Leigh](https://twitter.com/ldodds) as he types.

Way back in February, Michael ran an event at Newspeak House to chat about [analytics, tracking and privacy in the public sector](http://citizenbeta.attending.io/events/analytics-tracking-and-privacy-in-the-public-sector). It went well. Or Michael thought it did. And there was interest from attendees in collaborating on a document. Michael has been meaning to get on with this ever since but some combination of [statutory instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) and [tracking services](https://beta.parliament.uk/statutory-instruments) took his attention. So [Ade](https://twitter.com/Adewunmi) dropped by Tothill Street on Thursday and kindly kicked his arse. They started on an outline of a document which they'll share more widely when they're happy. Thanks Ade.

### Showing and telling

[Matt](https://twitter.com/mattrayner) did a brief reprise of his talk on the new website architecture which seemed to go down quite well. Michael watched over a crashy appear.in link and had questions about model expression in components. A meeting has been arranged.

### Domain modelling

A fair bit of progress this week but all a little less visible than would be ideal. The service we used to transform [Turtle](https://en.wikipedia.org/wiki/Turtle_(syntax)) files to HTML fell over and hasn't yet been resurrected. So our Turtle files and HTML are running a little out of sync. We've made previous efforts to run a local mirror of [LODE](http://www.essepuntato.it/lode) but our lack of Java skills let us down. In the meantime, Robert has set out to write his own Turtle to HTML converter. Which would be handy.

Anya, Jayne and Michael met [Jack](https://twitter.com/jackpdent) from the House of Commons Journal Office to run through the impact of withdrawal of statutory instruments across the [laying](https://ukparliament.github.io/ontologies/laying/laying-ontology.html) and [procedure](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html) model. Given withdrawal seems to preclude every other procedural step, they think they should just keep it part of the laying model and steer clear of adding withdrawal steps to the [procedure flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples). But they need to check that with Samu.

There was also some chat around approval motions for affirmative SIs falling at the end of [sessions](https://ukparliament.github.io/ontologies/time-period/time-period-ontology.html#d4e539) and new motions needing to be [tabled](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html). Which brought up talk about a session clock and how much additional procedure flowcharting would be necessary. There's a general feeling that the current procedure model doesn't allow enough in the way of conditional logic for steps that repeat in series according to flows through cycles. A head bending chat with Jayne, [Silver](https://twitter.com/silveroliver) and [James](https://twitter.com/thevinternet) is planned.

On the subject of head bending: librarians Anya, Jayne and Claire, Michaels Mike and Michael, some highlighter pens, and much paper all got together to check the [procedure data](https://procedures.azurewebsites.net/) matches the current state of the flowcharts. They had hoped to cover all five procedures but limped along to the end of one. An exhausted Mike crept from the room and decided that writing a screen's worth of SQL would save everyone's sanity here. More checking is planned but Mike's work will hopefully make fewer brains break.

Anya, Robert and Michael had all of Thursday booked in for a meeting with the slightly optimistic title of 'Comments blitz'. They'd intended to run through all the models so far and check the comments and improve them where possible. They managed to cover off one model. But at least they think the comments improved.

Anya and Michael drew up a new version of the [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) with SI series and series membership. Mostly off the back of Jack answering a stream of emails. And Catherine Tabone from [The National Archives](http://www.nationalarchives.gov.uk/) explaining SI series and membership constraints. Thanks Catherine.

[Alison](https://twitter.com/oliala) met with Nick Jones from the Business Systems team who showed her the application they've built for managing All Party Parliamentary Groups. For now it's used for registering APPGs, any benefits they've received and the membership of their governing committees. It doesn't maintain a full list of members, nor is it used for booking meetings. The information in the application is no more than appears on the [APPG web site](https://publications.parliament.uk/pa/cm/cmallparty/180718/contents.htm), although it can be used to run reports. External organisations linked to the groups are entered as free text. Alison's sketched a quick [domain model of what we have for APPGs](https://github.com/ukparliament/domain-models/blob/2291f4a5eb2c0c030756e15116a0b032463554df/APPGs/APPGs.pdf), excluding meetings and incumbency, which are already covered by other models.

### Data platform

This is a late one that just missed the deadline for last week. Samu spent a day with [Oli](https://twitter.com/olihawkins) exploring our chosen cloud offering from a Python developer's perspective. They started with a 'Hello world' and got as far as sending emails through a [Logic App](https://azure.microsoft.com/en-gb/services/logic-apps/) via Parliament's [Exchange server](https://en.wikipedia.org/wiki/Microsoft_Exchange_Server) to a list of recipients stored in a managed [Postgres](https://en.wikipedia.org/wiki/PostgreSQL) database by a little [Flask](http://flask.pocoo.org/) app in a [Docker](https://en.wikipedia.org/wiki/Docker_(software)) image continuously deployed to an [App Service](https://azure.microsoft.com/en-gb/services/app-service/). They stopped short of automating builds from [Git](https://en.wikipedia.org/wiki/Git) by [VSTS](https://visualstudio.microsoft.com/team-services/) because they both wanted to make it home to bathe their kids. And they feared our reader might run short on breath.

They now have longer term plans for improving the Current Awareness newsletter, moving [Research Briefings](https://researchbriefings.parliament.uk/) to the new website and improving them by adding facilities for publishing research data. They also talked about linking Oli's work on crowdsourced place names to the new data service. All in all they had a very good day. Which is nice.

[Matthieu](https://twitter.com/cognithive) set about creating Docker files to help demonstrate our issues with the latest version of [Vocbench](http://vocbench.uniroma2.it/). He also created a new set of load tests for the [Augustus](https://github.com/ukparliament/augustus) / [Thorney](https://github.com/ukparliament/thorney) infrastructure and got briefly (and it must be said incorrectly) blamed for killing search (see later). He spent some time chatting through the load testing with [Matt](https://twitter.com/cognithive), Allan and Christine and the results (about 10 pages per second on one node) gave Matt enough confidence to take his code to staging. Matthieu and Allan talked about graphs, ontologies and Brixton. In the absence of [Dan](https://twitter.com/dasbarrett), Matthieu also picked up the running of the data strategy session. And, perhaps unfortunately, was the sole attendee. Top marks for effort though.

### Use APIs, they said. What could go wrong, they asked?

Wojciech interrupted his well-deserved holiday to forward an alert from the search service. A quick check revealed no results were being returned for any search query. Which was less than ideal. [Jianhan](https://twitter.com/jianhanzhu) and [Jamie](https://twitter.com/oddtype) sat scratching heads and troubleshooting the issue. For a few minutes they worried that Matthieu's load testing had been a little too aggressive and had caused something in the data platform to keel over and die. But as they peeled back the 500 errors from our API Management layer they uncovered 400 errors in the underlying service. More specifically [410](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/410s). The API had gone.

Jamie spent some time [checking Twitter](https://twitter.com/oddtype/status/1030388597046816769) and Jianhan checked the [online service](https://dev.cognitive.microsoft.com/docs/services/56b43eeccf5ff8098cef3807/operations/56b4447dcf5ff8098cef380d/console) and it soon became clear the issue was with [Azure](https://en.wikipedia.org/wiki/Microsoft_Azure). A support ticket was raised and within an hour the service was up and running again. In the meantime, other people experiencing the same issue had migrated to a more recent version of the service. Another job for our to do list.

Jamie and Jianhan would like to apologise to Matthieu for ever doubting him.

### On search. And indeed indexing

Our Liz reports we now have more visibility of searches across [Hansard](https://hansard.parliament.uk/), [MPs](https://www.parliament.uk/mps-lords-and-offices/mps/), [Constituency Finder](https://constituencyfinder.digiminster.com/) and [online petitions](https://petition.parliament.uk/). And also across some things like the [deposited papers](https://www.parliament.uk/depositedpapers) filtered list. Though there's still some debate about whether we even call that search, given there are no search terms. That said, Michael has fewer doubts. In his head at least, it’s just a badly designed browse. According to Liz's calculations, these assorted forms are used more than the default website search, though she suspects her fuzzy query still needs work.

Hints went live on website search a few weeks ago. [Sara](https://twitter.com/sarafreis) et al decided they'd use time spent on a search results page before clicking a link as a measure for monitoring change. They've grouped sessions based on behaviour: the device type used and result number clicked. Which is similar to what they did when we ran the A/B testing for the display of URLs on search result pages. Sara's using [power analysis](https://www.statmethods.net/stats/power.html) to estimate the sample size required to detect a change with a given degree of confidence, i.e. how many days of data do we need to collect to confidently say that, if there’s been a change, that change is significant? As it turns out, for desktop users clicking the first result we have enough data points after 4 days, whereas for mobile users we’d need 67 days’ worth of data. Desktop users generate the majority of traffic.

### Measuring things

Our Liz also checks in to say lots of people are talking about measurement. Which obviously gets her seal of approval. Liz thinks we need more consistent messaging and a few practical things to help move everyone in the same direction. But she's not sure what they are yet. She's planning to speak with the performance managers about the new measurement model (which appears to not yet have a URL) but probably not until October.

### Corporate data

Lew's been monitoring our integration messaging system after a few performance configuration changes. He's also been looking at how best to utilise some new servers the team have had donated, continued his involvement in the ongoing stock system project, and spoken to people about how we improve our KPI reporting.
 
Noel continued his work to clear the tickets logged whilst [BizTalk](https://en.wikipedia.org/wiki/Microsoft_BizTalk_Server) burned during the last couple of weeks. He's used the tickets to test that the system is in the same state it was in prior to the fire. Or at least the ones that weren't too singed to read. All the tests have proved satisfactory, faults are being addressed and no new reported or observable problems have come to his attention. Work continues around improving the system and avoiding any reoccurrence. Fire extinguishers are on order.

### Strolls

Another week with very poor stroll performance analytics. Though Anya and Michael did wander through Spitalfields on their way to Newspeak. And stopped off to try on daft glasses.

### Leavers and joiners

Our Liz reports that James, our shiny new data analyst, will start with us on the 17th September. Delightful news.

### Did anybody get a free sandwich?

Liz got a free sandwich for pointing out Pret had messed up the labelling scheme. Well done Liz.

Anya acquired a free chocolate hazelnut croissant. This time because Michael messed up the queuing system. Again from Pret. They'll be bankrupt at this rate.

### Things that caught our eye

* [Optimising the ONS site search function with Google Analytics and Natural Language Processing](https://datasciencecampus.ons.gov.uk/optimising-the-ons-site-search-function-with-google-analytics-and-natural-language-processing/)

* [Beyond Findability - Enterprise Knowledge](https://enterprise-knowledge.com/beyond-findability/)

* [Project Open Data](https://project-open-data.cio.gov/principles/)