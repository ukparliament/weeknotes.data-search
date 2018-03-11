## 2018 Week 10

### Community

The team got a nice shout out in [Matt Jukes' talk on working in the open](https://twitter.com/jukesie/status/972078559455076352). As did these weeknotes. So somebody's reading them. Or pretending to.

Sara and Raphael went along to the [Department for Transport Lab meetup](https://www.eventbrite.co.uk/e/dft-lab-meetup-3-tips-for-building-an-artificial-intelligence-tickets-43662372331), to learn about how they 'taught a robot all about parliamentary questions'. Which appears to relate to this post on [human resources, robot responses](https://dftdigital.blog.gov.uk/2018/01/18/hr-chatbot-dft-lab/).

### One world, one web, one team

[Alex](https://twitter.com/alexedwardh) finally got a script working for merging shedloads of JSON files exported from [Solr](http://lucene.apache.org/solr/). Which should make it much easier for colleagues to analyse the data. He'd like to thank Wojciech for helping with this. Alex and Sara had lots of discussions about Solr and Sara discovered that the data being produced through Alex's script contained duplicates. So that's now been fixed.

Alex also did [Anya](https://twitter.com/bitten_) a couple of favours by extracting a list of the field names that have been used to link [Statutory Instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) to parliamentary business outputs, grabbing all the data for all Statutory Instruments in the last 4ish years and analysing the usage of the 'MemberPrinted' field. More thanks are due. This time to Sara.

Liz, [Ben](https://twitter.com/benwoodhams) and [Aidan](https://twitter.com/aidan_morgan) met to discuss the next steps for measuring where Digital Development activity has created 'civic value'. A decision was made to pursue qualitative as opposed to quantitative measures as the significance of the latter tends to fall away quickly upon detailed analysis and assessment. The next step is to chat to other organisations that have looked at measuring value and to think about ways of presenting qualitative measures in a useful way.

Liz, Anya and Alex went to a meeting on Statutory Instruments. Alex didn't understand any of it but, nevertheless, thought it was interesting. [Michael](https://twitter.com/fantasticlife) was there in body.

[Jianhan](https://twitter.com/jianhanzhu) supported the peers' portraits project by helping them clean the data and put the draft photos on the website for review. [Samu](https://twitter.com/langsamu) also helped to identify and fix some tricky problems with colour profiles.

Anya, Ben and Michael met with [Oli](https://twitter.com/olihawkins) from the House of Commons Library to chat through their modelling roadmap and explain a few of the difficulties they face. It's always nice to see Oli.

### Domain modelling

Anya, [Silver](https://twitter.com/silveroliver) and Michael spent a day looking at constituency stats for things like age profiles and benefits claimants. They came up with a [straw man model](https://ukparliament.github.io/ontologies/stats-series/stats-series-ontology.html) for adding this to the data platform. But it turned out the House of Commons Library are reconsidering how they get this data and what the shape should be. So that was a waste of time.

Anya, Silver, Ben and Michael had a meeting with Jack Dent (House of Commons), Jane White (House of Lords) and Claire Searle (from the Indexing and Data Management Section of the House of Commons Library) to translate the flowcharts they'd previously made for negative SIs in the [Commons](https://github.com/ukparliament/domain-models/blob/master/SIs/flow-commons.pdf) and [Lords](https://github.com/ukparliament/domain-models/blob/master/SIs/flow-lords.pdf) into something more amenable to [the proposed procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html). If you are confused about parliamentary procedure for handling negative SIs this [new flowchart](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/negative.pdf) might be of assistance. Obviously, it might not.

Silver has been spending time translating the new flowchart into a spreadsheet. A similar flowchart and spreadsheet for affirmative SIs will follow shortly.

Thursday was spent back in the realms of the procedure model. Anya, Silver and Michael met with Gordon Clarke. Who is, coincidentally, the clerk of the Transport Committee. They took the creation and population of a committee as another example of a procedural flow, and drew it out in a way that mapped to the proposed model. Tyres were kicked and no gaps were found. Which was reassuring.

In the afternoon, Ben and Samu came over and there was more chat about the procedure model in general and SI data in particular. It was good. In Samu we trust.

### Data platform

[Chris](https://twitter.com/chrisalcockdev) has been working on fixing a problem that has been troubling us for a while. In order to get data into the data platform we have to query business systems and process any changes. Unfortunately we don't have a feed of change events from these systems so we've had to grab all the data, compare it to what we exported previously and work out what's changed. For inserts and updates this has worked fine, but deletes from source systems have been tricker to identify. Without a separate feed to say, 'yes, this thing that used to exist has now been deleted', it's a little like arguing a negative.

So Chris has been working on a better way of comparing the current import to the previous import to give us a more reliable way to identify and check deletes. His code is, if not perfect, in a working state as of this week.

Chris would like to add, whilst the code is not yet completely stable, anyone can [get in touch](mailto:data@parliament.uk) and ask for near-live updates on any given table from the Members' Names Information Service. Michael suspects this might be of some interest to Wikipedia / [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) types...

Mike and Samu are almost ready to finish moving [Historic Hansard](http://hansard.millbanksystems.com/) from our current hosting provider to our new one. They've created the infrastructure and are currently waiting for the domain name to be re-pointed.

On a similar subject, [Mike gave an excellent show and tell on the migration of data.parliament.uk to our new cloud platform](https://twitter.com/dasbarrett/status/971009968966111233). Proving he's not just about excellent customer service.

Samu added content collections to the data service so articles can now be bundled up into things like parts, chapters and sections.

### Search

Just fix the browse. Search be fine.

### Corporate data

[Dan](https://twitter.com/dasbarrett) managed to get himself a shiny new job and is now responsible for "leading all aspects of our data strategy and its delivery". He'll be starting in the general area of fixing corporate data. Well done, Dan.

Dan did a fair bit this week on strategic corporate data stuff, starting to work more with [David](https://twitter.com/SmithDavidM), the Deputy Director of PDS. Highlights included helping the HR and finance system replacement programme by identifying roles and skills they're going to need.

Dan's also been interviewing for a new corporate data architect with Rupert from upstairs.

Lewis has continued work on the new stock and finance system integration, including some development, code refactoring and troubleshooting of one of our internal web services.
 
[Matt](https://twitter.com/matiasgermanico) has created another way of processing the data received from the House of Commons HR feed. Testing will be done and there's an expected deployment sometime next week.

Elsewhere, work has continued on the asset management system integration. Deployment to follow soon.

### Aidan's truly terrible week (slight return)

This week Aidan has been mainly:

* reviewing milestones and looking at ways to improve communication of the Data and Search roadmap

* streamlining reporting processes and developing proposals for automating the workflow for reporting

* finalising the budget requirements for 2018/19

* assorted procurement activities

* opening discussions around IP and planned development work

### Excellent customer service award

For anyone with a large enough gap in their lives to be following these posts, it will come as no surprise that Mike once again wins the customer service award. We had a variety of queries from public users about our search services. One in particular led to the discovery that a parliamentary question hadn't been indexed by external search engines (and therefore by our own new search) due to errors and delays in how it had been published by internal systems. It was a useful insight and something we'll need to bear in mind. It also supports our position that [you can't fix web search without fixing browse](http://smethur.st/posts/176135866). There was a team effort here and Mike was able to get the user what they needed by other means.

### Did anybody say [GDPR](https://en.m.wikipedia.org/wiki/General_Data_Protection_Regulation)?

Yes. Yes they did. Colleagues have been talking about it for a while, but this week GDPR became a topic of interest for the team and we're expecting we'll be working on it more and more.

Aidan attended a meeting on GDPR and now has some actions as a 'contract manager' to complete before 25th May when the legislation comes into force. He'll be talking to people across PDS to understand if changes to existing and upcoming contracts are required.

Liz noticed that [IP addresses](https://en.wikipedia.org/wiki/IP_address) have dropped out of the Microsoft telemetry data. From early February they [stopped the automatic logging of this information](https://blogs.msdn.microsoft.com/applicationinsights-status/2018/02/01/all-octets-of-ip-address-will-be-set-to-zero/), quoting GDPR. We had been using IP address ranges as an approximate way to identify internal and external users. Raphael has looked into it with Wojciech and thinks we can add some custom code to re-instate it. But maybe we don't want to do that, given it's a pretty rubbish method for the only current use we have for it. Also, yeah, GDPR.

It will be interesting to see if Google take the same route...

### Does Samu know about Photoshop

So it turns out he does. No end to the boy's talents. Seriously.

### Strolls

Once again we have very little here. Though in the course of a stroll through Brighton, Silver did get trapped on a ghost train. Which made the whole week worthwhile.

### Things that caught our eye

* [Linked Data, Ontologies, Controlled Vocabularies and their usage in the Italian Public Administration sector](https://github.com/italia/daf-ontologie-vocabolari-controllati/blob/master/Presentazioni/LinkedDataItaly.pdf)

* [Let's talk about strategy by Sophie Dennis](https://www.slideshare.net/sophiedennis/lets-talk-about-strategy-extended-workshop-what-it-is-why-it-matters-and-how-to-do-it-well-sophie-dennis-90089444)