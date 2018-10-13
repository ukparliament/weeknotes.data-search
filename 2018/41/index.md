## 2018 Week 41

### Community

Over in Tothill Street, librarians [Liz](https://twitter.com/greensideknits) and Jayne continued to peer at card indexes, question the handwriting of professors and diligently add data to the new Rush application. Up in Sheffield, and as he journeyed across Europe, [James](https://twitter.com/jamesjefferies) ploughed on with development and bug squishing. Introductions to [Andrew](https://twitter.com/generalising) paid dividends when he sent through a [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) extract containing matched IDs across the Rush data, Wikidata and Parliament's own [Members' Names Information Service](http://data.parliament.uk/membersdataplatform/). The Rush application will allow users to triangulate identifiers and combine data from multiple sources. Because we are nothing if not [native to a web of data](http://www.plasticbag.org/files/native/native_to_a_web_of_data.pdf).

### The delivery is the strategy

[Dan](https://twitter.com/dasbarrett) spent another week mired in strategy. He’s been working with someone called Olivia who, we’re told, ‘leads’ on information management. I have no idea what that means. Apparently they’re still trying to dock the data strategy with the information strategy but the pod doors won’t quite close.

A small yet select turnout at the data strategy open session this week, with [Alison](https://twitter.com/oliala), [Paul](https://twitter.com/paulwakely) and Steve(?) joining Dan. Some bloke called [Future Gov](https://www.wearefuturegov.com/) was occupying the room so our strategisers were forced to sit in the corridor. They spent the time talking about the problems with the pod doors. Alison, Dan and Paul met Helen Thomas in an effort to prepare for a meeting of something called the IMF, but not that one. It is in fact a thing going by the name of the Information Management Forum. This, apparently, is 60 people (60!) from around Parliament (60!) who have been determined to have some interest in information management. It seems Alison, Paul and [Matthieu](https://twitter.com/cognithive) are going to pitch the data strategy to this group at their next meeting in a couple of weeks. Best of luck here.

### The team meeting

So we had a team meeting. It was one of many meetings in Dan’s week, leaving him with very little time to do any actual work. Which usually involves meetings. Swings and roundabouts.

Robert ventured the opinion that the team meeting was ‘less bad’ than the last team meeting, and that the last team meeting was ‘less bad’ than the first team meeting. Dan is interpreting this as progress. [Michael](https://twitter.com/fantasticlife) senses a smoke screen. He's fairly sure Robert was mainly writing Python and gossiping on Slack.

### Showing and telling

Our Liz and Alison took on show and tell duties. They talked about [domain modelling](https://en.wikipedia.org/wiki/Domain_model): what it is and why it's useful. Then they talked about the work they’ve done to capture a model for KPIs and some of the benefits they hope to get from this. Alison and Michael had a conversation about making a Turtle file for the measurement model and adding it to our list of published models. Which is a possible thing that could happen.

### One world, one web, one team

Liz took the measurement domain model on its first public outing. She met Jenny from the Office 364 programme and Tom from the world of Skype for Business together with a few of their colleagues. They used the model to talk through how they're going to identify measures and KPIs. Consensus seemed to be that having the model helped the conversation.

### Domain modelling

[Anya](https://twitter.com/bitten_), Robert and Michael continued skirmishing in the foothills of model comments. We're marching slowly towards the sunlit uplands; it’s not unrewarding. Elsewhere, Robert has been hacking away at his [Turtle](https://en.wikipedia.org/wiki/Turtle_(syntax)) to HTML parser thing. Which looks better by the day. We look forward to publishing prettier pages in the not too distant future.

Late Wednesday brought the joyous prospect of yet another statutory instrument flowchart meeting. Anya, Robert and Michael once more met with Journal Office [Jack](https://twitter.com/jackpdent), this time looking at what happens and what definitely doesn't happen when a [draft negative](https://ukparliament.github.io/ontologies/procedure/sis/draft-negative.pdf) is [withdrawn](https://ukparliament.github.io/ontologies/laying/laying-ontology.html#d4e76). Luckily they came to the conclusion that this required less in the way of precludes arrows than the absolute shit show that is the [draft affirmative](https://ukparliament.github.io/ontologies/procedure/sis/draft-affirmative.pdf). Flowcharts were updated. Data to follow shortly.

Thursday saw a day long meeting with Anya, Robert, [Silver](https://twitter.com/silveroliver) and Michael. They spent the morning looking at work done last year around events in the context of committees. And decided it was terrible. So the event model is now in the bin. They took to whiteboards and started work on what they're calling a business item model. Which so far is [just a picture](https://github.com/ukparliament/ontologies/blob/master/business-item/business-item.png). With some odd words. But it's still better than the event model. Work continues.

In the afternoon they were joined by [Nicky](https://twitter.com/nickyhilton1) and [Chris](https://twitter.com/C_Fryer) from the [Parliamentary Archives](https://www.parliament.uk/business/publications/parliamentary-archives/). Some domain modelling happened around current archive processes. At a push you might even call it [event storming](https://en.wikipedia.org/wiki/Event_storming). We say that now because Silver has been on a course. After filling several sheets of paper with data flow type stuff, they moved on to areas of common concern. The archives face many of the same problems we face in web land. 

Parliament tends not to make things at a granular level, and so unless you're coming at it from the prescribed angle, you won't find it. And let's face it, the prescribed angle is usually a massive document. It's fairly easy to make documents out of data; you can’t easily make data out of documents. Somewhere between the modelling, the data platform and the archive there’s a conveyor belt of documents that don’t lend themselves to information discovery and don’t lend themselves to archival discovery.

### On search. And indeed indexing

[Alex](https://twitter.com/alexedwardh) wrote yet another automation script to fetch tabled oral [parliamentary questions](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) (OPQs) for the search and indexing triplestore. This is usually done by something called the harvester service which calls assorted endpoints around Parliament and grabs new data. But there are long running issues with the OPQ data source so occasionally the [harvest fails](https://www.youtube.com/watch?v=snnT5hgegi0&t=0m21s) and the feed is short on questions. Alex thinks he may have already typed up a workaround to this issue (weeknotes passim) but that script was browser based and required a human to click things. He thinks the new script is much better and hopes it will become a long-term internal service.

New joiner Jamie R has been looking at log analytics to detect and visualise significant changes in how often users click on one of the top three search results. He's planning to incorporate some graphs into a dashboard.

### Corporate data

Jamie R has also been thinking of ways to analyse data from the hardware asset system to provide the Windows 10 roll-out team with some information about hardware life cycles. Apparently so the team can plan their resources efficiently. No news on when rattling Dell keyboards get phased out. Never, one assumes.

David has been busy identifying and resolving issues with the MembersPost Address data transfer and updating the documentation to match. I'm not sure what this is. Maybe it's mailboxes. Or pigeons. Trained seals coming up the Thames.

Lew has continued developing and testing the sponge and custard system integration. He’s had a few chats about how best to document our existing pudding systems integrations and how puddings will be provisioned under our BizTalk upgrade path, and he's been making a new integration for our [Toby Jug sales](https://www.shop.parliament.uk/).

Noel has been soldiering on cleaning up after people. Especially the ones with an 'unknown' organisation or no job information. Which you feel could be quite a few people. Especially if someone were to update ‘strategy’ to null.

### Paul's truly terrible week (slight return)

Paul has also been attempting to tackle the pod door problem. We have a number of strategies in a low earth orbit. But unfortunately not the same orbit. Paul gets to play [James A. Lovell Jr.](https://en.wikipedia.org/wiki/Jim_Lovell) here.

This week he’s mostly been drafting a road-map of the work needed to support the data strategy and talking to some people called portfolio management - which is, like, bigger than a programme and, like, totally bigger than a project. He’s been trying to find ways of getting data considered earlier in the project approval process. Which, given the projects are all about computers, you’d think was a given.

### Customer service of the week award...

Nothing. Seriously.

### Did anybody have a pass office encounter?

Liz and David had a discussion about some issues with data coming from the Pass Office and the need to review some of the logic we use for data integration.

David and Matt picked up the conversation, chatting about the process of assigning roles to people. Currently, roles rely on the access code granted by the Pass Office. These used to be specific for each area of Parliament: staff of the House of Commons received a different access code to Members of the House of Commons, who received a different access code to staff of the [Parliamentary Computational Section](https://pds.blog.parliament.uk/) etc. A subsequent change in the way access codes are assigned means they’re no longer a useful indicator of roles. David and Matt are looking at whether the department and sub-department fields offer a better way of deriving what part of Parliament a person is supposed to be in. But, as there are 527 unique pairings, it might take a decent chunk of time to churn through.

Michael also had an encounter with the Pass Office when he left his pass at home and had to debase himself by begging for a day pass. He had a second encounter with the Pass Office when he turned up the next day and couldn’t get in anywhere. Because his day pass was in his kitchen bin. He remains convinced that nobody told him day passes had to be returned before real passes could be reactivated. He returned to the Pass Office but found neither succour nor comfort. 7am the next morning saw him face down in rubbish, attempting to scrape garlic and tomato off a plastic envelope and a bit of card.
### Strolls

Following several months of domain modelling in Tothill Street, Anya, Silver and Michael have pretty comprehensively obliterated roomfuls of whiteboards. It's getting to the point where nothing can get drawn on any of them. So Silver took them off on a stroll to the [Soho Stationery Store](http://www.sohostores.co.uk/) where he'd heard tales of a five star whiteboard cleaner that could cut through any amount of mess. Unfortunately Anya and Michael had both copped dodgy pints the night before, so what started as a pleasant walk across the park ended as a death march to Fitzrovia. Because obviously that's where the Soho Stationery Store is. They returned weeping slightly and coughing up blood. The tale would be redeemed if they could now boast of sparkling clean whiteboards but the five star whiteboard cleaner did not live up to its promise and the walls are still smeared with the contents of clerks' brains. Marvellous.

Dan and [Ben](https://twitter.com/benwoodhams) took off together for a reinvigorating stroll. They spoke about the data strategy, which you might reasonably assume to be a mood killer. Dan says Ben was a big encouragement, and seems to think Ben was suggesting he should be more practical. Or possibly more forthright. Or indeed bolder. [Other badges are available](/weeknotes.data-search/2018/39/#are-your-services-available-as-a-digital-transformation-consultancy). There’s a note here, adding that the whole modelling thing and the understanding what our data is thing is a seriously big deal. Oh, now they get it.

Dan also had the usual walk and coffee with Robert. Robert has a new rucksack. Strangely, Silver also has a new rucksack. Being Silver, and being all about the information retrieval, he's researched this at length and now talks about an expandable day carry. Or something. Which makes a change from pigs.

### Did anybody get a new job?

Dan kind of got a new job but it did not come with a title or, one suspects, any extra money. So more like slavery really. Anyway. He's joined what's known as the Service Design Team which is a group of eight people from around the department who think they're going to help change the way we work. They've given themselves six weeks to try to improve the way we order and provision computers. Let's see how that goes.

### Did Michael learn anything?

Chickens only have one bottom. A middle bottom. Who knew? Amaze.

### Things that caught our eye

* Chris sent Dan a post on [why ‘moving fast and breaking things’ must not extend to ethics](https://theodi.org/article/agile-ethics-pioneer-alix-dunn-on-how-to-minimise-harm-and-why-moving-fast-and-breaking-things-must-not-extend-to-ethics/). He also sent him a post about [working ethically at speed](https://medium.com/@alixtrot/working-ethically-at-speed-4534358e7eed). Dan would like it to be known he read them both.

* Dan also read [towards end-to-end local services, not transactions](https://medium.com/@mcaino/towards-end-to-end-local-services-not-transactions-a607b5d55ba9).

* Samu stumbled across an article on [why 'collaboration' creates mediocrity, not excellence](https://www.inc.com/geoffrey-james/collaboration-creates-mediocrity-not-excellence-according-to-science.html). He picks out a quote or two: "[...] rather than seeing a top performer as a role models, mediocre employees tend to see them as threats, either to their own position in the company or to their own feelings of self-worth" and "Rather than improving their own performance, mediocre employees socially isolate top performers, spread nasty rumors about them, and either sabotage, or attempt to steal credit for, the top performers' work." He adds no further comment at this point, your honour.