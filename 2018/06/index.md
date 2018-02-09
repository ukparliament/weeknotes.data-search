## 2018 Week 06


### Parliament in the area, [we're international, we're continental](https://www.youtube.com/watch?v=pNfHoPIxhXM&t=1m9s)

[Dan](https://twitter.com/dasbarrett) did a skype thing with the Portuguese Parliament as part of ongoing efforts to help out. They're looking to build their data visualisation capability. [Henry](https://twitter.com/henryjameslau) (ex of this parish) sent on some great links.

### One world, one web, one team

Dan seemed to spend most of the week talking to product teams. And a fair chunk talking to [Jamie](https://twitter.com/oddtype). He went along to a session with Fred and the Research Briefings team which was actually rather good. He also went to a group chat that Sharan set up to gather ideas for the [parlidigital](https://twitter.com/parlidigital) Twitter account. Which was something different.

Dan went along to the website roadmap meeting. And lots of people came to our show and tell where [Chris](https://twitter.com/chrisalcockdev) talked about integrating content storage into the data platform. So that's good.

[Anya](https://twitter.com/bitten_) left the library to travel to computer land and talk to assorted product people about the Indexing and Data Management Section and the work they do to subject index parliamentary material. [Michael](https://twitter.com/fantasticlife) chipped in with strong [SKOS](https://www.w3.org/2004/02/skos/) reckons. A fun time was had by all.

Anya and Michael met with Steve Wise, Anya's boss man and the Director of Information in the House of Commons Library. They had a good chat about [new search](https://beta.parliament.uk/search) and its [reliance on well planned information architecture](http://smethur.st/posts/176135866). The trick here is still hypertext. Everything in its right place, at persistent URIs, subsidiary resources exposed and *linked to*. They also chatted about super specialist queries and the planned [SPARQL](https://en.wikipedia.org/wiki/SPARQL) endpoint.

Anya, [Liz Marley](https://twitter.com/greensideknits) and Michael met to chat about the [TIPS](http://www.nglis.org.uk/tips/tipshome.htm) meeting they're hosting next week.

Our Liz talked to the Guide to Procedure team about how they plan to monitor the thing they've built. They have a problem with some of their measures where they don't have consistent comparisons. Or comparisons at all in some cases. They talked through prioritising what to measure and looked in detail at three of the ideas. Whilst brain storming measures was a good initial approach, it's important to understand the practical details of collecting data and assessing change. The three initial ideas were reduced down to two. They also talked about measuring failure below a certain point, rather than success above a certain point, where previous data isn't available to judge where to set the bar.

### Domain modelling

Anya and Michael met with the Principal Clerk of the House of Commons Table Office to talk about smushing down [round robin questions](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html#d4e676) into a single question going to multiple answering bodies. For assorted reasons this is not possible. At least for now. They've updated the [question and answer model](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) to reflect that decision.

Anya, [Silver](https://twitter.com/silveroliver), [Ben](https://twitter.com/benwoodhams) and Michael spent Tuesday doing some more wrestling with [statutory instruments](http://www.parliament.uk/business/bills-and-legislation/secondary-legislation/statutory-instruments/). They're coming to the conclusion that the basic model is pretty simple: just some routes over stepping stones. Hopscotch got mentioned. The problem is those steps touch on pretty much everything in Parliament from motions and amendments to debates and committees to divisions and reports and etc. So it's basically easy. But almost [impossible](http://www.hark.com/clips/zcskfldshq-i-sure-as-hell-wouldnt-start-from-here).

On Thursday Anya and Michael took a kind of break from Parliament and decided to do government for a change. [Ganesh](https://twitter.com/gansenthi) and [Tim](https://twitter.com/TimAdey2) from GDS / the Cabinet Office came over to talk about objectives and targets and policies and interventions. A [picture](https://github.com/ukparliament/domain-models/blob/master/government/domain%20model.pdf) was drawn. They think it is OK.

### Data platform

[Jianhan](https://twitter.com/jianhanzhu) worked with [Jeanette](https://twitter.com/clementgraphics) to get Lords' photos into the data platform. They'll be available on the beta website shortly and, like MPs' photos, they'll be [openly licensed](https://creativecommons.org/licenses/by/3.0/). Prepare to fill more boots.

Jianhan also released a new version of the [OData](http://www.odata.org/) service to reflect recent changes in the  ontology. And he's been working with Sarah to get more committee data into the platform. This new data is also available in the OData service.

Jianhan and [Samu](https://twitter.com/langsamu) uncovered what they think might be a bug in the library we use for creating the OData service. They've written some code to reproduce and might file a report once they're a little more confident.

Raphael created an automated import process for [Parliamentary period](https://beta.parliament.uk/parliaments) data, which hitherto had been hard-coded. This includes the [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) IDs kindly supplied by [Andrew Gray](https://twitter.com/generalising). Which Michael is still extremely excited about.

Matthieu, Mike and Samu gained access to the current hosting infrastructure for [Historic Hansard](http://hansard.millbanksystems.com/). They're working on plans to migrate it to a new home on our data platform, in a similar way to data.parliament and Indexing & Search.

Samu and Wojciech spent some time [(re)naming things](https://martinfowler.com/bliki/TwoHardThings.html). We periodically review our API endpoints, code namespaces and package names to align the naming guidelines with our evolving understanding of the service we're building. Here's what they came up with:

* api.parliament.uk/query - previously called the fixed-query API, these are the endpoints that supply the new website with data

* api.parliament.uk/sparql - not yet public, this provides a raw query endpoint for those in the need and the know

* api.parliament.uk/search - as the name suggest, this makes the new search service work

* api.parliament.uk/photo - Members' and Peers' portraits

* api.parliament.uk/odata - a standard interface that allows all our data to be pulled into spreadsheets for example

Wojciech and Liz looked at a new package for exporting our analytics data to a new blob store. Wojciech set up a test query showing page data and sent it straight to our visualisation software as a dataset. Other options are being explored.

### Data toolkit

Matthieu and Samu managed to install some new [SKOS](https://www.w3.org/2004/02/skos/) management software on our cloud infrastructure and import the [current controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri). They also came up with a longer term plan for migrating the vocabulary whilst not interrupting the authoring and indexing work that relies on it.

### Migrating data.parliament

Samu, Wojciech and Mike migrated [data.parliament](http://www.data.parliament.uk/) to its new home in the cloud. Seven [virtual machines](https://en.wikipedia.org/wiki/Virtual_machine) were replaced with two service plans. Which means it's about 85% cheaper to run. They also replaced some of the parts that were acting as bottlenecks. Content now reaches our external database 27 times faster. We're using the latest versions of all the software including the same version of the triple store as the new data platform - but with many more statements. So we've learned a bunch of stuff about big repositories and running a triplestore in an app service that will help us in the future . We no longer have to use a custom cache to cope with the current load on the services and integration with analytics gives us better monitoring, better logging, and etc. Because the new instance is in our own subscription, we have full control over everything there, no more asking (and paying) a 3rd party to do things like: scale up disk sizes, VM specs, open firewall ports, handle user access, etc.

### Corporate data

[Matt](https://twitter.com/matiasgermanico) continued work on the House of Commons HR system. The new integration is currently being tested with live data. A data comparison is being done to verify the amount of records being amended by the feed.

He also worked on the asset management system and tweaked the cost centre feed. All the other feeds (people details, asset usage) have now been successfully tested.

Noel got his hands on job information from the House of Commons HR system. He's now analysing this against data in the central pot to identify differences and understand why they exist. He's also provided a list of active users and their departments to the people responsible for our subscriptions to mailing and newspaper platforms.
 
David has been implementing the new facilities person interface and is currently working on the organisation interface.
 
Lewis continued work on a new finance and stock integration by developing and starting to test the new invoice data flow.

### Excellent customer service award...

...this week, like every week, goes to Mike who helped a commercial third party wanting to use data around [Research Briefings](https://researchbriefings.parliament.uk/). Maybe they'll switch to the data.parliament API instead of screen scraping the website....

### Are topics fashionable?

Hopefully, not so much.

### Did anyone on the internet confuse Parliament with government?

Whilst we did not witness this, we're fairly sure it must have happened. Anya and Michael did manage to increase the population count of people who now know Parliament != government by four. Which is a small achievement. But not unrewarding.

### Did Michael get headhunted?

Yes, Michael did get headhunted. Unfortunately it was for [the job he does in the organisation he works for](https://twitter.com/fantasticlife/status/960123698723348480), but, given no-one has ever expressed an interest in the past, he's still rather thrilled.

### Strolls

No strolls were reported, though Robert did go round to Dan's for dinner. Dan managed not to poison anybody. Anya, Ben and Michael are all looking forward to lunch with Robert tomorrow.

### Things that caught our eye

* [Blue Banana](https://en.wikipedia.org/wiki/Blue_Banana)

* [A reintroduction to Google’s featured snippets](https://www.blog.google/products/search/reintroduction-googles-featured-snippets/)