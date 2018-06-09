## 2018 Week 23

### DATOR Day

After a short break [data day](https://twitter.com/dasbarrett/status/1004346497582985216) returned and [turned](https://m.youtube.com/watch?v=W4ga_M5Zdn4) 40. In its new format it only takes us half a day, but it’s still pretty much all about the data.  Aside from the gossip. And the scheming. There was a decent variety of stuff, but we [didn't quite get through it all](https://twitter.com/dasbarrett/status/1004398440489549825).

Some stuff we agreed:

* Instead of implementing [Google Tag Manager](https://en.wikipedia.org/wiki/Google_Tag_Manager) on [Parliamentary Search](http://search-material.parliament.uk/) we'll work to understand the compliance requirement, and implement [Application Insights](https://docs.microsoft.com/en-us/azure/application-insights/app-insights-overview) in a lightweight way that doesn't involve working with the legacy code.

* In terms of tracking [Statutory Instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) we think we have a fairly good idea on where to capture SI citations and statutory day counts. We still need an accurate calendar for sitting days in both Houses before we can calculate statutory days (previously [praying days](https://ukparliament.github.io/ontologies/time-period/time-period-ontology.html#d4e459)) and determine "deadline" dates for SIs.

* On the wider legislation front we still need help from external experts before [Michael](https://twitter.com/fantasticlife) feels any degree of confidence. The names [Richard Pope](https://twitter.com/richardjpope) and [Paul Downey](https://twitter.com/psd) were both mentioned. Michael thinks it might be a good point to get back in touch with [David Beamish](https://en.wikipedia.org/wiki/David_Beamish).

* Performance analysts won't be given direct access to Application Insights. Yet. But our Liz will be on hand to answer specific questions.

* On [GDPR](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation) compliance, the Members Names Information System (MNIS) interface should not be exposing dates of birth. When this change is made we need to review downstream systems.

### More visions

Very little in the way of visions this week. The cheese must be wearing off.

### Community

We were joined at data day by [Marc Adams](https://www.linkedin.com/in/dr-marc-adams-79081a144/) from the [NAO](https://www.nao.org.uk/) to chat about stats in general and plan some actual work we might do together. We're now looking for a guest for the next data day in July. Hands up if that might be you.

Some immediate, practical stuff we agreed to do with Marc:

* Michael to send over the straw man model for [constituency stats series](https://ukparliament.github.io/ontologies/stats-series/stats-series-ontology.html). Which is done, with a meeting in the planning.

* Marc to send over the Access database for the [ONS](https://www.ons.gov.uk/) history of constituency codes and splits and merges.

* The NAO to include Parliament constituency identifiers in their data service.

On a similar subject, our Liz has been helping colleagues in the [House of Commons Library](https://www.parliament.uk/commons-library) set up systems to produce new reporting pages for constituency stats. New features for a [constituency dashboard](https://commonslibrary.parliament.uk/local-data/constituency-dashboard/) and [topic based stats browsing](https://commonslibrary.parliament.uk/local-data-browse-by-topic/) went live on Thursday. They’re looking really good and people have been positive about them so far. Which doesn't stop Michael scowling at the URLs. And the "topics". That aside, the data is ripe for ingesting into the data platform, to allow for display on the [beta website](https://beta.parliament.uk/) [constituency pages](https://beta.parliament.uk/constituencies/cS887qfc). And open up new ways to query parliamentary material in a way that hasn't been anywhere near possible before. A meeting is planned.

Robert had a couple of meetings about developing search functions over websites. One with people from [ACAS](http://www.acas.org.uk/index.aspx?articleid=1461), one with people from the [Legislative Assembly of Ontario](https://www.ola.org/en). Properly international, if not continental.

[Matthieu](https://twitter.com/cognithive) published his [blog post about the trip he took with Sara to TICTeC](https://pds.blog.parliament.uk/2018/06/06/the-impact-of-civic-technology-thoughts-from-tictec/). If you're interested in the impact of civic technology, you should read it.

A data scientist called Izzy got in touch with Mike to share [her MSc project](https://github.com/izzyStewart/democratising-parliamentary-data). It pulls House of Commons divisions data from [data.parliament.uk](http://www.data.parliament.uk/) and analyses voting behaviour across Members.

### Domain modelling

[Alison](https://twitter.com/oliala) has been meeting lots of people and having chats with the Collaboration team about all things related to "visiting Parliament".

[Anya](https://twitter.com/bitten_) and Michael met with [Lef Apostolakis](https://www.linkedin.com/in/lef-apostolakis-835159a5/) from [POST](https://www.parliament.uk/post) to get another view on the work they've been doing to [model research briefings](https://github.com/ukparliament/ontologies/blob/master/document/document.png). They'd already done a couple of passes with assorted people from the House of Commons Library and still need to sit down with [House of Lords Library](https://www.parliament.uk/business/lords/work-of-the-house-of-lords/lords-library/) people. The POST session didn't change an awful lot, which is good news and suggests the model is mostly correct.

On Wednesday, there was yet another meeting on SIs and the tracking thereof. This one with Jane, Jack, [Jen](https://twitter.com/benwoodhams), Janya, Jichael and Jalison. Jenna and [James](https://twitter.com/thevinternet) being otherwise occupied. After several weeks they think they’ve finally cleared up their confusion around SI procedure clocks, the definition of statutory days and how to model statutory day counts. That said, there’s another meeting next week to definitely, finally, completely agree the last bit.

Anya and Michael went to visit Brighton to meet [Silver](https://twitter.com/silveroliver). Because he lives there. Or near there. And because it's the seaside. And because it has dodgems and air hockey. They [sat on the beach](https://twitter.com/fantasticlife/status/1004691294315274240) and planned out a talk they're due to give to [NetIKX](http://www.netikx.org/). Which was supposed to be an introduction to ontologies for librarians and knowledge management people, but has ended up as plea to switch from learning ontologies to learning about [domain modelling](https://en.wikipedia.org/wiki/Domain-driven_design) instead. So no one gets their money's worth there.

They also spent a bit of time talking about the Modelling Parliament talk they're due to give at the [KanDDDinsky conference](https://kandddinsky.de/) in Berlin. And some time talking about teaching House of Commons librarians a little more [SPARQL](https://en.wikipedia.org/wiki/SPARQL). The day ended, as many days do, in the [pub](https://www.tripadvisor.co.uk/Attraction_Review-g186273-d5913501-Reviews-The_Heart_and_Hand-Brighton_East_Sussex_England.html), hatching a plan for the first useful chunk of a legislation model. Which has been bothering Michael for some time.

### Data platform

In the best news for a quite a while, [procedure data](https://procedures.azurewebsites.net/) is now live and happily turning into pages on the beta website. Although for now and I guess for reasons(?), those pages are still restricted to the parliamentary network.

After herculean data entry efforts by IDMS, some monumental procedure modelling work, an INTERIM DATA SOURCE built from scratch by [Chris](https://twitter.com/chrisalcockdev), visualisations in two and three dimensions built by Raphael, a novel editorial interface built by Wojciech, all ably supported by Mike... we got there.

In the first instance we're only working with procedures for Statutory Instruments. In the longer term we think any parliamentary procedure could be captured in this way. This excites us, for we are a very niche brand of nerd.

Wojciech's done some sterling work to describe our Query API using the [Open API Specification](https://github.com/OAI/OpenAPI-Specification) aka [Swagger](https://en.wikipedia.org/wiki/Swagger_(software)). We're now publishing details of assorted endpoints, query parameters and [content negotiation](https://en.wikipedia.org/wiki/Content_negotiation) options in a standard, machine readable format.

Jianhan has been busy adding fixed query endpoints for [questions asked by a Member](https://api.parliament.uk/query/questions_askedby_member?member_id=https://id.parliament.uk/4fn7q5Wl) and [questions answered by a Member](https://api.parliament.uk/query/questions_answeredby_member?member_id=https://id.parliament.uk/SWXSOmi9).

He also updated the [OData](http://www.odata.org/) endpoints to reflect the newly imported [questions and answers](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) data. You can now get the [total number of questions](http://api.parliament.uk/OData/Question/$count), [total number of answers](https://api.parliament.uk/OData/Answer/$count), [questions by a Member](https://api.parliament.uk/OData/Member('0FqjjgNp')/AskingPersonHasQuestion), [answers by a Member](https://api.parliament.uk/OData/Member('0FqjjgNp')/AnsweringPersonHasAnswer), [questions asked on a date](https://api.parliament.uk/OData/Question?$filter=QuestionAskedAt%20eq%202018-05-23T00:00:00Z), [questions asked between two dates](https://api.parliament.uk/OData/Question?$filter=QuestionAskedAt%20gt%202018-04-23T00:00:00Z%20and%20QuestionAskedAt%20lt%202018-04-26T00:00:00Z), and [correcting answers expanded with corrected answers](https://api.parliament.uk/OData/CorrectingAnswer?$expand=AnswerReplacesAnswer). There's also a fixed query to return [questions by search terms in headings](https://api.parliament.uk/query/questions_search_by_title?lowercase_string=health).

[Samu](https://twitter.com/langsamu) made major improvements to the default HTML rendering of data from our API. It now shows [meaningful labels for resources, images for member photos](https://api.parliament.uk/query/person_by_id?person_id=43RHonMf), [maps for constituency areas](https://api.parliament.uk/query/constituency_map?constituency_id=JzQPzQpf), and improved styling for a better table display. Matthieu helped en route with several useful suggestions.

Samu had a busy week. He also added analytics to capture redirects from [hansard.millbanksystems.com](http://hansard.millbanksystems.com/) (the thing that search engines still have indexed) to the new [Historic Hansard](https://api.parliament.uk/historic-hansard/index.html). Liz has been looking at user IDs. There's been about 22,000 unique users per week in the last month.

### [Use hyperlinks to subvert hierarchy](https://en.wikipedia.org/wiki/The_Cluetrain_Manifesto#Thesis_7:_Hyperlinks_Subvert_Hierarchy)

The [lastest version](https://github.com/dotnetrdf/dotnetrdf/blob/v2.1.0/ChangeLog.txt) of [dotNetRDF](http://www.dotnetrdf.org/) was released this week. It's an open-source software library we both contribute to and [rely on](https://medium.com/@langsamu/api-parliament-uk-7b87597019a4). The new release contains a number of contributions by Samu:

* A new read-only [SKOS](https://en.wikipedia.org/wiki/Simple_Knowledge_Organization_System) API, inspired by Matthieu's work on transforming our controlled vocabulary to SKOS and building tools to replace and improve the software used by the Indexing and Data Management Section of the House of Commons Library.

* A new [GraphML](http://graphml.graphdrawing.org/) triplestore writer that converts RDF data into an XML format used in visualisation software. It was inspired by Raphael's work on visualising procedures for the SI tracker project.

* A new feature for the GraphViz writer (another RDF visualisation converter) that allows for the output of separate literal nodes. Also inspired by Raphael's work on procedure visualisation.

* A fix for date handling in the [JSON-LD](https://en.wikipedia.org/wiki/JSON-LD) parser which was inspired by our work on serving developer friendly hierarchic JSON-LD and RDF/XML from the query API.

* A bug report regarding incorrect HTML serialisation that Chris found whilst working on the procedure prototype. This resulted in the maintainers identifying and fixing a deeply hidden indexing optimisation bug in the library.

Based on the code we've contributed, our query API now supports GraphML output for all queries. Here's Jianhan's query giving the [Parliamentary questions answered by Lucy Frazer MP in a format that can be visualised](https://api.parliament.uk/query/questions_answeredby_member.graphml?member_id=SWXSOmi9) by software like [Gephi](https://gephi.org/).

### Corporate data

[Dan](https://twitter.com/dasbarrett)'s been working a fair bit with David, Lew, and Noel on all things data integration-y. They’ve been trying to improve the pipeline of work coming in and the quality of requests the pipes contain. They've also been trying to keep the endless email chains to a minimum and working out where we go next with our infrastructure.

David went off to the [Biztalk 360 Integrate 2018](https://www.biztalk360.com/integrate-2018/) conference and returned with an assortment of Biztalk stickers. Which at least makes a pleasant change from Users First and Being Bold.

Dan also got a new gig. As of Friday he is now both Head of Data and Search and *Service Owner – Interaction Management*. I have no idea what interaction management might be, but it sounds super. Well done Dan.

### Strolls

No strolls were reported this week. Though Anya, Silver and Michael did walk to the end of Brighton pier. Well, at least as far as the [dodgems](https://twitter.com/bitten_/status/1004722028719562752) anyway. Anya and Michael played air hockey. Anya whipped Michael's ass.

### Things that caught our eye

* [On the merits of Tidy Data](https://vita.had.co.nz/papers/tidy-data.pdf) [PDF]

* [Microsoft sinks data centre off Orkney](https://www.bbc.co.uk/news/technology-44368813)

* [The Golden State Warriors, the happiest team in sports](https://www.theguardian.com/sport/2016/jun/08/golden-state-warriors-happiest-team-in-sports-nba)

* [This is what the best of data journalism looks like](https://medium.com/data-journalism-awards/this-is-what-the-best-of-data-journalism-looks-like-6f1713d60479)

* [The Structural Properties of Online Social Networks and their Application Areas](http://www.iaeng.org/IJCS/issues_v43/issue_2/IJCS_43_2_03.pdf)

* [Transport for London Launches Bus Passenger Tracking Trial](http://www.gizmodo.co.uk/2018/06/transport-for-london-launches-bus-passenger-tracking-trial/)

* [I Love GDPR Spotify playlist](https://open.spotify.com/user/popjustice/playlist/5Pe51v0sHLybSEkX0m0JRf?si=eg4nfyhZTXepN_VTLnK9ZA)

* Liz liked this paper on [Workflow of statistical data analysis](https://www.kirchkamp.de/oekonometrie/pdf/wf-screen2.pdf) [PDF]. She liked the description of creative (undocumented) and permanent (documented). "Anything that we give to other people (collaborators, journals,...) must come entirely from permanent".