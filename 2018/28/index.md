
## 2018 Week 28

Despite a few team members taking holiday, a lengthy evacuation due to a fire alarm, football not coming home, and the visit of Donald Trump, the Data and Search team has had a busy and productive week.


### Showing and telling...

[Dan](https://twitter.com/dasbarrett) stepped into the Show and Tell spotlight this week, talking about his developing Data Strategy. He has set up a weekly Thursday morning open session at 9.30 to discuss this as it evolves.

### Community

Our Liz and Dan went to the [ODI](https://theodi.org/) for a course on [data ethics](https://theodi.org/article/data-ethics-canvas/). Dan thought it was both excellent and thought-provoking. Having done training with them before, Liz did too.

Dan went to [Hackney Council](https://hackney.gov.uk/) to meet [Cate McLaurin](https://twitter.com/madebycatem), Head of Delivery, and [Matthew Cain](https://twitter.com/mcaino), Head of Digital and Data. They had a good talk about the respective challenges and similarities in their work, and identified similar experiences with the problems of reporting versus analysis. Dan expects to be going back before too long.

### One world, one web, one team

Dan went to the Data Steering Group meeting where they talked about the data strategy. Various senior people from the Lords and Commons were there. They made lots of good suggestions and were really generous with their time and thoughts. Dan thinks [data dictionaries](https://en.wikipedia.org/wiki/Data_dictionary) might be coming back with a vengeance!

One of [Michael](https://twitter.com/fantasticlife)'s [blog posts](http://smethur.st/posts/176135867) was referenced by the [Chamber and Committees Team (CCT)](https://www.parliament.uk/mps-lords-and-offices/offices/commons/teams/#jump-link-0) Digital Board. Unfortunately, they spelled his name incorrectly. Michael has had worse misrepresentations of his name from his doctor's receptionist. But we won't go there.

[Alison](https://twitter.com/oliala) and [Bridget](https://twitter.com/keam_bridget) met with Suzanne for a demo of the Planon workspace management application and how it is being implemented for arranging moves of people within spaces in Parliament. Alison and Bridget also met and discussed reference data for location.

[Matt R](https://www.linkedin.com/in/matthew-reed-b3b761105/) met with a number of programme managers to explore opportunities for data analysis within their areas.

Alison discussed options with Alex for improving the online shop navigation and tagging, to make finding that [Theresa May Toby Jug](https://www.shop.parliament.uk/products/30365) just that little bit easier.

Dan and Liz did a sift for data analyst interviews next week. They're keeping their fingers crossed. Dan also put on his "Service Owner for Interaction Management" hat and worked on how to set up a new development team.


### Domain modelling

Michael made a bit of a document model for research briefings that still needs checking by [Anya](https://twitter.com/bitten_) and Robert. The document model is [here](https://ukparliament.github.io/ontologies/document/document-ontology.html) but not complete.

After a chat with [Jack](https://twitter.com/jackpdent), Michael changed the [made](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/made-affirmative.pdf) and [draft](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/draft-affirmative.pdf) affirmative procedure flows to improve the modelling of [deferred divisions](https://www.parliament.uk/site-information/glossary/deferred-divisions/), but got confused about self-preclusion. He has also done some more wrangling around [Rush data](https://ukparliament.github.io/weeknotes.data-search).

Anya and Michael met with Gail Poulton, Catherine Meredith and Kevin Gardner from the [House of Commons Table and Public Bill Offices](https://www.parliament.uk/mps-lords-and-offices/offices/commons/teams/#jump-link-0) to talk about commonalities in [tableable things](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html). [Ben](https://twitter.com/benwoodhams) was supposed to be there too to cover the Lords. But he wasn't. Ben claims he turned up when they were all away at lunch, which seemed to him the most sensible time to arrive. In any case, they had to make do without him. Despite this, issues around parliamentary questions, motions, motion amendments and bill amendments now seem clearer. Next steps will involve looking into timetabling.

Anya, Alison and Michael met with Matthew Keep and [Cassie Barton](https://twitter.com/cassier_b). Cassie and Matthew look after constituency level statistics in the House of Commons Library. This follows on from some work our Liz has been doing with library people around constituency statistics. Anya and Michael have made a second and hopefully improved version of the [stats series model](https://ukparliament.github.io/ontologies/stats-series/stats-series-ontology.html). The comments may still need some work.

Alison, Sarah and Franny met with Matt Morgan, Giles Mason, Ian Lacey and Amy Treble from Visiting and [Democratic Access](https://www.parliament.uk/visiting/visiting-and-tours/tours-of-parliament/tours/) to model the ways non-parliament people can visit Parliament.

### On search. And indeed indexing

[Sara](https://twitter.com/sarafreis) is still working on matching search terms with the Indexing and Data Management Section (IDMS) controlled vocabulary. [Anya](https://twitter.com/bitten_) and [Liz Marley](https://twitter.com/greensideknits) gave her some really useful feedback.
We had been matching the search terms against the preferred terms, but preferred terms also have related acronyms and non-preferred terms. For example, for [concept 8483](http://eldaddp.azurewebsites.net/terms/8483), "Avian influenza" is the preferred term, and “Bird flu” is a non-preferred term. So now we have added the non-preferred terms to the analysis. This will allow us to compare matches between search terms and preferred terms, and search terms and non-preferred terms. We'll report on these once the analysis is completed.

Our Liz caught up with Robert on hints, search terms and taxonomy. They also had a chat with [Jamie](https://twitter.com/oddtype) about how to support decisions on whether to remove unhelpful summaries for results.

Liz noticed some changes to the operation names in appInsights for search requests. She enlisted Wojciech's help. They discovered that, due to changes made when website search went live, website and public use of the api are captured as the same operation name. Liz says we need to use the Product Name (a custom dimension) to distinguish between them ('live-public-search' and 'a long string of numbers and letters'). They found something strange in the url being captured at request. A lot are coming through like [this](https://api.parliament.uk/search?q=System.Collections.ArrayList&start=1&count=10), which seems to have been happening for a while.


### Corporate data

Noel has been doing work to identify an issue with People Data that is causing people records to be constantly republished. He has also requested several testing servers for the team so that new and existing integrations can be developed and tested in a controlled environment.

Meanwhile, David has been working on Planon. He's been testing the "person space" integration to ensure that the correct information is displayed. Lewis has been trying to improve the resilience of the stock system integration by preventing potential duplication of invoices. He is finding that BizTalk’s technical limitations are making this task very challenging. Good luck Lewis!


### Employee of the week award...

... goes to both Mike and Wojciech for fixing a problem with Bills data on [data.parliament.uk](http://www.data.parliament.uk/). Runner up prize goes to Dan, for volunteering to fill in every week that there isn't something on the Show and Tell agenda.

### Strolls

The strolls have a somewhat regal theme this week. Once the weather had cooled slightly, Anya, Robert and Michael went for a stroll through various parks. Anya and Michael paddled in [Princess Diana’s fountain](https://www.royalparks.org.uk/parks/hyde-park/things-to-see-and-do/memorials,-fountains-and-statues/diana-memorial-fountain). This was Michael's second royal encounter in a week. Earlier in the week, he took an opportunistic stroll to see the Queen, Camilla and extended family when he heard they were in the neighbourhood. He saw them all. He thought it was brilliant.


### Things that caught our eye

* [7 Steps to Reliable Web Analytics Data](https://www.locallyoptimistic.com/post/web-analytics-process/)
* [Women Invent the Future – Doteveryone – Medium](https://medium.com/doteveryone/women-invent-the-future-84809ff2c8d2)

* [From Maps to Apps: the Power of Machine Learning and Artificial Intelligence for Regulators](https://fca.org.uk/publication/documents/from-maps-to-apps.pdf)









```
