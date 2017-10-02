## Week 10: 29-09-2017

### Community

Wednesday saw a visit from [Benjy Stanton](https://twitter.com/benjystanton) of the [ONS](https://www.ons.gov.uk/). There was talk of potential collaboration on shared tools and lots of thoughts on a clubbing together of public sector organisations who publish things.

### Dator day

Wednesday was [dator day](https://twitter.com/fantasticlife/status/913833097355030528). For the first half it took too long to agree website work and there were a few unnecessarily disagreements. That said the outcome was constructive and we agreed some stuff:

* To have a first iteration of government roles live on the website by the end of the next Members sprint.

* To work with the website team to break down user stories around written questions.

* To investigate available data sources and systems for division (vote) data.

* To take a position on stable identifiers as soon as possible.

### Digital service quarterly event

[Dan](https://twitter.com/dasbarrett) spoke twice at the digital service quarterly event about the new data and search services and their relationship to the website and the web in general. Edward (who is our new user engagement person) helped out by driving the tabs. He did great. Dan did ok. Fewer laughs in the afternoon, though the 'dangirus doggs' search is a really good illustration of one way in which new search beats every other Parliamentary search out there.

### Parliament in the area, we're international, we're continental. But we're north of Glasgow

[Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver) and [Michael](https://twitter.com/fantasticlife) travelled to Stockholm for the [Euro IA conference](http://www.euroia.org/). Anya and Silver gave a talk on [Domain Driven Design at Parliament](https://www.slideshare.net/UKParliData/domain-modelling-parliament). Michael attempted to answer some questions. It seemed to go well though they were glad when it was over. Beer made nerves unfrondle.

### One world, one web, one team

Dan managed to make 3 website [stand ups](https://www.youtube.com/watch?v=cedNya7e8Uc) this week.

### Domain modelling

Anya, Silver and Michael continued work on modelling government departments, positions and incumbencies. The [model is now published](https://ukparliament.github.io/ontologies/government-department/government-department-ontology.html). Feedback is, as ever, welcome.

Michael met with [Chris](https://twitter.com/chrisalcockdev) to pass on work so far around the government model. He also met with [Colin](https://twitter.com/colinpattinson) to run through much the same stuff.

### Data quality

[Samu](https://twitter.com/langsamu) designed and [Jianhan](https://twitter.com/jianhanzhu) implemented a space on our internal network where people can easily make changes to data before it moves into the data service. This is accessible both to non-techical users through a somewhat friendly browser interface and to technical users doing batch operations. We're already making use of this new facility to make data quality improvements to data about Members' website links, photos, and committees. This interface will also be used for the "Lords Inflation" work. Don't ask, really don't ask.

Work continues on adding website and social media links to members. Again using the new interface. The data is now ready, so we're expecting much collaborative work between the teams over the next two weeks. Thanks to Callum for help with importing the data, Jianhan for setting up interim storage and editing facilities, Chris for creating mock data in our API so website development can proceed without waiting for data, and Wojciech for writing import code at record speed.
 
[Aidan](https://twitter.com/aidan_morgan) is chasing the Ordnance Survey about constituencies going missing from regions, postcode grey zones, and Northern Ireland postcodes and constituencies.

### Data platform

Wojciech (working with [Matt Rayner](https://twitter.com/mattrayner) and Sarah Allett from the website team) released a new version of the data platform infrastructure. A casual visitor to [beta.parliament.uk](https://beta.parliament.uk) would not notice that anything's changed, which means we've done a good job. Behind the scenes, however, this release:

* Brings our data up to date with most recent changes to the domain model.

* Saves us money by using the cheapest cloud computing resources available.

* Introduces architectural improvements that makes our live easier for importing data.

* Makes it easier and faster for us to switch between versions of applications.

* Reduces our dependency on the website release schedule.

Samu spent time with Sean Brazier to conduct a Service Assessment for the Integrated Workspace Management System (IWMS) project. This was the first session of a new format aiming to improve technology governance.

A quote from one of the project documents made him stop for a second:

"The current parliamentary estate measures approx. 222,000 square metres and consists of 34 buildings, properties and an underground car park. There is a total of 227 floors and 9651 rooms, when consolidated, across all of the buildings."

### Search

Michael and Robert wrote something about what we've done with the new search and why and assorted advantages and disadvantages. Anya added grammar. Silver removed a bit that was unintentionally rude to librarians.

The search team have been looking at how we better label search results according to document type. From what was a vague idea we now have a working prototype. The work will be considered for production soon.

To enable this [Raphael](https://twitter.com/raphaelleung) picked Ed McCarthy's brain to understand rules and exceptions around URL structures of publications which varies for current and archived materials.

Robert helped [Dia](https://twitter.com/DN78) with preparing a presentation for the Digital Strategy Board.

The team met with Fred to talk about library Research Briefings, particularly with regard to search. They came to the conclusion that it will take some time before we see most of what he described, but the broad aims were in line with those of the data service.

Robert is also catching up with Archives and Library folks on plans for search in the medium term.

Dia is also working on a feature list for search based on the feedback so far.

[Tony](https://twitter.com/psychemedia) wrote an excellent post on [options for search result display](https://blog.ouseful.info/2017/09/29/contextualised-search-result-displays/).

### Machines that do learning

Raphael went along to the [GDS](https://gds.blog.gov.uk/) data accelerator course and learned about how hyperparameter tuning can help with the toolkit for the Indexing and Data Management Section. He also with Angela on her application to join the next cohort.

### Measuring things

Liz met with [Steve](https://twitter.com/steve_bromley) and Trine to discuss collaboration around research and analysis. She also met with Nik on measurement and analysis for product teams. These were effectively the same, positive, conversations on embedding good practice and principles.

Liz requested a session with the search product team to plan A/B testing for resurrecting the display of URLs in search results. This went well. We now have defined measures and decision criteria for assessment of whether they are a bad thing. Or not.

### Corporate data

[Matias](https://twitter.com/matiasgermanico) met with Charlotte (head of the Enterprise Portfolio Management Office) to review the dashboard / report work he's been doing with Sam. The main concerns were how to be sure the sources could be trusted, how we could reduce text displayed and how to display trends especially regarding dates. Matias suggested they provide 3 KPIs as examples so we can try to produce them with the current data set.

### Documents from data

Tony and Michael met with Gordon Clarke and Louanne Middleton from committee land to talk them through some of the work Tony's been doing around [reproducible research](https://simplystatistics.org/2014/06/06/the-real-reason-reproducible-research-is-important/) using [Jupyter Notebooks](http://jupyter.org/). This seemed to match at least some of their thinking. Tony is planning to build a demo of a committee report and a library briefing in this fashion.

### Did anybody say blockchain?

To the best of my knowledge nobody said blockchain \o/

### Did Samu recommend any music?

Samu recommended the [Prophets of Rage](http://prophetsofrage.com/). Michael looked [a bit baffled](https://twitter.com/fantasticlife/status/914199895568994307).

### Strolls

Anya, Silver and Michael took a number of strolls through Stockholm. This was nice.

### Things that caught our eye

* [Can Well-Being Define What Government Does?](http://datasmart.ash.harvard.edu/news/article/can-well-being-define-what-government-does-1123)

* [Visualizing the Evolution of Ontologies: A Dynamic Graph Perspective](http://ceur-ws.org/Vol-1456/paper7.pdf) [PDF]

* [A Brief Overview of Outlier Detection Techniques](https://medium.com/towards-data-science/a-brief-overview-of-outlier-detection-techniques-1e0b2c19e561)

* [Attacking Machine Learning with Adversarial Examples](https://blog.openai.com/adversarial-example-research/)

* [Computing Machinery and Intelligence](https://en.wikipedia.org/wiki/Computing_Machinery_and_Intelligence)

* [What's the world's largest database?](https://www.quora.com/What-is-the-worlds-largest-database)