## Week 5: 25-08-2017

### Community

A reminder that our [4th Parliament, data and democracy meetup](https://attending.io/events/parliament-data-and-democracy-meetup-4) is on Thursday 14th September at [Newspeak House](https://www.nwspk.com/). 

There will be interesting talks, nice people and [free beer](https://www.howtogeek.com/howto/31717/what-do-the-phrases-free-speech-vs.-free-beer-really-mean/). You should probably come.




### Capability

[Raphael](https://twitter.com/raphaelleung) went to [GDS](https://gds.blog.gov.uk/) for the mid-point event in the data accelerator programme. He heard about progress of data science projects from other attendees and got feedback on a diagram he drew of implementing our machine learning and retraining pipeline.



### Domain modelling

[Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) went back to visit [Ganesh](https://twitter.com/gansenthi) at GDS. They chatted to a policy person about the flow of a policy from party manifesto through (possibly) to Parliament and (possibly) legislation. Came to the conclusion that what looks like a simple step flow on a diagram is probably some kind of insane [Sankey diagram](https://en.wikipedia.org/wiki/Sankey_diagram). So went to the pub.

### The URI is the thing

Michael spent time with [Colin](https://twitter.com/colinpattinson), Angela and some post-its to design a first draft of the URIs we'll need to support committee membership. Michael forgot to document this. Michael will document this. Soon.



### Data service

[Chris](https://twitter.com/chrisalcockdev) implemented a solid if very basic select committee / formal body membership model in the physical ontology and created a mock API for the website team to develop against. He also attempted to progress the select committee / formal body membership model to allow for chairs etc and ran into a long-fomenting name clash on "Incumbency" that needs some real work so will have to wait.

[Samu](https://twitter.com/langsamu) was encouraged to publish his triple visualiser as a chrome extension for the purposes of fun and profit.

Mike had Alex, our new operations person, in and we talked to him about our work.

[Jianhan](https://twitter.com/jianhanzhu) continued with experiments to pipe data from internal databases to our data store on the cloud. He set up a pipeline for House of Commons Library enquiry data. This allows for direct database access unlike most of our other data ingest processes that rely on the presence of an [OData API](http://www.odata.org/) [warning: clip art].

Jianhan and Angela worked with colleagues from the House of Lords to further clean up committee data in the Members' Names Information Service (MNIS).

And Jianhan and Michael had a chat about how we link up Select Committees to the Government departments they scrutinise. This was found to be hard.

Raphael troubleshooted an issue with with the triple store workbench, the tool used by the website team to query the triple store.


### Search

Robert had an action-packed, if slightly short week. He met with [Dia](https://twitter.com/DN78) and Rachel from the communications team to discuss comms for the search roll out. And again with Dia on updates to the search release timetable.

There was a good hour spent on planning the next search sprint and a meeting between Robert and Samu on future search development.

Robert worked with user research colleagues on search research questions.

Matthieu coordinated with the website team for the search move to live.



### Measuring things

Sara created a dashboard / report to monitor API performance on search requests. She also started working with Saffiyah on the Library enquiries model. They're linking tables and creating measures at the moment.

Sara added [data.parliament.uk](http://www.data.parliament.uk/) to the analytics store which will allow us to analyse the raw data and track individual user journeys.

Lewis completed the spreadsheet to XML pipeline allowing us to process spreadsheet data directly in the service bus. This is about to be used to process information from our service incident database allowing the performance analysts to get more information on cases.

Project (and indeed programme) management office dashboards have been created allowing navigation from a general overview, to details on a programme to details on projects within a programme.

Sara, Saffiyah and Matthieu had a good chat about the current dashboard software.



### Strolls

Robert and Michael went for a long walking meeting round [Kew Gardens](https://www.kew.org/). Because they felt they deserved it. Much chat was had on data models and hypertext and search and browse and the making of websites. Being grumpy old men they agreed that everything was better in the old days when it was [all more punk](https://www.youtube.com/watch?v=78S0yrMLfTU) and before we got cursed with professionalisation.


### Things that caught our eye

* [Andrew Dudfield's post on open data, open standards and an open web](http://mrdudders.posthaven.com/open-the-data-save-the-world) is excellent

* [An introduction to the new ONS beta API](http://digitalblog.ons.gov.uk/2017/07/13/api-an-introduction/)

* [Some stuff on Microsoft's ventures into AI](https://www.pluralsight.com/blog/software-development/microsoft-ai-tools-2018?mkt_tok=eyJpIjoiTUdObE1EWXhZelZrTldKbSIsInQiOiJtMFwvV2dMYndnK3BpdVlTVjM0MnU3MWloQ3JqMEFvdm81TUpZbzNPTmVDZ09iR012Rlk5OCsraDF3MDl2REdrcGJRdURtWjhyd2JIQXg1NmJna3RGaGtOTVwvQ0N1aUlNYWQxRXJKOW1yUk8rSmszajAyeEFhbGpOMXRRM2lzQUZrIn0%3D&oid=&promo=&utm_campaign=nl-w-a-082317&utm_content=&utm_medium=email&utm_source=marketo&utm_term=&vid=7010a000002BeZdAAK). God, that's a terrible URL

* [A new digital strategy for the National Archives](http://www.nationalarchives.gov.uk/about/our-role/plans-policies-performance-and-projects/our-plans/digital-strategy/)

* [Some security guidance for obsolete platforms](https://www.ncsc.gov.uk/guidance/obsolete-platforms-security-guidance)

* [What a digital organisation looks like](https://medium.com/doteveryone/what-a-digital-organisation-looks-like-82426a210ab8). Still not sure I'm any clearer

* [An AI from the Alan Turing Institute to recognise beauty in scenery](https://www.turing.ac.uk/media/news/ai-trained-recognise-beautiful-scenery/)

* [An interesting article about amplification of bias in training datasets (or why an image of a man cooking in a kitchen may be detected as a woman) and a possible solution](https://www.cs.virginia.edu/~vicente/files/bias.pdf)

* [An introduction to machine learning](https://medium.com/machine-learning-for-humans/why-machine-learning-matters-6164faf1df12) 

