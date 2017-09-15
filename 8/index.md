## Week 8: 15-09-2017

### Community

Last night was our [4th Parliament, data and democracy meetup](https://attending.io/events/parliament-data-and-democracy-meetup-4) at [Newspeak House](https://www.nwspk.com/). Thanks to everyone who came along and to our speakers. It was a good night with talks from:

* [Our Dan](https://twitter.com/dasbarrett) on where [we're at with Data and Search](https://docs.google.com/presentation/d/1BA3APE7JjZ-jusuZjO_UMb6CwI5JI1cUnBctfIQK8TE/edit). And how bloody difficult everything is.

* [Anna Scott](https://twitter.com/Anna_D_Scott) from the [ODI](https://theodi.org/) on [open data for democracy](https://docs.google.com/presentation/d/1zq_HuYESyLkiHYEfEdKUfiiKPQj1OFK8TFMVh8_bP7A/edit#slide=id.g2623662c47_0_57)

* [Rachel Coldicutt](https://twitter.com/rachelcoldicutt) from [doteveryone](https://doteveryone.org.uk/) on [building a better internet and better technology culture](https://docs.google.com/presentation/d/1DUDG7cwGxyYTWQz8tSDuXYRP-WIVIeM3nukDtA1WXqQ/edit#slide=id.g262a9c6907_0_1452)

* [Our Samu](https://twitter.com/langsamu) on the [new Parliament data platform](https://www.slideshare.net/UKParliData/a-new-data-platform-for-parliament-79810322/).

There was beer and chatter. You should come along one day. And if you'd like to hear a talk or give a talk or just say hello, [our mailing list is here](mailto:uk-parliament-data@googlegroups.com).



### Data day

All told data day was a "punishing hell ride". Dan had a bit of a reversion and went into project manager mode. We like to think this was well received by colleagues.

On the plus side things were agreed:

* we'll work with Ben to come up with a proposal for "Lords inflation" (don't ask)

* Anya and Michael will pick up the government departments, positions and incumbencies domain modelling in preparation for that being needed on member pages

* we need a new approach for delivering links to MPs websites. A ridiculously simple feature made almost impossible by the brittleness of downstream systems. New work should include social media links.

* we'll do any ongoing fixes / take downs for the new members' photos

* [Aidan](https://twitter.com/aidan_morgan) will arrange a meeting with the Ordnance Survey to discuss long-standing issues with region, constituency and postcode data
 
* we'll work with the members website team to break down the stories for showing votes on member pages

* we'll work with the committees website team to collaboratively design new data sources for information missing from existing systems

* we'll prepare for committing to stable identifiers very, very soon

* we'll investigate the impact of removing upper case letters and vowels (to avoid [inadvertent swears](http://www.bbc.co.uk/programmes/b0110ck3)) would have on the length of identifiers. [Jianhan](https://twitter.com/jianhanzhu) is about to do maths

### Parliament in the area, we're international, we're continental

Dan presented to a delegation from the [Lok Sabha](http://loksabha.nic.in/) (the lower house of India's bicameral Parliament). Mainly around data and search but also technology in general, and publications, and archives, and broadcasting. One of the delegates said Dan had "...a scholarly look, like Karl Marx" . This pleased Dan enourmously.

[Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) met with [Rose Rees Jones](https://twitter.com/rosebotanic) who's doing a piece of work for the ODI around the challenges of adopting and proposing data standards. They grumbled a bit but it was very useful.


### Domain modelling

Michael spent Monday diving into [Oli](https://twitter.com/olihawkins)'s election candidate database and wrapping a Rails app around it. He made some [pictures of gender splits](https://twitter.com/fantasticlife/status/907955346660102145) that he felt might be indicative but were somewhat drowned in caveats.

He had many conversations with assorted people about the problems we face with joint inquiries given the state of our current data model and the way it forces people to double and triple enter the same information. He's hoping to get some internal user research happening around this.

He also went along with the website team who did a show and tell to House of Commons committee people. Again he banged on about the problems with existing data models and joint inquiries and joint evidence sessions. He came to the conclusion that 90% of his job is asking dumb questions about cardinality.


### Data quality

Angela and [Raphael](https://twitter.com/raphaelleung) met with Jacqui Cooksey from the House of Commons to go through the current state of select committee data in the Members Names Information Service. They discussed possible solutions to tidying and ingesting the data. They also discussed data ownership and update frequencies for committee data currently only found in the website CMS.

Samu, [Ben](https://twitter.com/langsamu) and Michael met to discuss an approach to "Lords inflation". This is both too difficult and too tedious to explain but there is a plan and it will establish a more firm footing for House of Lords member data.

Samu worked with Angela and [Ed](https://twitter.com/ewhitur) from the website team. He designed a database and data entry form for recording committee data. This will be further developed and maintained by Angela, and will be used to record data that's not available in existing committee systems.

### Data platform

Samu made substantial improvements to the API that serves the new website. [SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries can now be extracted out of the application code and into separate files making it much easier for web developers to write, test and deploy the queries. Developers seemed pleased with this.

### Search

Feedback on search, which was at first a trickle, is now a flood. Thankfully expert colleagues are helping to manage, disseminate and analyse this information. 

There was a first meeting on how to deal with the search feedback; early days but all seems to be headed in the right direction. Wider proposals on search, including the search-of-beta, are beginning to be discussed. 

Robert met with a Commons Library colleague to hear about the data science work they’re starting and also discussed inference and text analysis. He also spoke with various people about how to add useful ‘hints’ to search results, in the form of labels.

Robert and [Dia](https://twitter.com/DN78) met [Laurence](https://twitter.com/laurencegrinyer) to talk through the proposal for searching the beta website.

### Machines that do learning

Dan met with Oli Hawkins to talk about the Commons Library establishing a data science function.

Raphael went over to [GDS](https://gds.blog.gov.uk/) as part of his data science accelerator course. He worked on implementing feedback for a [retraining pipeline](https://lcyraphael.github.io/img/mlpipeline.pdf) and looked at [multiclass decision forests](https://www.ncbi.nlm.nih.gov/pubmed/15585126) (not a clue, mate).

### Measuring things

Saffiyah spent the week looking at ways of using APIs and [Webhooks](https://en.wikipedia.org/wiki/Webhook) to  automatically grab data from our survey software.

She also continued to work on establishing metrics for the House of Commons Library Enquiries service.

Sara and Dia met to talk about search feedback. Sara made changes on the report for monitoring search API performance. She also looked at clustering techniques to define user types based on their journeys around the website.

Liz started a search feedback and measures log to help inform decisions about future testing and record a history of changes and caveats which might influence measurements made and conclusions drawn. She started to look at the two feedback polls for search. Data requires cleaning and there's work on how to categorise comments. As much as possible will be automated and summarised weekly whilst the polls are running. The aim is to use this information to understand possible areas for development.

### Excellent customer service awards

Mike compiled a CSV of data back to 2000 to help a PhD student from the [Federal University of Minas Gerais](https://en.wikipedia.org/wiki/Federal_University_of_Minas_Gerais) in Brazil with their thesis on gender equality representation in the British House of Commons.

### Capability

[Julie](https://twitter.com/julietouring) presented her thoughts and potential options for how to take forward the capability work to the senior management team.

Julie and Mike attended a DevOps Journey presentation by the British Medical Journal. It was followed by a really useful discussion about culture, challenges and our current situation across assorted development / technology teams.

### Corporate data

[Matias](https://twitter.com/matiasgermanico) and David attended a people data workshop organised by Tori. There were people from a variety of teams across Parliament.

The general consensus was that:

* There's a need to redesign the People Data service

* Current processes and workflows have to be reviewed

* Business teams need to understand that the data they produce has an impact on other parts of the organisation

* Data on source systems has to be consistent

* A single identifier should be used wherever possible

* A new standard data model of a person should be created


### Strolls

Robert and Michael went for a stroll in St James's Park. Talk turned once again to hypertext and their general belief that 95% of improving search comes from improving browse. They also chatted about how we haven't quite properly explained what we've done with the new search and what implications that has and the various advantages and disadvantages. There is still a blog post or something missing here. Michael has promised to type words. When his hangover dissipates. If. 

They also chatted about "digital transformation" (whatever that is) and came to the conclusion that it only usually works if it's emergent from internal organisational change and rarely works by driving stakes into ground from the outside. This is a problem.

No other strolls were reported.

### Things that caught our eye

* [Westminster Bubble - What Westminster journalists are tweeting about, summarised in one word cloud a day](https://twitter.com/wmbubble)

* [What machines can tell from your face (is terrifying)](https://www.economist.com/news/leaders/21728617-life-age-facial-recognition-what-machines-can-tell-your-face)

* [Calculating the average face of a UK Member of Parliament](https://medium.com/@puntofisso/i-calculated-the-average-face-of-a-uk-member-of-parliament-and-heres-what-i-found-37f31b72b5d9)

* Catalogues and Context (a talk from Karen Coyle)[https://kcoyle.net/catcon.html]

* [The Difference Between AI, Machine Learning, and Deep Learning?](https://blogs.nvidia.com/blog/2016/07/29/whats-difference-artificial-intelligence-machine-learning-deep-learning-ai/)

* [Calling Bullshit on the machine learning sexual orientation research](http://callingbullshit.org/case_studies/case_study_ml_sexual_orientation.html)

* [MIT research analysing emoji with neural networks is none too shabby at detecting sarcasm](https://github.com/bfelbo/DeepMoji)

* [To balance out this machine learning discussion](https://xkcd.com/1875/)

* [A Case study on Burkina Faso’s open elections by Anna Scott of the ODI](https://theodi.org/case-study-burkina-fasos-open-elections)


