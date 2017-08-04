## Week 2: 04-08-2017


### Search

The weekly stand-up happened on Thursday. There was a good discussion mainly around feedback and analytics for the new service.

[Dia](https://twitter.com/DN78) took Robert through the plans for next week's search workshop and the current backlog.

Dia met Franny to discuss user research progress so far. She also met with [Dan](https://twitter.com/dasbarrett) and Robert to plan internal communications around changes to search.

There was also a meeting with [Matt](https://twitter.com/mattstutely) to talk through the plan for search going live and understand the dependencies.


### Data models

[Ben](https://twitter.com/benwoodhams) continued to work on documenting data integrity issues with particular focus on the Registers of Members' Interests. Conversations around registered interests, data models, and identifiers continued between Ben and [Michael](https://twitter.com/fantasticlife) over ping-pong, Slack, and cigarettes.

Michael had a play with visualising co-occurrence of Lords members' interests. [Interests co-occurrent by members is here](https://github.com/ukparliament/weeknotes.data-search/blob/master/assets/interests.pdf). Vice versa [here](https://github.com/ukparliament/weeknotes.data-search/blob/master/assets/members.pdf).

[Raphael](https://twitter.com/raphaelleung), Angela, [Jianhan](https://twitter.com/jianhanzhu), and Matthieu continued exploratory work on the landscape of committees data. They restored database backups and tried to figure out details of the models. This was presented alongside [Anya](https://twitter.com/bitten_), Ben, [Silver](https://twitter.com/silveroliver), and Michael's work on [domain models](https://github.com/ukparliament/domain-models) and [ontologies](https://ukparliament.github.io/ontologies/) at the Tuesday show and tell.

They also met with Sadia and realised that that much of the committee information on the current website is only present in the CMS and not available as structured data. And realised that the database behind committee tracker provides mappings between identifiers in a variety of systems and should be a useful data source in future investigations. 

Matthieu, Michael, Jianhan, Raphael & [Chris](https://twitter.com/chrisalcockdev) met to discuss progress on the committee domain model and associated ontologies.

Matthieu and Angela met with Ed McCarthy from Committees Services in the House of Lords to look into the editorial details of the CMS and the Members' Names Information Service.



### Capability

Wednesday was data day - our fortnightly planning and gossip session. It felt like we got somewhere with setting out medium term development priorities. Several members of the web team joined us and we talked through some of their immediate priorities around select committee membership data and finding constituencies by region.

We also covered off the first iteration of e-petitions tagging with Anya. Raphael set up a meeting with IDMS colleague [Liz](https://twitter.com/greensideknits) to keep them updated.

Robert attended a capability stand-up led by [Julie](https://twitter.com/julietouring) where actual standing up happened. They worked on refining job family descriptions into something a little more like how we expect them to exist in the future.

Ben went along to a cloud migration meeting and stayed long enough to establish his presence was not required.

Dia and Ben went back through the "Data 101" presentation - our attempt to explain our work to internal stakeholders.

Matthieu continued investigations into cloud service billing.



### Community

At data day we worked on our plan for events and visits in which we will most certainly [leave the capitol](https://www.youtube.com/watch?v=GpMoRS_9bcM).

Robert and Ben recorded a podcast episode with [Rob Greig](https://twitter.com/Rob_Greig) which seemed to go pretty well and ended up with more audio than expected.

Dan went along to a data visualisation workshop run by [Jamie](https://twitter.com/oddtype) with assorted people from the House of Commons Library and select committee land. It was a really good session and felt like there's plenty of opportunity for collaboration and community building here. Michael sulked because he did not know this was happening.

Raphael met with Luke from the Universal Credit team in the Department of Work and Pensions to look at their [RShiny](https://shiny.rstudio.com/) apps and extract / load / transform process. A return favour was offered.

He spent Thursday at GDS as part of the data science accelerator programme where he completed the work around comparing two ways of vectorising text features into numeric features. 

In other RShiny news, Liz organised a meeting with Andrew from the Ministry of Justice, who told us about their work on [latent semantic analysis](https://en.wikipedia.org/wiki/Latent_semantic_analysis) of Parliamentary questions. Which made Ben want to throw registered interests into vector spaces. [Source code here](https://github.com/moj-analytical-services/pq-tool).



### Analytics

Liz and Robert met to chat about search related user research and analytics issues and what we might do to improve things.

Sara started to look at analytics data from the current open data service, focusing on pageviews and common user paths.

She also had a chat with Liz and Wojciech about log data from members' pages on the [beta website](https://beta.parliament.uk), looking at how many users have downloaded MP's photos and if we could potentially use the log data for that.

### Corporate data

Lew continued work on the Non-Cleared People / Github integration and the spreadsheet to XML pipeline.

Noel has been working closely with the Learning and Development team to understand why some data issues happen and help them mitigate them.

[Matias](https://twitter.com/matiasgermanico) has finished the Enterprise Portfolio Management Office database model.

All the team have been working on installing BizTalk on their machines to test on them until the new environment is in place.

### Links

Dan published [a post on his recent working trip to North America](https://pds.blog.parliament.uk/2017/08/04/dude-wheres-my-data-pds-north-america/).

Robert spotted [a podcast episode from the Economist on state control of artificial intelligence in China](https://overcast.fm/+GfebProCA).


