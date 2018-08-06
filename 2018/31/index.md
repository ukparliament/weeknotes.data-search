## 2018 Week 31

### Dator day 

Tuesday was [data day 42](https://twitter.com/dasbarrett/status/1024711433739804673). Or possibly Wednesday. It's hard to keep track. Dan, Jamie, Samu, Alison and Robert locked themselves away in a humid cupboard and talked about data. And work. What better way to spend the summer?

They chatted website progress, technology in general, cloud adoption in particular and what's happening with all the other (non-public) data. Later in the day they were joined by Alex who brought along some interesting questions. How do data teams justify their existence was a particular doozy. Answers on a postcard please.

Jamie would like it to be known he found Alex’s comments and questions inspiring. Particularly around how the Libraries act as an institutional memory for the state (and not just our own Members). Basically because information management in government departments might be best described as broke. Alex also endorsed our new 'purple' unified search. He commented on how the simple interface felt familiar. His views on the purple are not recorded.

We don't learn from Slack if all Alex's question were answered to everyone's satisfaction. We do learn they [ended up in the pub](https://twitter.com/dasbarrett/status/1024711616040972288). And what question has never been successfully answered in a pub?

### Is Samu morality?

On the subject of juicers, Anya, Samu and Michael also took a trip to the Red Lion. At some stage in the evening Samu announced to his eager crowd, I AM MORALITY. We're not sure how we got there. Anya and Michael took an extra sip and lit another fag. It's best not to question.

### Community

Dan went to Bristol. It was dreadful. Or at least the trains were. Railways and hot days don't combine well. In this country. As a result he missed two of his meetings but he did have a mind-expanding time at the [Office for Students](https://www.officeforstudents.org.uk/) learning about [Microsoft Dynamics 364](https://en.wikipedia.org/wiki/Dynamics_365) on behalf of the Interaction Management Programme.

Anya, Robert and Liz had a phone call with Thomas Francart from the European Legislation Identifier project. They're expanding their work from legislation to draft legislation and wanted to check how that fitted with our stuff. The connection was made via Dan from the schema.org conversations. Thanks Dan.

Our Liz chatted to Andy at the ONS about their processes for deciding on features and improvements. Andy said it's not lead by any specific routine although they do regularly gather feedback and talk to users. Their negative feedback is almost always from users on the site, and not from those arriving externally. ONS use Elastic Search so are more concerned with ranking content than we are. They also monitor their top 100 terms and group terms to try to understand how to solve problems based on what they see people do. For the ONS, search isn't a a separate consideration from pages and journeys. Which is as it should be, says Michael. They have similar questions on domain specific language and sometimes feel they make decisions that are best for the business and not for users. Liz says it would be good to speak with their analyst. Plans were made for further chats.

### One world, one web, one team

Michael met with Steve to chat about user research and Michael's half coherent thoughts on the ecosystem, information flows and ripples of parliamentary users. And how measuring and targeting individual user needs might not play well with this. Michael's been bending many ears on this recently, not least Anya, Robert and Paul. A blog post might be brewing.

Alison spent some time with our Liz and her dedicated team of data analysers to start sketching out their workflow. Liz thought they got quite far. Together they identified some further work around how they communicate results (or insights as we say these days) and some more general stuff around how they move from [Exploratory Data Analysis](https://www.itl.nist.gov/div898/handbook/eda/section1/eda11.htm) to a more established process.

Alison also ran a workshop with performance analysts and data analysts (don't look at me, I don't know). They talked in more detail about some of the terminology used to describe measurement and how the different terms might be related (measurement vs. metric vs. indicator vs. KPI). We are, as ever, divided by a common language. Sara says it was a good exercise and a good start at defining and unifying the language we use for measurement. We're also told a lot of post-its were involved but not whether this was a good or bad thing.

Samu met Oswin Taylor from the Legislation Office in the House of Lords. They had a second talk about supporting the drafting process for Private Members' Bills again, this time focusing on a the practicalities of document and workflow management. Samu reports it was a good talk. And if Samu approves we can be sure it was good.

### Did Mike discriminate?

A report came in from an internal user flagging up our internal search application doesn't work with a certain browser / operating system combination. This gave rise to allegations of discrimination against a certain fruit-based operating system. Luckily the machines do not yet have HR, so we're fairly sure Mike is safe. For now.

Scarred by allegations of systemic OS discrimination, Mike continued to investigate and found that the problem can be reproduced by connecting to the application over a certain network route. No minority OS bias contributed to this. Mike chatted to Rob Preston from the architecture team, who provided some expert advice on certificates and Parliament's network topology. Samu threw in a few ideas for possible solutions concerning routing, DNS, IP addresses and web-server configuration. Mike's quest ended when he finally found the team responsible for this setup. Unfortunately they claimed to knowing nothing about such 'web voodoo' but did replace the expired certificate with a valid one. No machines died.

### Domain modelling

Alison met with House of Lords Ed and House of Commons James to look at whether committee reports could be slotted into the existing document model. What we have now reflects a very simple structural model that doesn't get us much past slightly improved HTML output. For both library briefings and committee reports there is more underlying structural data that could be exposed which points back to the reproducible research angle that Tony was experimenting with. In many cases the data is statistical but for committee reports includes more parliamentary business data such as committee memberships, recommendations, minutes of meetings, and the business items that were part of those meetings. In the longer term there's a feeling that we need to move away from serialising documents and toward a model that's more an ordering of decorated transclusions. Michael is planning for more Tony chats.

Alison spent some time discussing the initial information architecture for visiting Parliament with the Collaboration team and spoke to Sarah from the Visiting team about the ticketing category model. She also expanded the Visitor Events domain model to introduce the concept of a Series as well as a Season of visitor events. Series of business items (debates, PMQs, questions and answers) are an idea Anya, Robert and Michael have been playing around with in respect to tabling and time tabling. So there's some overlap here. Although to Michael every nail tends to look like the Programmes Ontology.

Anya and Michael made a couple of minor changes to the laying and tabling models to make them more fag packet like. They also met with Stephanie Hunter who's doing an audit of the Parliamentary Computational Section, to chat about their work and how it fits into (or occasionally doesn't) the wider picture. And whether there's a wider picture.

### Data platform

Work continued on the SI tracker service to pick up all the bits that weren't possible for launch. Anya, Samu, Matthieu and Michael had a long chat interspersed with many fag breaks to chat about the legislation, tabling, time period and laying models. Once those are in place and we have a working calendar all the known knowns of SI tracking will be done. From our end anyway. Matthieu continued to probe via Michael, via Jamie, via Ben, via Kirsty Mc Askill (House of Lords head of business data) the quality of data in our existing calendar application. We're starting to hit interesting question about what a business item is and how that relates to parliamentary procedure.

Matthieu ploughed on with the physical ontology in the absence of Chris (get well soon) and had more conversations with Samu, Jayne, Michael, Anya, Mike and Wojciech. He's started to refine some of the functional properties and sub-properties and, apparently, had fun doing it. He's also been read Semantic Web for the Working Ontologist, How Parliament Works and assorted technical recommendations from the W3C. Which is some kind of sweet spot.

### On search. And indeed indexing

Matthieu has been furiously fighting the newest Vocbench to make it run on app services. With no noticeable signs of succes. Yet. Armando, the maintainer, has been, as ever, most helpful. And we're sure success shall ensue at some point. Hopefully. The team talked again about getting a Java professional for a day a week. Which might help.

Liz and Robert talked in some detail about the work he's done on recognising unclear or unhelpful content or title text display on search results. They talked about how they'd turn Robert's pixel thoughts into reproducible analysis that has the benefit of input from different people. And supporting what he wants to achieve rather than being lead too much by the approach. Although Liz points out everything he went through was sound, as usual. They talked about methods of assessment and analysis and what they'd like to implement in the future. But for now there are many quick and simple things that can be done to improve search result display.

Sara reports that new tracking code has been added to [Parliamentary search](http://search-material.parliament.uk/). An unusual number of requests searching for 'horses' and 'farms' were noted. Agricultural searches were running ar one request per minute. Which is a lot. For us. After chatting to Mike, Sara discovered that the 'horses' search is used for monitoring the service. Farms we're still less clear on. The good news is we can now filter these out as operational synthetic searches. Which might make our numbers go down but at least be more accurate.

The data analysts moved their work relating to search into the public document library on the data and search Sharepoint site. We're not given a URL so I'm not sure of the definition of public here.

Matt has been looking at creating a method for determining when certain measures on and around search have changed. Things like how much would the percentage of people searching for something but not clicking on any of the results need to change, and over what time period, before we considered it to be a significant difference.

Matt and Sara visited the Indexing and Data Management Section in the House of Commons Library to observe Jason working on a data task. Their goal is to be able to predict when action will be required in these tasks. Seeing Jason at work and a task being done gives them lots of useful context around this work.

### Corporate data

The beloved [Biztalk](https://en.m.wikipedia.org/wiki/Microsoft_BizTalk_Server) continued to explode in assorted faces. As is its wont. David, Lew, and Noel had another tough week wrestling with Microsoft's finest. Aidan stepped in to help out with coordination, prioritisation and communication. A few other colleagues from the department were drafted in. Cos, let's face it, no one's gonna volunteer here. Microsoft were called. Presumably someone slipped a flat snack under a door in Seattle because some progress was made. By the end of the week Noel was making sure that missing records were getting manually updated. Because that's why we have computers. Davis also got 90% of the way to implementing a change that should see some improvements. You'd hope.

### Did anybody fill in anyb forms?

Aidan and Liz talked through how we support our business intelligence software and filled in the service group form. It would be good to move away from requests needing to be channeled through Liz. She'd like to build in the option for users to read the framework before getting a licence and get to the point where the application is just something that's there rather than anyone having to request it.

Michael's security pass expired and he had a slight run in with the chap in the pass office. So Anya had to fill in forms to get him into buildings. Thanks Anya.

### Strolls

Dan and Robert went for a stroll which turned into more of a punishing hell-trek through a sun baked Westminster in search of hot coffee. We'll be drinking fresh cactus juice soon. 

Eventually they did manage to find a small island of shade. At which point, things improved. There was some chat about watches and post-war Japanese manufacturing which are some of the many and varied things Robert knows about. Maybe a milkshake next time lads?

Anya, Robert and Michael took a stroll to St Martha's church out in the Surrey hills. Anya saw England for the first time and was most impressed. Ben was supposed to join them but his teeth fell out so sadly couldn't show. We know you're thinking this was a log stroll for a working day, but it happened on Saturday and they took a train. They did talk a little about work though so should probably bill Parliament.

### Things that caught our eye

* [Magical thinking about machine learning won’t bring the reality of AI any closer](https://www.theguardian.com/commentisfree/2018/aug/05/magical-thinking-about-machine-learning-will-not-bring-artificial-intelligence-any-closer)

* [Has Machine Learning Become Alchemy?](https://medium.com/@Synced/lecun-vs-rahimi-has-machine-learning-become-alchemy-21cb1557920d)

* [The Emoji Report](https://www.brandwatch.com/reports/the-emoji-report/view/)
















