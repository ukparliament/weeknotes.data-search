## Week 16: 10-11-2017

### [Leave the Capitol](https://www.youtube.com/watch?v=GpMoRS_9bcM)

A reminder that our [5th Parliament, data and democracy meetup](https://attending.io/events/parliament-data-and-democracy-meetup-5) is on Wednesday 6th December, this time at [ODI Leeds](http://leeds.theodi.org/).

More in the way of interesting talks, nice people and [free beer](https://en.wiktionary.org/wiki/free_as_in_beer). Come along. Bring a friend.

### Data Day

[Data day](https://twitter.com/dasbarrett/status/928304905697288192) was something of a curate's egg. [Dan](https://twitter.com/dasbarrett) thought it mostly good. Quite frankly Robert found it... challenging.

The new post data day 'Dan and the developers' session was good. They went through work to do, context, and future plans.

The 'work that Data and Search are doing for the website' bit was the smoothest yet. Also definitely more than 10% of the team's time. Some things were agreed:

* Dan and [Jamie](https://twitter.com/oddtype) need to have a conversation with [Emma](https://twitter.com/_allenemma) about uptime and support.

* Dan and Jamie need to have a chat about the technical approach to managing and publishing 'content'.
 
* We need to decide on how we model committee staff.

* A user need for the bulk download of Member photos has emerged. Data and Search have volunteered to do the work required.

* We'll continue to prioritise work on divisions and written and oral questions and answers for the Members' activity work.
 
### Community

Liz, Sara and Saffiyah went to the [ODI](https://theodi.org/) for some training on open data. Liz thought it was interesting, informative and well structured.

Apparently open data doesn't automatically mean free (in cost). Liz didn't know that. The [share-alike licence attribution](https://en.wikipedia.org/wiki/Share-alike) was interesting and also, linked to that, the 'pay to close' model.

### One world, one web, one team

In Ceremony Watch, Dan went to one stand-up this week. [Aidan](https://twitter.com/aidan_morgan) and [Michael](https://twitter.com/fantasticlife) went to more.

Dan and Aidan covered all of the Members website product team 'Members activity' 'discovery day'. Dan enjoyed it and thought the energy levels were good. Michael also attended.

There was a brief look at other Parliamentary websites. Dan thought it was funny how they all tended to blur into one and liked the attitude of trying to do something different and better. 

### Domain modelling

[Anya](https://twitter.com/bitten_) and Michael took a second shot at adding comments to the [Formal Body model](https://ukparliament.github.io/ontologies/formal-body/formal-body-ontology.html). This time it seemed to pass the Ed McCarthy test. It still needs to get checked by House of Commons people. And someone needs to decide if House of Commons General Committees are similar enough to House of Lords non-select committees to treat as the same thing. At least in the data model.

Anya and Michael also visited Sally Carter in the House of Lords Hansard office to see how they deal with written questions and answers.

Dan had a good talk with Matt Stutely (Head of Business Systems Applications) about the House of Commons [Register of Members' Financial Interests](https://www.parliament.uk/mps-lords-and-offices/standards-and-financial-interests/parliamentary-commissioner-for-standards/registers-of-interests/register-of-members-financial-interests/). Dan's feeling pretty positive about this. More to follow.

Ed wrote a 'data principles for business systems’ document in preparation for working on the new bicameral committee business system in the new year.

### Data platform

The stable identifier work is now done. So the little strings of text at the end of URLs will no longer change when the data platform gets rebuilt. [The web will thank us](https://www.w3.org/Provider/Style/URI).

Government positions are now live in the data platform and on [beta.parliament.uk](https://beta.parliament.uk). Pages for government departments and answering bodies should follow shortly but we need to import the data first.

Opposition positions will also be needed at some point in the not too distant future. Data day meeting notes suggest the data modelling work is done here. It isn't but should be shortly.

The first iteration of the ‘search hints’ capability will be available via the API shortly. The target is for the first changes to website search to be implemented by the end of November.

[Ben](https://twitter.com/benwoodhams) has continued to work on Lords' inflation (still don't ask) which is almost complete. The data will be imported into the data platform and made available to the beta website shortly.

### Search

This week Robert has been mainly having visions about search. [Dia](https://twitter.com/DN78) and Robert continued to work on defining the vision and goals. The team are trying to ensure that the 'vision' for search doesn’t stray too far from the Digital Strategy. It seem to be... going fine. 

Robert spoke with Joe from the content team about search description text and how to improve it. He thinks he may have learned how to 'measure success'.

Robert also found the usual post-it shuffling ceremonies a little more useful. Which is nice. He also spoke with Jamie on metadata for search spiders on the beta website and is currently working on a note for Jamie’s team on “writing for machines”. Notably this is a note, with very particular goals, not a technical document or backgrounder. It’ll go past Joe in Content and anyone else who’s interested before next week.

A/A testing, which the team wanted to perform before commencing the A/B testing for the display of URLs on search results, has begun. The test is designed to ensure that the analysis tool is communicating with the website.

Dia will be presenting at [Product People on Monday](https://www.eventbrite.co.uk/e/product-people-november-2017-meet-up-in-london-tickets-38719744799) which the product management team at PDS are hosting.

Anya got back with some observations on the performance of Parliamentary Search (a search service available to internal users only) since the migration to the cloud:

> I’ve noticed that it is quicker at retrieving search results, so much so that the first couple of times I used search this morning I hadn’t realised that the previous search results had been replaced with new ones.

> I’ve not had any timeouts since yesterday and using advanced search does seem to be quicker than previously. The one thing I have noticed as an improvement is narrowing down your search results using the filters, it used to be much slower but now applies the filters pretty much instantly.

> working fine – no error messages today

Anya says, "It's worth noting that before the migration there were error messages every day."

### Measuring things

Liz met with [Liz Marley](https://twitter.com/greensideknits) from the House of Commons Library to discuss search terms and vocabulary analysis. This is information they've been wanting to get their hands on for a while to feedback into their work on maintaining and developing the [vocabulary](http://www.data.parliament.uk/dataset/thesauri). Liz is interested in finding [differences between parliamentary language and search users language](https://en.wikipedia.org/wiki/Folksonomy#Folksonomy_vs._taxonomy). Assorted Lizes talked about the structure of the data that's available in Ontology Manager (which for the pedantry record is a taxonomy manager, goddam), how often it's updated and how we might approach the analysis by prioritising based on what people are looking for.

Sara got in contact with Matt Upson from GDS to talk about using [machine learning to categorise user feedback from surveys](https://dataingovernment.blog.gov.uk/2016/12/20/using-machine-learning-to-classify-user-comments-on-gov-uk/). A proper chat will be scheduled.

Liz has been playing with a new analytics package, writing a query to extract search term, click number and search result page number, and then looking at how to combine this with search term groupings. 

Wojciech wrote Liz a function to decode search terms. Liz says thank you Wojciech.

Wojciech also helped Saffiyah to automate an API call to collect data on surveys and help drill into the House of Commons Library enquiries database.

Liz met with Rosie from the House of Commons Library communications team. Rosie has been working on website analytics for [research briefings](https://researchbriefings.parliament.uk/), providing feedback to producers on how their briefings are viewed. They discussed plans to join together the research briefings database, web analytics and research tracking data and share the model created so library staff can more easily use the information. Rosie had questions on how to serve the different reporting needs of different people with one model, something Matt and Liz talked with Krzystztof about last week.

Ben and Michael had a meeting with [Edward Wood](https://twitter.com/edwardwood99) from the House of Commons Library to chat about analytics and privacy.

### Machines that do learning

The machines are still thick.

### Did anyone say blockchain

Samu said blockchain twice. He also said "smart contracts". But he was grinning at the time so we think we're safe.

Michael also said blockchain but he was *particularly* hung over.

### Strolls

Robert and Michael took another stroll around Westminster. Nothing was resolved to anybody's satisfaction.

### What's Samu reading?

Samu read the [Programmers' Handbook for Manchester Electronic Computer Mark II](http://www.alanturing.net/turing_archive/archive/m/m01/M01-001.html) by Alan Turing (though not all of it), which he found fascinating. It shows that iterative development was not invented recently: "At the time of writing, comparatively little programming has been done with the Mark II machine. It is hoped to issue supplements consisting of particular routines from time to time." Samu has the feeling it explains why we use the slash (/) so extensively in computing. Turing chose / to stand for the 00000 teleprinter code, which means "no effect". You can imagine lots of all-zero sequences in machine code. There's also a [transcript here](http://curation.cs.manchester.ac.uk/computer50/www.computer50.org/kgill/mark1/RobertTau/turing.html).

### Things that caught our eye

* [The cost centre trap](http://www.leanessays.com/2017/11/the-cost-center-trap.html)

* [How Cloudflare uses lava lamps to encrypt the Internet](http://www.zdnet.com/article/how-lava-lamps-are-used-to-encrypt-the-internet/)