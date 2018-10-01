## 2018 Week 39

### Community

Wojciech, Mike, [Chris](https://twitter.com/chrisalcockdev), [Samu](https://twitter.com/langsamu) and [Matthieu](https://twitter.com/cognithive) all went along to an [Ontotext](https://en.wikipedia.org/wiki/Ontotext) meeting to talk about our work. We're not told how this went but we assume they enjoyed it. They do tend to like talking about computers and stuff.

[Dan](https://twitter.com/dasbarrett) met with Joel from the Cabinet Office to talk about data modelling, how we got the new data service off the ground, and our long standing desire to see [registers](https://gds.blog.gov.uk/2015/09/01/registers-authoritative-lists-you-can-trust/) of Government things. Like ministers. But Dan's main thought was what a strong story we've got to tell from the past two and a half years. Like, really good. Proper mate.

In further jolly news, Dan also went to a meetup at the Treasury about all things data and strategy. He thought it was good on balance, but came away unsure about how well the consensus view of what should be in a data strategy fits with our work.

### The delivery is the strategy

The major event in Dan's previous week was a trip to the Information Authority where he put on his best face and pitched the data strategy. We're told the Information Authority are the internal board who are most relevant to the data strategy. So that's handy. Dan took up most of the session and answered lots of questions. He says the best bit was the support for the [work behind](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html) the [Statutory Instruments tracker](https://beta.parliament.uk/statutory-instruments) and a sense that people are starting to 'get it': why it's important and what it entails. He didn’t really get a clear set of actions, other than to work to ensure that the data strategy is ‘aligned’ with all the other strategies around the place. He’ll be returning to the Information Authority by the end of the year.

This week he's received more feedback from the Information Authority, including a recommendation that a 'project board' be convened for the data strategy. He's not yet sure what that's going to be like or who is going to be on it. But he hopes it will be helpful. We all hope this.

Dan's also started work on making sure the data strategy is aligned with assorted other strategy type things and has been meeting with a variety of folks who do information strategy and with Rosie and Vincent on the digital strategy. He's really not 100% sure how this is going to work, but he hopes we get to carry on with the central recommendations of the data strategy as they stand.

Dan put a bit of a shift in for the Interaction Management programme. Whatever that is. It reminded him that if all else goes to pot he's a passable project manager. He provides a handy definition of 'putting a shift in' here. Apparently it means going to meetings and suggesting to people what they might want to do and how they might want to do it.

In the enforced absence of Dan, [Alison](https://twitter.com/oliala) took over on data strategy open session duties. Though no video of her mumbling into a flask exists. Dominique from the [Clerk of the Parliaments](https://en.wikipedia.org/wiki/Clerk_of_the_Parliaments) office came along, which was really useful. Alison thinks we need to think about how to get more attendees from outside the Parliamentary Computational Section. We're told they discussed the strategic alignment of the strategy to wider strategies in Parliament. As opposed to the tactical alignment of tactics. We have strategies like Dante had circles.

### One world, one web, one team

Dan spent all of Tuesday fully immersed in the world of Service Design with something called the 'change team' and a special support appearance from [FutureGov](https://www.wearefuturegov.com/). He thought much of it was really good, and particularly enjoyed the keynote by [Bea Karol Burke](https://twitter.com/beatricelucy). He says there was loads in Bea's presentation about working in change at Citizen's Advice that was really relevant, particularly when services on a website aren't transactional. Our Liz and Alison got a shout out from a few people for the work they're doing on the modelling of measuring things.

Alison held another workshop type thing with data and performance analysts in an attempt to resolve a few outstanding differences in their measurement models. Liz and Alison worked together to tidy the model and add a few additional concepts. Work on definitions remains in progress.

Team data analysis have been busy discussing documentation: what they need to capture as a standard and which elements are appropriate for which audiences. Liz found [dataMaid](https://www.rdocumentation.org/packages/dataMaid/versions/1.1.2), an [R](https://en.wikipedia.org/wiki/R_(programming_language)) package that produces a document assessing various aspects of a dataset, like missing values, ranges etc. She thinks this could be part of the team's workflow. And given [it's customisable](https://cran.r-project.org/web/packages/dataMaid/vignettes/extending_dataMaid.html), they could add their own checks. New joiner, Jamie R has been leafing through some features provided by [R Markdown](https://rmarkdown.rstudio.com/) that can help analysts record the work they do in a way that is usable across different audiences without creating overly long documents.

### Domain modelling

[Anya](https://twitter.com/bitten_), [Silver](https://twitter.com/silveroliver), Robert and [Michael](https://twitter.com/fantasticlife) spent Tuesday tucked up in the relative sanity of Tothill Street. No strategies were discussed. No programmes were initiated. Instead they took a long overdue second look at the [formal body model](https://ukparliament.github.io/ontologies/formal-body/formal-body-ontology.html), removed some cruft and happily simplified things. They need to do much the same for the rest of the committee-ish models.

[Jamie](https://twitter.com/oddtype) called by and asked them to look at the data coming from the new Committee Information System API and checking where it meets the models. And where it doesn't. So that was the afternoon lost. Pictures got drawn. Notes were typed.

Otherwise, most of the effort went into more comment editing. They are getting better all the time. But they have to tell themselves this.

### Data platform

It's been a big week for team:Samu. Since the launch of [data.parliament](http://www.data.parliament.uk/) we've had a lot of requests to just make the data available to download. So Wojciech has [done that for the new data platform](https://api.parliament.uk/download). Which as yet doesn't have all the data in data.parliament but is better modelled and hopefully more comprehensible. The lastest dump is available at [api.parliament.uk/download/latest](https://api.parliament.uk/download/latest); older dumps at api.parliament.uk/download/{timestamp}.trig. As ever, the list endpoint responds in HTML, XML and JSON depending on your accept headers. The request rate is initially limited to (an intentionally conservative) 1 file per 10 seconds per IP address and 2TB per month in total. Go fill your boots.

Matthieu also [took strides](https://twitter.com/langsamu/status/1044662469334114306) to making our data more widely available. He's created a [docker image of our triple store and data graph](https://hub.docker.com/r/ukparliament/graphdb/) with initial permission from Ontotext to distribute for a month. Though if you go grab it now it will continue to work once the month is up. Matthieu and Samu worked together on the continuous integration part to make sure the data gets updated on a daily basis. Have [a tinker](https://twitter.com/cognithive/status/1044663163612991493). Have fun.

### On search. And indeed indexing

[Sara](https://twitter.com/sarafreis) has continued with her work to measure correlation between search terms entered by users and the [House of Commons Library controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri). This week she's been paying particular attention to the issue with false matches to acronyms. Using the current method, the non-preferred term 'DATA' (an acronym for 'Design and Technology Association') matched 872 search terms. But we're assuming people are actually searching for data and not DATA. Though we are biased here obviously.

Our team of trusty data analysts have been busy setting up queries to slice and dice the analytics around search behaviour. Which proved useful when Matt R noticed a large and unexpected change in the average position of the result users were clicking on. Peering at the data they found most clicks were being recorded as position 10. Your correspondent is not sure if this is good or bad. Liz also noticed an error in counting search hints. She had a chat with [Bex](https://twitter.com/rklappleyard) about how we might test more thoroughly before releasing custom events in the future. Allan's been looking at the errors and Peter is looking at setting up some standard checks. Liz says thanks to all of them. She also says the team are looking at how they can make the measures we have more visible, so people can see the info without having to run the all the queries.

### Corporate data

Bridget went along to two out of three demos by Oracle on something called [Enterprise Resource Planning](https://en.wikipedia.org/wiki/Enterprise_resource_planning) which had something to do with the art of the possible. Which is a welcome clarification. She also met with a PDPM business analyst to discuss something about the data model requirements of the PDMP Blueprint. Dear [reader](https://twitter.com/PhilDRoberts), I have no idea what a PDMP is or what its Blueprint might be. I'm assuming we're not going into the prescription drug market but you can never be sure. Answers on a postcard please.

Bridget has also been continuing work on the development of the data strategy approach and processes by breaking down the tasks to improve our approach to data migration. This is currently being tested in the ECM project (no idea) with an upgrade of three instances of Dynamics CRM 2011 to Dynamics 364. The team are in discussion with Liz about what data profiling support her team could provide. We're told the ECM project (still no idea) is also helping us think about what a wider implementation of Dynamics 364 might look like. Bridget is looking forward to discussions with the interim Solution Architect around options and impacts. And who wouldn't be? 

Bridget's week ended with a kick-off meeting for the Retail Management System replacement project to find out what they know about the data to date and identify gaps. Marvellous stuff.

### Paul's truly terrible week (slight return)

[Paul](https://twitter.com/paulwakely) experienced a small uptick in fortunes this week. He went along to the Service Design day, which he says seemed like a reasonable start to what looks like a great deal of work for the Parliamentary Computational Section. He also had a good session where [Aidan](https://twitter.com/aidan_morgan) explained lots more about what everyone is working on and presumably why. Unfortunately he then faced several conversations about [PowerBI](https://en.wikipedia.org/wiki/Power_BI). And was forced to spend the rest of the week reading, talking and writing about the data strategy and how it fits with various other strategy type things. Poor lad.

### Customer service of the week award...

...goes to [Alex](https://twitter.com/alexedwardh), who helped out Chris Watson from the House of Commons Library by doing a big bulk export of all Commons Member contributions since the start of the 2015 session. 270k records have been sent to Chris. Top work Alex.

### Did anybody say blockchain?

Somewhat worryingly Jamie reports that Samu did indeed say blockchain. At least once. More worryingly still, Samu does not deny this. He explains this away by telling us he was thinking about introducing cryptographic proof into our identifiers so people could validate them. Luckily Wojciech reminded him that we already have validation because they're HTTP URIs and therefore [dereferenceable](http://www.liquidquotes.com/mpasin/quotes/1241). Anyone can take an identifier and ask Parliament for some information about the thing it identifies. If an identifier wasn't issued by us, the response will just be nothing. Dereferencing is also backed by DNS and SSL certificates, so we think we're pretty safe. Close call that one.

Dan also reports hearing someone else say blockchain. But he doesn't reveal who.

### Fashion news

Dan tells us he bought one of those outdoors-y type coats like what Michael wears. But a shit ton cheaper. He's much influenced by Michael and Robert, is Dan.

### Are your services available as a digital transformation consultancy?

Well, it's funny you should ask that. Silver and Robert have been deep in conversation about providing digital transformation consultancy for all your civic tech needs. [parliament.digital](http://parliament.digital/) has already been registered. 'Evolution, not revolution' posters have been blu tacked to walls. 'Be timid' stickers are already rolling off the printers. If you're in the market for cookie cutter approaches to digital transformation and would like to outsource your thinking, do get in touch.

### Strolls

Again, a notable lack of strolls have been reported. Although Dan did take a couple of walks with Robert. Presumably in the direction of artisan coffee.

### Things that caught our eye

* Dan suggests that a lot of people might be reading [Tom Loosemore's Making government as a platform real](https://public.digital/2018/09/25/making-government-as-a-platform-real/). And he's probably right.

* Matt R found and enjoyed [Spotify's summary app](https://spotify.me/en). Snoopware but for cultural populists.

* Dan read [My favourite design tool](https://ethanmarcotte.com/wrote/a-design-tool/) which he says is short. And it is.

* Dan read [Terence Eden's study of the mobile phones of Doctor Who](https://shkspr.mobi/blog/tag/doctor-who-phones/) which is about phones on telly.

* Alex pointed out [Tim Berners-Lee's plan to upend the World Wide Web](https://www.fastcompany.com/90243936/exclusive-tim-berners-lee-tells-us-his-radical-new-plan-to-upend-the-world-wide-web). Too little, too late. Said Robert. And Silver. And Michael. Because they are old and cynical. And the web is too broken to fix now.