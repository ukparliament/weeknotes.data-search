## 2018 Week 04


### [Christmas cake, it's 38](https://www.youtube.com/watch?v=u3ZvO4pcTHs)

Wednesday was [dator day 38](https://twitter.com/dasbarrett/status/958745516371775489). Which was fine. We even got through the agenda. The bit around commitments for the website took a while but the outcome was clear and it looks like an achievable amount of work for next two weeks. It was good to have [Jamie](https://twitter.com/oddtype), [Caroline](https://twitter.com/carolinekippler) and Sarah with us.

Some stuff that was agreed:

* the big priority for the next two weeks is getting [written question and answer](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) data into a state where features can be built and put into production on the beta website

* continued collaboration with the committees and Guide to Procedure teams to get features into production on the beta website

* helping to get Peers' portraits into the data platform and onto the beta website

* developing search hints for works of art and the new shop

* looking at open graph and similar 'standards'

Following on from dator day, [Dan](https://twitter.com/dasbarrett) gave the development team an update on priorities for the next two weeks. The team really got a lot of stuff done in the past fortnight.

### Community

Dan went along to [Teacamp](https://teacamplondon.com/) and heard about [digital work in health](https://twitter.com/dasbarrett/status/959139568330166273). It was a good dose of perspective and made him realise that Parliament isn't really all that hard.

### Corpcomms

Imagine you're in a bar. It's Paris in the mid 1930s. At the next table there's a group of blokes, going by the names Joyce, Hemingway, Beckett, Pound, Eliot and Yeats. If you stay quiet enough you can eavesdrop. That's what Yammer's like. But you'll have to take our word for it.

### One world, one web, one team

Dan has been working on the 'data strategy' for Parliament and has had helpful discussions with [Vincent](https://twitter.com/VRousselet). He's trying to strike the magic balance between enterprise IT and the stuff with personality and a democratic mission. Aren't we all.

Wojciech made a change to our data service infrastructure. It means uptime for our services on [beta.parliament.uk](https://beta.parliament.uk/) and [new search](https://beta.parliament.uk/search) will be improved. Wojciech was awake at 5.30am to make this happen. Some commitment here.

Saffiyah had a meeting on useful digital tools for people with dyslexia and dyspraxia.

### Domain modelling

[Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver), [Ben](https://twitter.com/benwoodhams) and [Michael](https://twitter.com/fantasticlife) continued to dig into [secondary legislation](http://www.parliament.uk/business/bills-and-legislation/secondary-legislation/) and updated their flow charts for the [House of Commons](https://github.com/ukparliament/domain-models/blob/master/SIs/flow-commons.pdf) and [House of Lords](https://github.com/ukparliament/domain-models/blob/master/SIs/flow-lords.pdf). These still need to be idiot checked. The next step is turning all that into a data model. Silver seems to think this should be easy. Michael is, as yet, less convinced.

Anya and Michael made some changes to the comments on the [time period model](https://ukparliament.github.io/ontologies/time-period/time-period-ontology.html) following several emails and fag break chats with Paul Evans. They also made a couple of minor tweaks to the [question and answer](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) and [tabling](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html) models.

They had a good conversation with Gini Griffin from the House of Commons Table Office about whether [round robin questions](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html#d4e44) could be treated as a single question with multiple answers. This would be a major change to existing practice and mean removing mentions of the gender of the answering minister. So, at least for now, it doesn't seem likely.

Liz introduced Michael to Matthew Keep from the House of Commons Library. They're looking for better ways to self-serve constituency information. We've suggested that part of the answer should involve adding constituency demographic data to the data platform. Michael is going to take a look at modelling some of the data we already have. In the long term it would open up an opportunity for the Library to ask questions like: give me questions from session x, on topic y from members representing constituencies with demographic z. Which would make all this linked data stuff actually worthwhile.

### Data platform

Our [OData](http://www.odata.org/) API has been listed by [pragmatiqa.com](https://pragmatiqa.com/) which provides a rather nice [visualisation of our data](https://pragmatiqa.com/xodata/?url=https://api.parliament.uk/Staging/odata/$metadata). It's a good place to start if you want to see what we have so far.

[Chris](https://twitter.com/chrisalcockdev) spent lots of time fiddling with our [headless CMS](https://en.wikipedia.org/wiki/Headless_CMS) which will eventually become a component in the data platform. He's been working with the Indexing and Data Management Section (IDMS) in the House of Commons Library and the Guide to Procedure product team. The result is an API endpoint serving information about [Concepts](https://www.w3.org/2009/08/skos-reference/skos.html#Concept), their definitions, their connections to other concepts and their connections to Guide to Procedure articles. Big shout out in particular to [Liz Marley](https://twitter.com/greensideknits) who extracted a subset of [Parliament thesauri](http://www.data.parliament.uk/dataset/thesauri) Concepts, indexed the articles and is currently writing scope notes.

Progress has continued on the more conceptual elements of the data toolkit, including technical investigations and understanding requirements. The first component will be a new system for IDMS, allowing them to manage their taxonomy. This is a critical enabler for 'topics' on the new website.

[Jianhan](https://twitter.com/jianhanzhu) worked with Wojciech and [Samu](https://twitter.com/langsamu) to create an 'interim data source' to provide committee data which is either not in the Members' Names Information Service (MNIS) or is in MNIS but is incorrect and can't be fixed. To help editors, this has been pre-populated with data from MNIS where possible. The orchestration has also been deployed to grab data from the interim data source and push it to the data platform. Progress on getting this into website production is reliant on the product team filling in the data source and either creating new queries or working with Data and Search to create them.

Chris has been working on importing Government Organisation data into the platform. Queries still need to be created to get this information onto the website. He's now chatting to Anya about answering bodies. There's some fuzziness here because whilst all committees, government organisations, government departments and answering bodies are groups, not all government organisations are government departments, not all answering bodies are government departments and some but not all committees are answering bodies. And we haven't even got to laying bodies yet. Our world is full of non-exclusive sets. Despite its detractors, at this point we'd like to express our gratitude to [RDF](https://en.wikipedia.org/wiki/Resource_Description_Framework).

[Raphael](https://twitter.com/RaphaelLeung) has started to look at importing Wikidata identifiers for [parliament periods](https://beta.parliament.uk/parliaments). Michael feels this will be very cool.

The migration of [data.parliament.uk](http://www.data.parliament.uk/) to her new hosting environment happened. Which is a big deal in terms of saving public money. There were a few bumps in the road, but that's to be expected.

### Search


#### Web search

Dan finally did some actual search leadership, making a decision about some new features for a public website for the first time in possibly ever. He's still bitter that didn't even get to say 'no' to the [data.parliament.uk](http://www.data.parliament.uk/) carousel. And that's like a decade ago. He's also asked for input from design colleagues.

Raphael added some server side tracking and we can now see the hints returned for the results of a search. It's a custom event and in testing we found that [a search result can be a search result](https://en.wikipedia.org/wiki/Turtles_all_the_way_down). This is currently being fixed in [robots.txt](http://www.robotstxt.org/). Sara is using the tracking to build on the work to evaluate hints by URLs.

We've decided to release [Research Briefing](https://researchbriefings.parliament.uk/) search hints in order to generate data and feedback. We'll use that to refine what the hints are called and which ones to keep or remove. Liz has requested [Second Reading](https://secondreading.parliament.uk/) hints which Raphael has since added.


#### Parliamentary search

Saffiyah, Liz and Sara met with [Alex](https://twitter.com/alexedwardh) to explore the Search and Indexing triple store and [Solr index](http://lucene.apache.org/solr/). They'd like a way to easily export and store data. Anya and Michael would also like this to continue with plans to interlink the Parliament thesauri with [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page). A plan is emergent. 

### Measuring things

Samu and Wojciech turned on continuous export for our analytics package, which now gives us access to more than 90 days worth of data.

Liz taked to Jane in corporate services about how we plan to remove the need for a SharePoint repository for their KPI data. We want to bring all KPI data into a staging area and connect to their current sources (spreadsheets mostly), removing the need for them to re-enter information. Since everyone hates the SharePoint solution, they seem happy with the proposal.

### Corporate data

[Matt](https://twitter.com/alexedwardhmatiasgermanico) continued work on the House of Commons HR system integration. He's completed isolated testing including extraction of people data. Full testing has now started. As a part of that he'll verify the policies that perform the data matching and get a comparison of People Data records before and after running the feed.

Matt's also been building the feeds to send People Data, cost centres and hardware asset usage to the assets management system. These feeds need to be tested by the Information Systems Team. We await the results.

Noel's been conducting a review of data surrounding job information and identifying a way of making sure that our mangament chain information is accurate. He's created a query of users managerial information as stored on People Data. The information has been passed on to Liz and Saffiyah for analysis. He's also been looking at records whose matching has been placed on hold and created a query that improves the identification of potential matched records.
 
David's been reviewing the scripts involved with processing job information from the House the Lords HR system. He's aiming to fix the problem where some managerial information is not being fully populated.

Lewis has been developing the new stock system integration. He's built a robust authentication module that can be used by the other four systems to make API calls.

### Excellent customer service award...

...again goes to Mike who continues to boss the customer service game, this time doubling up with Raphael like the Utah Jazz's [Stockton and Malone](http://www.complex.com/sports/2012/03/the-15-best-duos-in-nba-history/duos-10). Questions were answered on a Hansard / data science tip. Mike went on to cover general enquiries about [data.parliament](http://www.data.parliament.uk/) like a champ.

### Are topics fashionable?

Yes. Yes they are. For one brief moment it looked like putting telly on web pages might overtake them. Which brought back particularly bad memories for Michael. But now topics are back. With a vengeance. Bigly.

On the subject of telly, Dan and Robert kicked around casting ideas for 'Data and Search - the movie'. Derek Jacobi, Bill Nighy, Christian Bale, Mark Gatiss, Russell Crowe, Mark Ruffalo, Meryl Streep, Zach Galifianakis, Jessica Chastain and more featured in a stellar but generationally challenged hypothetical cast. Not a clue here.

### Did anyone on the internet confuse Parliament with government?

Yes. That did happen.

### Strolls

Nada. Nothing. Zilch. Not a stroll in sight.

### Things that caught our eye

* [We Can’t Do That In One Sprint](https://hackernoon.com/we-cant-do-that-in-one-sprint-a6780d67480)

* [We Need Fewer Product Managers](https://hackernoon.com/we-need-fewer-product-managers-50e47dfd95a0)

* [Legislative Openness Data Explorer](https://beta.openparldata.org/)

* [Improving ‘Find’ for the Find Property Information Service](https://medium.com/@IanAmes/improving-find-for-the-find-property-information-service-6d2cb50728ee?source=linkShare-4cd140afefc2-1517485283)

* [JSON-LD and Why I Hate the Semantic Web](http://manu.sporny.org/2014/json-ld-origins-2/)

* [Electronium - an early combined electronic synthesizer and algorithmic composition / generative music machine](https://en.wikipedia.org/wiki/Electronium)

* [Moving a legacy Microsoft environment to the Azure cloud](https://18f.gsa.gov/2018/02/01/moving-a-legacy-microsoft-environment-to-the-azure-cloud/)

* [CommanderSong: A Systematic Approach for Practical Adversarial Voice Recognition](https://arxiv.org/abs/1801.08535)

* [Digital Deceit: The Technologies Behind Precision Propaganda on the Internet](https://www.newamerica.org/public-interest-technology/policy-papers/digitaldeceit/)