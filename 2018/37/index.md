## 2018 Week 37

### Babies

We’re delighted to announce that the break of dawn on Saturday was met with the [soft and gentle cries](https://www.youtube.com/watch?v=Su_l0d-st1k) of a new born baby. And [Jianhan](https://twitter.com/jianhanzhu) Jnr entered the world. No name as yet, we're sure it will follow along soon. Because our Jianhan is a [great computer scientist](https://martinfowler.com/bliki/TwoHardThings.html). And we probably need to settle on an identifier pattern first. Welcome aboard Jianhan Jnr.

In the very same week [Samu](https://twitter.com/langsamu) was also delivered of a new baby, in the shape of a [public SPARQL endpoint](https://api.parliament.uk/sparql). Joyful tears were shed. Samu has since been spotted wandering round the office with a rictus grin, 1000 yard stare and a cigar clamped between his lips. At least we think it's a cigar. We're told that mother and baby are both doing well.

### About that

As we've been building out the new data platform, we've prioritised the use of open standards. So our data storage layer is a [triple store](https://en.wikipedia.org/wiki/Triplestore) with a [SPARQL](https://en.wikipedia.org/wiki/SPARQL) access layer. It means every time you request a page on the new website, the web application queries the data platform with a pre-canned SPARQL query, gets back some data and renders a page. To oversimplify things.

We've also taken the approach that our website is our API. Or at least that data views should be available to match every page type. Try browsing [beta.parliament.uk](https://beta.parliament.uk/), view the page source and check out the [rel-alternate](http://microformats.org/wiki/rel-alternate) links. Truly beautiful. Brings tears to your eyes. We think.

The problem with this pattern is that it limits us to building the things we think of and have time for. As the graph of data expands, new ways of querying it become possible. And somebody, somewhere out there might want to query across the data in a way that we haven't exposed as a URL on the website. The word librarian springs to mind here.

So rather than restricting data access to pre-canned SPARQL queries and rather than restricting access to people inside Parliament, we now have a public SPARQL endpoint. Which means that anyone, anywhere can query our data in any way they find useful. And if we find common patterns we can roll them back into the website.

Team:Samu have been beavering away at this for a while, and [announced it on Wednesday](https://twitter.com/langsamu/status/1039950343088615425). Samu [encourages people to give it a try and kick its tyres](https://twitter.com/langsamu/status/1039950348901916674). For now, queries time out after 5 seconds and are rate limited to 10 per second per IP address. So no matter how ham-fisted you are, you can't do too much damage. Give it a whirl. [Let us know](mailto:data@parliament.uk) what you think.

[Matthieu](https://twitter.com/cognithive) has already started hacking around and made a quick [MP name lookup service](https://mp-names.cognithive.com/?name=Mouse) last night. You'd think he'd have enough of this stuff in his day job. Keen as mustard that lad.

### The delivery is the strategy

[Dan](https://twitter.com/dasbarrett) ran another data strategy open session. Which we're told attracted a good audience. He thinks it would be great if things continued in this fashion. You can [see Dan and his beard talking about it here](https://twitter.com/dasbarrett/status/1040238433627791360).

Dan also logged a call with the service desk to unblock [thebridalfile.co.uk](https://en.wikipedia.org/wiki/Binders_full_of_women) website. Which means we can unsubscribe from their marketing spam to the [data@parliament.uk](mailto:data@parliament.uk) inbox. And also maybe check out the latest in canapé trends and what have you.

### Community

Over in library land, work continued to decant [Michael Rush](https://socialsciences.exeter.ac.uk/politics/staff/rush/)'s card index files into spreadsheets. That said, it did almost come to a grinding halt. [Michael](https://twitter.com/fantasticlife) realised he'd made a schoolboy error with his original export of reference data. And that quite a lot of it was missing. He crept back to Tothill Street expecting only the disapprobation of librarians. But [Anya](https://twitter.com/bitten_) stepped in to help. And promptly ballsed things up to a completely new level. There was some sitting in silence. It was not companionable. Tuesday passed. But no strong words were issued and no punches thrown. They combined all of their brains and all of their computational skills and pulled off yet another audacious goalline clearance. From zeroes to heroes.

Anya and Michael met with [Lorna](https://twitter.com/laurnarobertson) from the Scottish Parliament to talk all things taxonomy and search and data. The subject of SEO came up but Michael was strong. He did not flinch. Or froth. He did ask for a trip to Edinburgh though.

### One world, one web, one team

Anya and Michael trotted off to the House of Commons Journal Office to see Mark Hutton, Clerk of Journals. They chatted about web analytics and user data and privacy. Particularly in the context of [online petitions](https://petition.parliament.uk/). More chats to follow.

[Sara](https://twitter.com/sarafreis) and Matt have been looking further into the use of [natural language processing](https://en.wikipedia.org/wiki/Natural_language_processing) to classify calls made to the helpdesk. They've been borrowing ideas from work by the Ministry of Justice analytical services on their [parliamentary questions tool](https://github.com/moj-analytical-services/pq-tool) and taken a turn toward [Latent Semantic Analysis](https://en.wikipedia.org/wiki/Latent_semantic_analysis). Sara and Matt got a proof of concept running, then Matt worked on it alone. And broke it. Luckily, Matt's also been chatting to Sam Tazzyman who was responsible for the MoJ work. Sam helped Matt get it working again. Thanks Sam.

In simple terms, Sara and Matt are looking at how often words are used together in sentences, as well as the words *those* words are used with, and so on, to group sentences by common topics. We're hoping that we can then use common topic-ness to help with assigning calls to teams. Sam also provided [a link to the more recent work](https://moj-analytical-services.github.io/NLP-guidance/) they've been doing, where you'll find some very good write ups on what this stuff actually is.

### Domain modelling

Anya, Robert and Michael continued with the long hard slog of editing model comments. It's like chipping away at a block of rock and failing to see a figure emerge. Anya and Michael get the feeling that Robert is trying to train them in the art of comment writing. Or English. They'd probably prefer it if he just rewrote them. Their trust is implicit.

#### September [spawned a monster](https://www.youtube.com/watch?v=Xv8LdKp2Y-8)...

The [draft affirmative procedure](https://ukparliament.github.io/ontologies/procedure/sis/draft-affirmative.pdf) changes that caused so much confusion [last week](/weeknotes.data-search/2018/36/#september-spawned-a-monster) have now been sense checked by House of Lords Jane and House of Commons [Jack](https://twitter.com/jackpdent). And declared to be sane. Or as sane as they're ever likely to get. Anya and Michael had hoped to add them to the [procedure data](https://procedures.azurewebsites.net/Procedures/3/graph) this week but the Rush data calamity cost them a day. So that's a joyful thing to look forward to next week.

### Data platform

Mike found some server errors in the Search Service telemetry and had a hunch that it was happening on searches with no results. Samu debugged and confirmed Mike's suspicions. Since we [upgraded to the latest version of Bing](https://ukparliament.github.io/weeknotes.data-search/2018/34/#data-platform), our code wasn't handling cases when the external search provider found no results.

Samu's grin temporarily disappeared when he thought he might have made the noobest possible programming mistake and not checked for nulls. But he soldiered on and did not [think badly of Sir Tony Hoare](https://en.wikipedia.org/wiki/Tony_Hoare#Apologies_and_retractions). A [fix was deployed](https://github.com/ukparliament/Search/compare/62a8797e22c12ba47bb5c28e71d76f71f65dce6b...a509da1ccabfbbf1570b4a456ac1e5c130f771b8?diff=split#diff-54a72b6692c682e402df897d42ada6c9R25) within the hour.

Mike continued to peer at the usage statistics for the Search Service and found that since the fault was introduced, only 1.38% of searches were affected. And that it wouldn't have been noticed by users because the search page just says 'no results' when the underlying service fails. Which in this case was actually true. So really 0% of searches were affected.

### On search. And indeed indexing

Sara continued with her investigations into search terms and the House of Commons Library [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri). Alex helped out by exporting a list of all the controlled terms in use. Which worked out to be 41,936 preferred terms and 27,130 non-preferred terms. Which is a lot of words. Sara took this list and and attempted to match it to search terms from four sources: our [new website search](https://beta.parliament.uk/search), [parliamentary search](http://search-material.parliament.uk/), the internal only parliamentary search and [Hansard search](https://hansard.parliament.uk).

To make things more manageable, the analysis covered the period from May to June 2018. It's not yet complete, but we have some numbers. So that's good. Out of 154,918 unique search terms, 67,082 matched with preferred terms and 23,042 search terms matched non-preferred terms. So a total coverage of 58%. Super.

### Corporate data

Noel and David wiped the sweat from their brows and emerged into a [rubble strewn landscape](https://www.youtube.com/watch?v=MrHoMSRZOS4&t=3m47s) to continue the configuration of their new development and testing environment. Noel continued to clean up the duplicate or incomplete records that exist on People Data following its recent explosion. And David reviewed an issue that's currently affecting the Time and Labouring System. Which sounds pretty dystopian.

Elsewhere Lew finished setting up our hosted dev machines so we can develop BizTalk solutions in a more stable environment. And made progress towards a test environment. Dan says this is important work. Lew also continued with the development work for the new catering finance system. Steamed pudding and custard being considered mission critical round these parts.

[Aidan](https://twitter.com/aidan_morgan), Lew, David and Dan worked through some potential SQL upgrades for the integration servers.

### Strolls

Nothing. Nada. All quiet on the stroll front. Although Anya, Robert and Michael did take a train to go and ride on some trains. Including this [absolute unit](https://twitter.com/fantasticlife/status/1038393479347535872). Sadly they did not ride on Thomas, because he was sat in a siding [with his face missing](https://twitter.com/fantasticlife/status/1038402425026224128). Michael feels he knows that feeling.

### Things that caught our eye

* Dan read the Harvard Business Review article on why [Design Thinking Is Fundamentally Conservative and Preserves the Status Quo](https://hbr.org/2018/09/design-thinking-is-fundamentally-conservative-and-preserves-the-status-quo) and why the alternative is messier, but more democratic. He does not offer an opinion here.

* Robert and Dan both read this article on how [Amazon is stuffing its search results pages with ads — and they seem to be working](https://www.recode.net/2018/9/10/17797720/amazon-is-stuffing-its-search-results-pages-with-ads).

* Sara listened to a [radiolab episode on hate speech and Facebook](https://www.wnycstudios.org/story/post-no-evil).

* Dan read a Google post on [Five insights on voice technology](https://www.blog.google/perspectives/scott-huffman/five-insights-voice-technology/). He also suspects Robert read it. Probably first. Or ^first^ as we used to say.

* Dan also read [Translating data ethics by Sarah Gold](https://projectsbyif.com/blog/translating-data-ethics) from [projectsbyif](https://twitter.com/projectsbyif) and took a look at their [9 practices for organisations operating digital services](https://s3-eu-west-1.amazonaws.com/projectsbyif.com/data-ethics-practices/9+practices+for+organisations+operating+digital+services.pdf).

* The [Government Computational Service are removing support for a whole bunch of data formats from their registers](https://www.registers.service.gov.uk/data-format-changes). We're not sure why. Or what [Roy](https://en.wikipedia.org/wiki/Roy_Fielding) might think.