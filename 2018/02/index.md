## 2018 Week 02

### Back to school

Refreshed and revived and not at all hungover, the Data and Search team has now returned to the coal face. Mostly. Numbers still seem a little short but we're assuming they might turn up at some point. As for the rest of us, we are, much like [Alan Minter](https://en.wikipedia.org/wiki/Alan_Minter), [fit and working again](https://www.youtube.com/watch?v=QnxZkK4mdM8). Mmmmmph.

[Dan](https://twitter.com/dasbarrett) returned from the Christmas break and started picking up some of 2017's many loose threads. The big things this week are work on [Statutory Instruments](http://www.parliament.uk/business/bills-and-legislation/secondary-legislation/statutory-instruments/) and some movement on topics. There was also something about the data strategy and fixing all the corporate data. And Portugal got in touch to talk about data visualisation following Dan's trip to the [IPU](https://twitter.com/IPUparliament) in Geneva last year because we are...

### International, continental, Parliament in the area

Whilst Oxford is not really a different country, people do tend to pronounce things differently there. Anyway, it's where the annual [Study of Parliament Group](http://www.studyofparliament.org.uk/) conference is held so [Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) took the train and went along. It was all most interesting and they learnt more about trade deals in light of brexit in one session than journalism had taught them in a couple of years. Thanks journalism.

### Community

Last Wednesday [Sally](https://twitter.com/cinnamon_sally), [Ganesh](https://twitter.com/gansenthi) and [Mark](https://twitter.com/markhurrell) from [GDS](https://gds.blog.gov.uk/) came over to meet Anya, [Silver](https://twitter.com/silveroliver) and Michael and chat about domain modelling the liminal zones between government and Parliament. It went quite well though we still have no clue what that thing government people call "policy" might be. [Lucinda](https://twitter.com/LucindaMaer) joined us for an hour. Thanks Lucinda.

The next day Michael paid a return visit to Ganesh and Mark to chat about information architecture and navigation and subsidiary resources and search. And some of the things both gov.uk and parliament.uk will need to fix if they want to [play nicely with search engines](http://smethur.st/posts/176135866). Conversation continued over chops at [Tayyabs](http://www.tayyabs.co.uk/). Nice chops. Seriously nice chops.
 
### Corpcomms

Yammer so quiet you could hear a fist drop. We're sure it'll pick up in the new year.

### One world, one web, one team

Dan and Michael spent some time with the Members' activity website product team to go over plans for their alpha. Dan also went along to the website product roadmap meeting.

### Domain modelling

There seemed to be a lot of meetings about topics for some reason. Like suddenly topics are fashionable. Anya and Michael met with [Jamie](https://twitter.com/oddtype) and the Guide to Procedure team to chat about topic tagging and navigation. They continued to tweak the [question and answer](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html), [tabling](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html) and [formal body affiliation](https://ukparliament.github.io/ontologies/formal-body-affiliation/formal-body-affiliation-ontology.html) models as feedback came in. The latter still does not pass the Ed McCarthy test but they feel they are close.

Anya, Silver and Michael finished writing a paper for [ESWC](https://2018.eswc-conferences.org/). Fingers are now firmly crossed.

### Data platform

Matthieu's post on [Graph Database Performance testing](https://pds.blog.parliament.uk/2017/12/15/performance-testing-a-graph-database/) caught the eye of [Jesús Barrasa](https://twitter.com/BarrasaDV), director of Telecoms Practice at Neo4j and author of [an RDF import / export tool for Neo4j](https://twitter.com/BarrasaDV/status/948958016736563201). We sent him a dump of our data as well as the SPARQL queries used. We're looking forward to hearing about performance testing in other graph database engines.

Our [OData](http://www.odata.org/) RESTful interface has received over 4K requests since it launched back in December. Considering the holiday season and the limited exposure, we are most encouraged by this. [Jianhan](https://twitter.com/jianhanzhu) took a look at the application insight log to check unsuccessful responses to these requests. He identified one issue with the ExternalIdentifier property and worked with Wojciech and [Chris](https://twitter.com/chrisalcockdev) to change the property from single to multiple values. He's also been working with Wojciech to remove interfaces from our class hierarchy to simplify the OData data model. The work will make the data model more straightforward, and will fix some issues with the OData interface.

[Raphael](https://twitter.com/raphaelleung) loaded 100+ million statements into a cluster of triple stores. That's many, many more statements than in our current data platform triplestore, but quite a few fewer than our older subject indexing triplestore. This is being done as part of running the [Berlin SPARQL Benchmark](http://wifo5-03.informatik.uni-mannheim.de/bizer/berlinsparqlbenchmark/). There have been a few kinks in the process, as the benchmark hasn't been updated for a few years but it was still a good learning process.

### Search

Raphael and Liz met with Fred to talk about search hints for [Research Briefings](https://researchbriefings.parliament.uk/). We have hints covering lots of different briefing types and aren't sure if they would all be understood by users. Fred's team will talk to the business and help us refine the hint names with a plan to make them live.

Alongside this we can now crawl the website to get a list of URLs. We're working on analysis for hint coverage and hint types related to Research Briefings based on the current rules.

### Measuring things

Much things, very measure.

[Colin](https://twitter.com/ColinPattinson) and Liz met with Cassie, Mark and Philip from the House of Commons Library statistics section to talk about consolidating and improving reporting for constituency statistics. They're looking for a better user experience. And some savings in processing time. The current method for publishing information is bespoke and updates are made to individual datasets manually. Constituency pages aren't currently a priority on the [beta website](https://beta.parliament.uk), but [Samu](https://twitter.com/langsamu) and Liz had a chat and will explore storage in the triplestore as an option.

Sara is helping [Trine](http://twitter.com/StealthGeekUK) set up a survey to be sent to constituency offices about the type of enquiries they receive. Based on the responses we’ve got so far, the format of a few questions will be changed to better fit the way constituency offices work. Sara also started writing a 'how to' guide for AB testing experiments. She's currently reading about [mental models](https://www.nngroup.com/articles/mental-models/) and has done a competitor analysis exercise for the Utilities product team.

Saffiyah started planning an assessment of the impact of the hints that have been added to search. She presented her planning to Liz and Steve from the User Research team. It was useful to discuss ideas on other ways to assess impact. Sara found that the Irish parliament website also uses ['hints' in search results](https://beta.oireachtas.ie/en/search/).

Sara and Liz presented the A/B testing results for showing URLs on search results at show and tell. We saw a small change in the measures we assessed but didn't have enough data to be confident this change was repeatable. Although the data showed a slight improvement for users seeing URLs, it might just be chance. URLs are now live on search results in a truncated format.

### Did the machines learn owt?

Diddly-squat. But they got early learning toys for Christmas so we're still hopeful.

### Did anyone say blockchain?

No one in the Data and Search team seemed to say blockchain. Though [these blokes did](https://twitter.com/matt_levine/status/951147744772743168). Jesus wept.

### Strolls

Robert and Michael took a couple of strolls through Westminster in search of coffee. Coffee was eventually found.

### Things that caught our eye

* [When unique IDs are not... unique](https://medium.com/@Ellayanor/when-unique-ids-are-not-unique-b469ec0a6c63)

* [Inverse problem](https://en.wikipedia.org/wiki/Inverse_problem)

* [Data-driven programming](https://en.wikipedia.org/wiki/Data-driven_programming)

* [W3C study of practices and tooling for Web data standardisation](https://www.w3.org/2017/12/odi-study/)

* [Sources of Evidence for Automatic Indexing of Political Texts](https://pdfs.semanticscholar.org/351b/c4fb0a85f3de3690e0131ad7479c1942ec87.pdf) [PDF]

* [Digitization of the Canadian Parliamentary Debates](ftp://ftp.db.toronto.edu/public_html/cs/ftp/public_html/pub/gh/Beelen-etal-CJPS-2017.pdf) [PDF]

* [Measuring Emotion in Parliamentary Debates with Automated Textual Analysis](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0168843)