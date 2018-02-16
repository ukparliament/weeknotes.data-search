## 2018 Week 07


### [Steps, it's 39](https://www.youtube.com/watch?v=u3ZvO4pcTHs)

For many people Wednesday was Valentine's Day. For a lucky few it was [dator day 39](https://twitter.com/fantasticlife/status/963803168692932608). Our [Dan](https://twitter.com/dasbarrett) was ill so the team took a turn for the holacratic and successfully self-organised.

We were joined in the afternoon by [Caroline](https://twitter.com/carolinekippler), Sarah and [Jamie](https://twitter.com/oddtype). Joint website priorities were agreed:

* Moving concepts (indexing terms) to the live service for the Guide to Procedure team.

* Building out content collections in the data platform to allow the Guide to Procedure team to curate content into things a bit like parts and sections and chapters. We need to firm up modelling of collections, collection hierarchies, ordering within a collection, collections in a collection and basic collection descriptions.

* Continuing to work on getting written question and answers into the data platform and agreeing the API spec with the website team.

* Continuing work on modelling the [Statutory Instrument](http://www.parliament.uk/business/bills-and-legislation/secondary-legislation/statutory-instruments/) process flow with some accompanying modelling around [Early Day Motions](http://www.parliament.uk/site-information/glossary/early-day-motions/).

* Continuing to help both the Members and Committees teams with queries around all things group like (government organisations, committees and answering bodies).

* Some [Samu](https://twitter.com/langsamu) and [Matt](https://twitter.com/mattrayner) time to coordinate changes to the API, accompanying rel-alt elements, support for hierarchical JSON etc.

### Community

[Liz Marley](https://twitter.com/greensideknits) organised and hosted a meeting of [TiPS](http://www.nglis.org.uk/tips/tipsben.htm) in Tothill Street. [Anya](https://twitter.com/bitten_) and Michael gave a talk about the work they've been doing with [Silver](https://twitter.com/silveroliver) on domain modelling and ontology design and etc. It seemed to go quite well.

Samu and [Chris](https://twitter.com/chrisalcockdev) called by in the afternoon to chat taxonomies and taxonomy management software.

### One world, one web, one team

[Alex](https://twitter.com/alexedwardh) has been tinkering with the Search and Indexing triple store in an attempt to grab data for our Liz. Liz has been looking at usage of subject indexing terms over time by the Indexing and Data Management Section (IDMS) in the Mouse of Commons Library. Alex has automated a query to return daily reports for subject terms used and the frequency of their usage. It's now whirring away and spitting out data.

Alex also automated a query to export the last six months of data from the Solr index. In order to keep things from breaking, the app currently runs twice a day and is grabbing a week's worth of records at a time. It should take about 13 days to grab 6 months of data at its current rate. Sara and Saffiyah are planning to use this data to help IDMS, investigating things such as how consistent indexing is over time, the granularity of the terms used, and the cooccurrence of terms across content.

Liz and Steve ran a "drop in session" to offer help and advice around all things analytics and user research. 8 people from 8 different teams came along to chat. [Julie](https://twitter.com/julietouring) would like to say thank you.

Liz met Jamie to talk about webmaster tools. Jamie has recently set webmaster access at DNS level for current and beta sites. He's now given Liz access.


### Domain modelling

Michael went along to a kick off meeting with the web team that's about to start work on the "Statutory Instrument tracker". He showed them some flow charts and tried to explain that modelling SIs is trivial but impossible.

Anya and Michael dipped a toe into Early Day Motion waters. Something a bit like a model emerged, but they're not quite sure how much of it is specific to EDMs and how much of it is generally applicable to things which are tabled. They're meeting a House of Commons Table Office person next week to discuss.

Anya and Michael also met with [Nerys](https://twitter.com/nerys_d) (formerly of this parish) to idiot check their SI flow charts. There's still some confusion around the proportion of negative SIs that need to go to the Speaker for [EVEL certification](https://www.parliament.uk/about/how/laws/bills/public/english-votes-for-english-laws/). They hope to have an answer on this next week.

### Data platform

Samu's been making some improvements to the Fixed Query application. This is the application that holds the many and varied queries that serve data to the new website. He's added an additional unit test to guarantee new queries are mapped to a corresponding endpoint. Previously it was possible for a developer to forget to create the endpoint definition to expose a new query on the API. And now it isn't. 

Samu's also added a status check to pull requests, so developers submitting new code know whether their code passes our tests. We have both belts and braces.

Work has continued on investigating source systems and data quality for written questions and answers. No data has been orchestrated as yet, but that should start to happen soon. In the meantime, we know the shape of the data model so it's possible for the website team to develop against agreed API specs.

### Search

[Jake](https://twitter.com/carboia) has pushed [Open Graph](http://ogp.me/) markup to the beta website. Which means assorted social media platforms and search engines get a little more "metadata" (forgive me) about our pages. And can decorate their links accordingly. Top work Jake.

At Jake's request, Samu has tinkered with our [robots.txt](http://www.robotstxt.org/) to open Members' photos to search engines.

### Corporate data

Matt's new feed for the House of Commons HR system has run successfully in the test environment. The initial data comparisons are promising. Noel's been working on a manual examination of live records. Both Matt and Noel were pleased when the number of accounts to delete matched exactly between the manual examination and the automated process. A few more tests and checks are left. But the feed will be live soon.
 
Noel's been doing a data cleanse of people directory records in the HR systems. He's continuing to review the data held in People Data and continuing to create, update and delete users as requested.

Noel's also updated the statistical information pulled from the incident management system.
 
Lewis is continuing with development and testing work for new finance and stock data integrations.

### Excellent customer service award...

Sadly, no excellent customer service was delivered. Tune in next week when we're sure we'll have been of some use to someone.

### Are topics fashionable?

Well, we met some taxonomists who certainly seemed to think so.

### Did anyone on the internet confuse Parliament with government?

Not when we'd finished with em.

### How many doctors have we got?

We now have two doctors. Sara has joined [Jianhan](https://twitter.com/jianhanzhu) in being educated. Well played Sara.

### Strolls

No strolls reported but Anya, [Ben](https://twitter.com/benwoodhams) and Michael did pop by Robert's house for a lovely lunch and some wine. We played by Surrey Rules. [Everybody wore Robert's socks](fantasticlife: Everybody wore Roberts socks pic.twitter.com/LyVOSZ5Zdu).

### Things that caught our eye

* [The Dangers of Faith In Data](http://scottberkun.com/2013/danger-of-faith-in-data/)

* [Microsoft: We're developing blockchain ID system starting with our Authenticator app](http://www.zdnet.com/article/microsoft-were-developing-blockchain-id-system-starting-with-our-authenticator-app) [goddam]