## 2018 Week 40

### Dator day

Wednesday was [dator day](https://twitter.com/dasbarrett/status/1047467603114037249). Or half of it was. Our Liz, [Anya](https://twitter.com/bitten_), [Alison](https://twitter.com/oliala), Robert, [Paul](https://twitter.com/paulwakely), [Samu](https://twitter.com/langsamu), [Jamie](https://twitter.com/oddtype), [Dan](https://twitter.com/dasbarrett) and [Michael](https://twitter.com/fantasticlife) spent several hours locked inside the Archbishops' room which is really big considering there's only two of them.

There was a conversation around plans for [taxonomy](http://www.data.parliament.uk/dataset/thesauri) management tools which everyone seemed to think was constructive. Then Jamie outlined some short term plans for the [beta website](https://beta.parliament.uk/) in general and the [statutory instrument tracker](https://beta.parliament.uk/statutory-instruments) in particular. Immediate priorities being the ability to list [SI](https://en.wikipedia.org/wiki/Statutory_instrument_(UK))s (or at least [work packages](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e343)) currently before Parliament and SIs laid by a [laying body](https://ukparliament.github.io/ontologies/laying/laying-ontology.html#d4e51). Given the [laying model](https://ukparliament.github.io/ontologies/laying/laying-ontology.html) most of the domain model bit of this is done but currentness (or currentcy as Robert might say) is hard. Keep reading for [more details](#domain-modelling). Or stop now.

Your correspondent struggles to cover the rest of proceedings, since he threw a mard, (accidentally) knocked over the water dispenser and flounced from the room like a low-rent Laurence Llewelyn-Bowen. If you're craving more detail, there's a [photo with some ticks here](https://twitter.com/dasbarrett/status/1047521627955765248).

### Community

Dan headed off on another trip to Bristol where he gave a talk at [Delib](https://www.delib.net/)'s [practical democracy project meetup](https://www.eventbrite.co.uk/e/the-practical-democracy-project-meetup-bristol-tickets-49295154133#). Where, by pure chance, the theme of the night was fixing websites for Parliaments and legislatures around the world. Because no Parliament is a snowflake. You might say. Dan says he met lots of great folks and had many useful conversations. There were some tough questions about democracy and citizens and, perhaps unsurprisingly [user needs](http://smethur.st/posts/176135868). Which we're sure Dan answered with applomb.

On Thursday Anya and Michael were joined by librarians Jayne and [Liz](https://twitter.com/greensideknits), [James](https://twitter.com/jamesjefferies) and [History of Parliament Trust](https://www.historyofparliamentonline.org/) [Paul](https://twitter.com/pseaward1). They chatted about progress on the Rush data project from both a technical angle and a data entry point of view. Development work is almost done and Jayne and Liz reckon they've added about 50% of the Members from the last three intakes. The new plan is to switch data entry from a set of spreadsheets to James' application and see what breaks. If anything serious goes wrong we'll use the remaining time to fix bugs. If all goes to plan we'll use the time to add data downloads and handle identifier interlinking with Wikidata. The last bit seems easy enough so Michael has put James in touch with [Andrew](https://twitter.com/generalising) and a plan has emerged.

### The delivery is the strategy

With Dan down in Bristol, Alison took over on data strategy open session duties. Which attracted its usual hardcore audience and a smattering of new faces. Notable by his presence was Bill Boshell, an Information Manager from Strategic Estates. The session focussed on one specific principle from the data strategy, 'protect our data and consider privacy'. They discussed the practical implementation of this in relation to Bill's work on Information Asset Registers, Information Owners and training for users. We're told Bill left feeling like he'd had a thorough grilling. But we hope that won’t put him off attending future events.

### One world, one web, one team

[Sara](https://twitter.com/sarafreis) met with librarians Liz, Martin and Steve to discuss the results of her work to correlate search terms with the controlled vocabulary. They talked though the method in some detail and came up with a plan for improvement. The next step is to look at the list of search queries that did not match any terms from the controlled vocabulary to better understand if there are any topics / themes / words that users search for that are not in the vocabulary and could potentially be included as synonyms for what's already there.

Our Liz has been watching stuff on [reproducible analysis](https://lib.colostate.edu/services/data-management/reproducible-analysis/) to support our thinking on workflow and documentation. She thinks it would be good to get other people doing analysis thinking about reproducibility. The key point is having clear reasons behind each step taken to produce a result and making those decisions visible. Liz thinks this will help make analysis more relevant and convincing. She also points out that making decisions visible isn't specific to analysis and has been discussed in relation to other work. Michael is reminded of [Tony](https://twitter.com/psychemedia)'s thinking on reproducible research here.

### Domain modelling

The week started with a poorly Anya. Her nose and chest exploded almost simultaneously. We start to worry that she may not be smoking enough. Nevertheless, even with a librarian down, team:whiteboard ploughed on regardless.

Michael spent a chunk of Monday morning with [Martyn](https://twitter.com/martynpatrick), clerk bloke for the House of Commons [Procedure Committee](https://www.parliament.uk/business/committees/committees-a-z/commons-select/procedure-committee/). They talked through what exists of the [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) to date and feedback they've received from [David](https://twitter.com/clerkly) and [John](https://twitter.com/johnlsheridan) around powers and duties. Some words got nudged around.

Robert and Michael spent a large chunk of Tuesday diving back into the legislation model, tweaking some of the shape, some of the labels and some of the comments. They spotted [Nerys](https://twitter.com/Nerys_d) across Tothill Street cafe and managed to grab her to idiot check some words. It feels like the legislation model is getting to a stage where they're almost happy with it. At least for now. Thank Martyn. And David. And John. And Nerys.

Luckily Anya picked up her smoking and was able to return to work on Wednesday. Still spluttering slightly. But able to attend a meeting with librarian Jayne and Computational Section representatives [Bex](https://twitter.com/rklappleyard) and [Chris](https://twitter.com/chrisalcockdev). They began to crack apart what it means for a statutory instrument to be 'current', in a currently before Parliament sense. And thought they'd cracked it. They hadn't.

Luckily Robert's brain was available for a large chunk of Thursday, so Anya and Michael sat down with him and rewrote the rules, checked them three times and started to add 'no longer before the House' steps to the [procedural flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples). So far they've covered proposed negative statutory instruments and both of the negative procedures. Affirmatives to follow.

At some point they really need to bite the bullet and think about adding [logic gates](https://en.wikipedia.org/wiki/Logic_gate) to the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html). But they're comforted by the sound of Robert's brain grinding into gear on this.

### Data platform

[Matthieu](https://twitter.com/cognithive) worked on automating our deployment of [VocBench](http://vocbench.uniroma2.it/). He also wrote [a post](https://medium.com/@neiges/using-a-sparql-endpoint-to-generate-bash-scripts-5d8e6609d6da) about generating [bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) scripts using our [public SPARQL endpoint](https://api.parliament.uk/sparql) to help a [BBC](https://en.wikipedia.org/wiki/Blockbuster_LLC) person grab a bunch of our Member portraits more easily. And for anyone else wanting similar tips.

### Dashboarding all the measurements

Mike's been hard at work creating a dashboard view of our data platform API. It's fed by data from our analytics software and lists each endpoint by the percentage of failed requests, a breakdown of response codes per environment and the request URL of all responses tagged as failed over the last hour. It also shows the total number of API requests for all endpoints or per environment or per endpoint. Again with a breakdown by response. Top dashboarding Mike.

### On search. And indeed indexing

Following the recent deployment of new analytics software to the [website search service](https://beta.parliament.uk/search), our Liz took a look at the referrer info we're getting back. For any view of a search result page we can now see the page the user was on when the search was performed. Perhaps unsurprisingly, the top locations for users starting searches are the Member biography pages. Information about MPs and Peers accounts for a large proportion of our traffic. Which means we probably need to consider referrer page counts in the context of views of those pages.

### Corporate data

Bridget spent most of the week working on the upgrade of Dynamics CRM 2011 to Dynamics 364. There are plans to merge the three instances used by [POST](https://www.parliament.uk/post), Participation and the House of Lords Enquiry service into a single instance on what we are told is an 'evergreen platform'. She had a productive meeting with our third party supplier and is now able to put the finishing touches to a data migration framework for the project. She's hoping the migration framework might be that may be reusable across other projects and tap into our Liz's skills for data profiling.

### Paul's truly terrible week (slight return)

Paul did even more strategy-wrangling because there is no strategy for interlinking our assorted strategies. He also attended his first Data Day and I believe stayed to the end. And he went along to a workshop run by Alison and Bridget with Janis McAnallen and Andy Woods from Strategic Estates. Luckily he had booked Friday off because his head is now wrecked. But none of his teeth fell out. So that's an uptick in fortunes.

### Customer service of the week award...

No award this week. Nobody has been good enough to justify the cost of printing the badges.

### Strolls

Robert and Dan took a stroll to the finest coffee stall in SW1. Robert and Michael did similar. There was a shortage of any real adventure and a lack of real spice in our lives.

### Bridal news

Email spam from [The Bridal File](https://en.wikipedia.org/wiki/Binders_full_of_women) is still arriving thick and fast to the [data@parliament.uk](mailto:data@parliament.uk) inbox. This has something to do with the website being blocked and the service desk not having unblocked it. We're still hopeful this might happen soon.

Nobody got married.

### Things that caught our eye

* Matt read this post about [a man who used R to stop his rent getting increased](https://www.r-bloggers.com/rent-scraping-how-i-saved-money-using-r/amp/). It really is every man and his computer for himself these days.