## 2018 Week 41

### Community

Over in Tothill Street, librarians Liz and Jayne continued to peer at card indexes, question the handwriting of professors and diligently add data to the new Rush application. Up in Sheffield (and on his journeys across Europe) James ploughed on with development and bug squishing. Introductions to Andrew paid dividends when he sent through a Wikidata extract containing matched IDs across the Rush data, Wikidata and Parliament's own Members' Names Information Service. The application will allow users to triangulate identifiers and combine data from multiple sources. Because we are nothing if not native to a web of data.

### The delivery is the strategy

Dan's spent another week mired in strategy. He's been working with someone called Olivia who, we're told, 'leads' on Information Management. I have no idea what that means. Apparently they're still trying to dock the data strategy with the information strategy but the pod doors won't quite close. Even Dan admits this seems quite odd but he suggests that it makes a lot of sense when you work through it and apparently there'll be lots of opportunities and things.

The data strategy open session experienced limited attendance this week with just Alison, Paul and Steve(?). Some bloke called FutureGov was occupying the room so our strategisers were forced to sit in the corridor. They spent the time talking about the problems with the pod doors. Alison, Dan and Paul met with someone called Helen Thomas in an effort to prepare for a meeting of something called the IMF. Which we're told is neither the International Monetary Fund nor the Impossible Mission Force. But is in fact a thing called the Information Management Forum. Which apparently is 60 people (60!) from around Parliament who have proved some interest in Information Management. It seems Alison, Paul and Matthieu are going to pitch the data strategy to this group at their next meeting in a couple of weeks. Best of luck here.

### The team meeting

So we had a team meeting. It was one of many meetings in Dan's week which left him with very little time to do any actual work. Which usually involves meetings so it's all circular.

Robert ventured the opinion that it was 'less bad' than the last one, and that the last one was less bad than the first one. Dan is interpreting this as progress. Michael is fairly sure Robert was mainly gossiping on Slack.

### Showing and telling

Liz and Alison took over on show and tell duties. They talked about what domain modelling: what it is and why it's useful. Then talked about the work they've done to capture a model for KPIs and some of the benefits they hope to get from this. Alison and Michael had a conversation about making a Turtle file for the measurement model and adding it to our list of published models. Which we really should do at some point.

### One world, one web, one team

Liz took the measurement domain model she's been working on with Alison for its first public outing. She met Jenny from the Office 364 programme and Tom from the world of Skype for Business together with a few of their colleagues. They used the model to talk through how they're going to identify measures and KPIs. Consensus seemed to be having the model helped with the conversation.

### Domain modelling

Anya, Michael and Robert continued their assault on the foothills of model comments. It's slow progress and there's no peak yet in sight, but it's not unrewarding. Elsewhere, Robert has been hacking away at his Turtle to HTML parser thing. Which looks better by the day. We look forward to publishing prettier pages in the not too distant future.

Late Wednesday brought the joyous prospect of yet another statutory instrument flowchart meeting. Anya, Robert and Michael once more met with Journal Office Jack, this time looking at what happens and what definitely doesn't happen when a draft negative is withdrawn. Luckily they came to the conclusion that this required less in the way of precludes arrows than the absoute shit show that is the draft affirmative. Flowcharts were updated. Data to follow shortly.

Thursday saw a full day meeting with Anya, Robert, Silver and Michael. They spent the morning looking at the work done last year around events in the context of committees. And decided it was terrible. So the event model is now in the bin. They took to whiteboards and started work on what they're calling a business item model. Which so far is just a picture. With some odd words. But it's still better than the event model. Work continues.

In the afternoon they were joined by Nicky and Chris from the [Parliamentary Archives](https://www.parliament.uk/business/publications/parliamentary-archives/). Some domain modelling happened around current archive processes. At a push you might even call it event storming. We say that now because Silver has been on a course. After filling several sheets of paper with data flow type stuff, they moved on to areas of common concern. The archives face many of the same problems we face in web land. Parliament doesn't make things at a granular enough level so people can't find anything. You can fairly easily make documents out of data; you can't easily make data out of documents. Somewhere between the modelling and the data platform there's a conveyor belt of documents getting generated that don't lend themselves to information discovery and don't lend themselves to archival discovery. More collaboration is needed here.

### On search. And indeed indexing

Alex wrote yet another automation script to fetch current tabled oral parliamentary questions and process the missing records in the search and indexing triplestore. This is usually done automatically by something called the harvestor service which, at least in theory, calls assorted endpoints around Parliament and grabs new data for processing into parliamentary search. But this time the harvest failed. Alex thinks he may have typed up a workaround to this issue (weeknotes passim) but that script was browser based and required a human to click things. He thinks the new script is much better and hopes it will become a long-term internal service.

New joiner Jamie R has been looking at log analytics to detect and visualise significant changes in how often users click on one of the top three search results. He's planning to incorporate some graphs into a dashboard. Your correspondent is not entirely sure why.

### Corporate data

Jamie R has also been thinking of ways to analyse data from the hardware asset system to provide the Windows 10 roll-out team with some information about hardware life cycles. Apparently so the team can plan their resources efficiently. No news on when rattling Dell keyboards get phased out. Never, one assumes.

David has been busy identifying and resolving issues with the MembersPost Address data transfer and updating the documentation to match. I'm not sure what this is. Maybe it's mailboxes. Or pigeons. Trained seals coming up the Thames.

Lew has continued development and testing the pudding and custard system integration. He's also had a few chats about how best to document our existing pudding system integrations, how puddings will be provisioned under our BizTalk upgrade path and making a new integration for our Toby Jug sales.

Noel has been soldiering on cleaning up after people. Especially the ones with an 'unknown' organisation or no job information. Which you feel could be quite a few people. Especially if someone updates 'strategy' to null.

### Paul's truly terrible week (slight return)

Paul has also been attempting to tackle the pod door problem. We have a number of strategies in a low earth orbit. But unfortunately not the same orbit. Paul gets to play James A. Lovell Jr. here.

This week he's been mainly drafting a roadmap of the work needed to support the data strategy and talking to some people called portfolio management (which is like bigger than a programme and like way bigger than a project). He's been trying to find ways of getting data considered earlier in the project approval process. Which given the projects are all about computers you'd think was a given.

### Customer service of the week award...

Nothing. Seriously.

### Did anybody have a pass office encounter?

Liz and David had a discussion about some of the issues we see with data coming from the Pass Office and the need to review some of the logic we use for data integration.

David and Matt continued the conversation and chatted about the process through which Roles are assigned to people. The current process uses the type of access level granted to people by the pass office, which used to be specific for each area of Parliament. It meant that staff of the House of Commons received a different access code to Members of the House of Commons who received a different access code to staff of the Parliamentary Computational Section etc. Since this was first implemented, the way in which access codes are assigned has changed which means they're no longer a useful indicator of role types. David and Matt are now looking at whether department and sub-department fields are a better source for determining what part of Parliament a person is supposed to be in. But there are 527 unique pairings, so it might take a decent chunk of time to churn through.

Michael also had an encounter with the Pass Office when he left his pass at home and had to debase himself by begging for a day pass. He remains convinced that nobody told him day passes had to be returned before real passes could be reactivated, so when he turned up the next day he couldn't get in anywhere. Because his day pass was in the bin. He returned to the Pass Office but found no source of charity. 7am the next morning saw him face down in rubbish, attempting to scrape garlic and tomato off a plastic envelope and a bit of card. He'd like to thank Robert for his help in securing visitor passes.

### Strolls

Following several months of domain modelling in Tothill Street, Anya, Silver and Michael have pretty comprehensively destroyed several roomfuls of whiteboards. It's getting to the point where nothing can get drawn on any of them. So Silver took them off on a stroll to the Soho Stationery Shop where he'd heard tales of a five star whiteboard cleaner that could cut through any amount of mess. Unfortunately Anya and Michael had both copped dodgy pints the night before so what started as a pleasant walk across the park ended as a death march to Fitzrovia. Because obviously that's where the Soho Stationery Shop is. They returned weeping slightly and coughing up blood. The tale would be redeemed if they could now boast of sparkling clean whiteboards but the five star whiteboard cleaner did not live up to its promise and the walls are still smeared with the contents of clerks' brains. Marvellous.

Dan and Ben took off together for a reinvigorating stroll. They spoke about the data strategy which you assume must have killed the mood. Dan says Ben was a big encouragement and seems to think Ben was suggesting he should be more practical. Or possibly more forthright. Or indeed bolder. Though other badges are available. There's a note to say the whole modelling thing / understanding what our data is is a seriously big deal. Oh, now they get it.

Dan also had the usual walk and coffee with Robert. Robert has a new rucksack. Strangely, Silver also has a new rucksack. Being Silver, and being all about the information retrieval, he's researched this at length and now talks about an expandable day carry. Or something. Which makes a change from pigs.

### Did anybody get a new job?

Dan kind of got a new job but it did not come with a title or, one suspects, any extra money. So more like slavery really. Anyway. He's joined what's known as the Service Design Team which is a group of eight people from around the department who think they're going to help change the way we work. They've given themselves six weeks to try to improve the way we order and provision computers. Let's see how that goes.

### Did Michael learn anything?

Chickens only have one bottom. A middle bottom. Who knew? Amaze.

### Things that caught our eye

* Chris sent Dan a post on [why ‘moving fast and breaking things’ must not extend to ethics](https://theodi.org/article/agile-ethics-pioneer-alix-dunn-on-how-to-minimise-harm-and-why-moving-fast-and-breaking-things-must-not-extend-to-ethics/). He also sent him a post about [working ethically at speed](https://medium.com/@alixtrot/working-ethically-at-speed-4534358e7eed). Dan would like it to be known he read them both.

* Dan also read [towards end-to-end local services, not transactions](https://medium.com/@mcaino/towards-end-to-end-local-services-not-transactions-a607b5d55ba9).

* Samu stumbled across an article on [why 'collaboration' creates mediocrity, not excellence](https://www.inc.com/geoffrey-james/collaboration-creates-mediocrity-not-excellence-according-to-science.html). He picks out a quote or two: "[...] rather than seeing a top performer as a role models, mediocre employees tend to see them as threats, either to their own position in the company or to their own feelings of self-worth" and "Rather than improving their own performance, mediocre employees socially isolate top performers, spread nasty rumors about them, and either sabotage, or attempt to steal credit for, the top performers' work." He adds no further comment at this point, your honour.