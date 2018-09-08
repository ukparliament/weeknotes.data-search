## 2018 Week 36

### Dator day

Wednesday afternoon was supposed to be data day. But [Dan](https://twitter.com/dasbarrett) had childcare issues so it got cancelled. Well done, children.

### The delivery is the strategy

Dan's gone all in on data strategy stuff this week. He's currently preparing for a pitch to the Information Authority in a couple of weeks' time. He's also been doing some Service Owning for the Interaction Management programme. Mostly in the form of meetings. And generally trying to pull his head out of holiday mode.

### Community

Tuesday lunchtime saw [Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) take a short stroll across St James's Park to the [Institute for Government](https://www.instituteforgovernment.org.uk/). After partaking of a light lunch, they took their seats for the star studded [launch](https://www.instituteforgovernment.org.uk/Parliamentary-Monitor-2018) of the [Parliamentary Monitor 2018 report](https://www.instituteforgovernment.org.uk/sites/default/files/publications/IFGJ6416-Parliamentary-Monitor-Report-2018-1808-WEB-FINAL.pdf). The event was excellent as is the report. Your favourite [computational section](https://pds.blog.parliament.uk/) gets a nod or two and there's a constructive description of the ongoing difficulties people face when attempting to work with Parliament's data.

Late on Thursday, [John Sheridan](https://twitter.com/johnlsheridan) and Matt Bell, both of [TNA](http://www.nationalarchives.gov.uk/), dropped by library land to chat with Anya, [Jack](https://twitter.com/jackpdent) and Michael. There followed an hour of John's rather brilliant mind explaining some of the intricacies and patterns of legislation. With Michael attempting to capture a little of John's brain on a whiteboard. The meeting had been occasioned by a link to the [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) in [last week's weeknotes](https://ukparliament.github.io/weeknotes.data-search/2018/35/) which John had duly followed and hit upon some areas of concern. Twitter chats commenced and [John offered his help in explaining powers and duties](https://twitter.com/johnlsheridan/status/1035862660657696769) and how they interwingle.

Michael's now drawn [a new picture of the legislation model](https://raw.githubusercontent.com/ukpds/ontologies/master/legislation/legislation-powers.png) which we thinks captures some of John's intentions. We also think it brings us closer to fixing some of the concerns raised by [David Beamish](https://twitter.com/clerkly) last week. And we hope it is more pleasing to [our Samu](https://twitter.com/langsamu). Because Samu's happiness is important to us. Thanks John. Thanks Matt. Thanks David.

Anya, [librarian Liz](https://twitter.com/greensideknits) and Michael caught up on where we're at with [entering the Rush data](https://ukparliament.github.io/weeknotes.data-search/2018/34/#one-world-one-web-one-team). So far about a fifth of the card index files have been entered into the spreadsheet. With remarkably few questions arising. There are some things on the cards that don't fit into the current shape of the database. They decided to make additional sheets even if the data couldn't be slurped into the database yet. Emails were exchanged with [Paul](https://twitter.com/pseaward1) and [James](https://twitter.com/jamesjefferies). Progress was made. Go librarians.

[Alex](https://twitter.com/alexedwardh) finished getting a big chunk of data out of [Solr](http://lucene.apache.org/solr/) and sent it over to the lovely people of [Newspeak House](https://www.nwspk.com/). More details back in [week 33](https://ukparliament.github.io/weeknotes.data-search/2018/33/#community). He also sent some other stuff like [Matthieu](https://twitter.com/cognithive)'s [SKOS](https://en.wikipedia.org/wiki/Simple_Knowledge_Organization_System) vocabulary export and a TPG visualisation that Raphael made some time ago. We think they're happy with it.

### One world, one web, one team

Team data analysis showed and told how they're approaching their work on search data. In particular, splitting apart variations that can explained and variations that trace back to random process. Unfortunately the computational section was unable to provide either a working Skype camera or a slide projector, so no one got to see Matt's pretty pictures. Sad face, Matt. Feeling for you.

Pictures, pretty or otherwise, apart, they looked at how they might group search data to better investigate the behaviours and processes behind the observations. The general approach is to bucket by device type and weekday versus weekend since these often show significant differences. In measures that can be summarised as success or failure events, they're using the standard deviation of a binomial distribution to compare current observations to past observations. Which we're told is a general method and doesn't require a baseline to access a change. Liz says she enjoyed the discussion that followed about data driven baselines and KPIs. Each to their own I guess.

Our Liz met with Jenny and Tom, the communications and change managers for Skype and Office 364, to share some thoughts around creating KPIs. Jenny and Tom are running a workshop to identify what they need to measure to demonstrate the benefits of their work, creating common measurements where possible. They also talked about including measures that can relate their actions to outputs, to reflect the impact on the measures they create. Liz covered how team data analysis could help to assess measures and KPIs. We're planning to work with them further to develop their ideas.

Liz spent some time with [Julie](https://twitter.com/julietouring) helping her think about a workshop she's running with Jonathan Seller, Tori Baker and Peter Lamb. They're hoping to gather metrics that will help with with the People, Culture and Capability work. Which, as a rough translation, means Employee Satisfaction, HR recruitment and retention stats, skills gaps etc. Julie says Liz has been a great help in getting them to think about their approach to data and KPIs. Julie also says thank you.

Matt and [Sara](https://twitter.com/sarafreis) have been analysing data from service desk calls. In the first place creating a cooccurrence matrix by looking at how often pairs of words occur together in call descriptions. They're interested in seeing if there's any correlation between these word pairings, and the teams the calls are assigned to. They also broke this down by individual words, looking at where calls ended up if they contained the word 'Spire' or 'iPhone' or some such.

### Domain modelling

After several weeks spent [playing possum](https://www.youtube.com/watch?v=xIwwo--5meU), the [LODE](http://www.essepuntato.it/lode) service underwent a Lazarus like resurrection. So our HTML files are now back in line with [turtle](https://en.wikipedia.org/wiki/Turtle_(syntax)) files. Which is pleasing.

In the meantime, Samu has managed to deploy our own local version of LODE, so we don't get stuck the next time it goes down. More [details below](#data-platform). In a different corner, Robert has been chipping away at his own turtle to HTML translator. Results so far look good. The LODE service is handy but it doesn't pick up all of the data in the turtle. So once the HTML is generated there's some manual cutting and pasting and bodging and fudging. Which our ham fists occasionally get wrong. Given we have more control over Robert's translator, we can easily tune it to pick up new vocabularies and new data properties. Which means the HTML expression remains closer to the model and less stuff can go wrong.

To that end Michael and Robert have been tinkering with ontologies, adding image links, authors etc. Which was all stuff we've been ignoring for months because LODE didn't pick it up. As a side benefit, the Robert powered parser choked on our use of rdf:isDefinedBy. Which, as any fule kno, should have been [rdfs:isDefinedBy](https://www.w3.org/TR/rdf-schema/#ch_isdefinedby). An error we'd copied and pasted 700 times and which hadn't been spotted by LODE. So that's also now fixed.

Following on from last week's meeting with David Beamish, Anya, Robert and Michael gave the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html) a minor tweak. The [subjectTo](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e161) predicate is now hanging off the [work packageable thing](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e291), which, at least for now, is either a [statutory instrument](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) or a [proposed negative statutory instrument](https://www.parliament.uk/site-information/glossary/proposed-negative-statutory-instrument/). Rather than off the [work package](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e278). Which all feels neater and truer to the domain language of Parliament. Although this might also go as we flesh out the legislation model and powers and duties. John remains in charge here.

Last week's weeknotes had a [slurry of words](https://ukparliament.github.io/weeknotes.data-search/2018/35/#domain-modelling) about the problems the procedure model has with self-preclusion and steps that can be [actualised](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e22) many times in series but not in parallel. I won't repeat them here. Off the back of this Anya and Michael tweaked both the [flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples) and the [procedure data](https://procedures.azurewebsites.net/) to remove some self-preclusions and some withdrawal to decision preclusions. Fascinating stuff.

Off the back of a meeting with Jack they also found out that there can only be one non-fatal motion for the negative procedure in the House of Commons. Which presumably Jack had already explained and they'd drawn wrong. This is now fixed in both flowcharts and data.

Anya, Robert and Michael continued with their 'comment blitz' in a bid to improve all the comments across the models. They probably rewrote three before getting distracted by Daily Express comments. But they were a good three. As was the Daily Express comment.

#### September [spawned a monster](https://www.youtube.com/watch?v=Xv8LdKp2Y-8)...

...in the shape of statutory instrument [withdrawal](https://ukparliament.github.io/ontologies/laying/laying-ontology.html#d4e279) in the [draft affirmative procedure](https://procedures.azurewebsites.net/Procedures/3/graph). We had hoped to avoid modelling withdrawal in the procedure data, on the assumption that withdrawal kills everything and withdrawal is always possible. But it turns out withdrawal can only happen before decisions in each House. So we had to capture withdrawal precluding some things, withdrawal causing some things and decision points precluding withdrawals. Dear reader, we are sorry. You'd have to be [Erskine May](https://en.wikipedia.org/wiki/Erskine_May) with a cheap Dell to find any of this interesting.

For all these reasons, Anya and Michael had yet another meeting with Jane and Jack to draw even more lines on the draft affirmative flowchart. This has now been tidied. To the extent that this horror could ever be described as tidy. It's now awaiting sign off from Jane and Jack before we make the data changes. I mean, [look at it](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/draft-affirmative-with-withdrawal.pdf). Absolute state of that.

### Data platform

In happy news, our [Rebecca](https://twitter.com/rklappleyard) has returned to the fold. And has been busy writing [an assortment of SPARQL queries](https://github.com/ukparliament/Query/tree/master/Parliament.Data.Api.FixedQuery/Sparql) for the purposes of tracking statutory instruments. Way back in [week 7](https://ukparliament.github.io/weeknotes.data-search/2018/07/#data-platform), Samu added checks on our public repository so that developers collaborating on [SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries could get feedback on whether their changes had worked. Or crashed. Or burned.

The return of a [super-productive Rebecca](https://github.com/ukparliament/Query/pulls?q=is%3Apr+author%3Akatylouise+created%3A2018-08-24..2018-09-10) prompted Samu to add pull request cloning from [GitHub](https://help.github.com/articles/about-required-status-checks/) to [VSTS](https://docs.microsoft.com/en-us/vsts/pipelines/build/ci-public#validate-contributions-from-forks). Which makes it much easier to review and merge changes to the [Query API](https://medium.com/@langsamu/api-parliament-uk-7b87597019a4#2b73). Which means web developers can work faster.

For the past few months we've been using [LODE](https://github.com/essepuntato/LODE) to generate human readable pages for our [domain models](https://ukparliament.github.io/ontologies/). It's a piece of open source software created by [Silvio Peroni](http://www.essepuntato.it/), a senior assistant professor at the University of Bologna. Silvio maintains a freely available instance of the tool online. Unfortunately it's proved a little unreliable and is fairly frequently unavailable. Twitter calls have gone out and Silvio has kindly kicked it back to life. But it's not good that we've been relying on an unsupported tool for something so crucial.

So Samu's now deployed our own local instance which runs on an Azure App Service. It's deployed by a [VSTS](https://visualstudio.microsoft.com/team-services/) build script from the LODE public source control repository on GitHub. And it's running on a free plan so doesn't cost anything to run. The whole thing took some time to get working because LODE isn't really built in a robust way that facilitates cloud deployment. It relies on either the ontology source being RDFXML (which ours aren't), or on the [OWLAPI](https://github.com/owlcs/owlapi) to convert it from other formats to RDFXML. For some reason, Samu's version can't seem to find the OWLAPI library, so the second option is not an option. This is either because it's wrong (works on the developer's setup but fails elsewhere) or because Samu's no good with Java.

In truth, none of us are any good with Java. Which is a pain considering more and more of our services are written in Java . Samu thinks we've done a good job making these all happen and gives credit to Wojciech on [GraphDB](http://graphdb.ontotext.com/), Matthieu on [VocBench](http://vocbench.uniroma2.it/), and [Chris](https://twitter.com/chrisalcockdev) on [WebVowl](http://vowl.visualdataweb.org/webvowl.html). But he also thinks we'd benefit from some expertise here. Which doesn't mean we need permanent Java capability. But some serious Java mentoring would do us good.

In the absence of OWLAPI, Samu resorted to [EasyRDF](http://www.easyrdf.org/converter) (thanks [@njh](https://twitter.com/njh)), another free online tool that converts between RDF serialisation formats. Which is either another hack or a true embracing of loosely coupled web architecture. Depending on your particular sense of aesthetics.

The only actual modification Samu made to the LODE source is the addition of a [custom HTML homepage hosted on Gist](https://gist.githubusercontent.com/data-parliament/f84b294fc2fdeebf7b038d0663f90cce), which the automated deployment injects into the installation. This homepage retrieves a list of ontology folders from the domain model repository on GitHub and generates pre-parametrized download links.

### Corporate data

Judging by the email your correspondent received, Noel was on his tod this week. Poor Noel. He's been looking through more tickets on the incident management system. He's also created a [stored procedure](https://www.goodreads.com/quotes/4857-ginny-said-mr-weasley-flabbergasted-haven-t-i-taught-you-anything) to fix an issue in [BizTalk](https://en.wikipedia.org/wiki/Microsoft_BizTalk_Server).

Dan met with Liz to begin development of a few progress and performance measures for the integration engineers. We're hoping that Matt, Sara, David, Lew and Noel will work together to develop something useful.

### Strolls

No strolls reported, but we're told that Dan and Robert were planning one this very afternoon. No more details are available at this point.

### Things that caught our eye

* Samu read [fake news in the context of digital media by Alan Rusbridger](https://www.theguardian.com/news/2018/aug/31/alan-rusbridger-who-broke-the-news).

* He also read [architect Modern Web Applications with ASP.NET Core and Azure](https://docs.microsoft.com/en-us/dotnet/standard/modern-web-apps-azure-architecture/). Samu says it's the state of the art in cloud based Web development. All coming from Microsoft. Who, by coincidence, supply the technology we use in the Data Service. It all contributes to the long overdue work on upgrading our applications (Query, Search, Photo and OData) to the latest version of the web development framework.

* Liz flags up [a survey on exploring key performance indicators](https://www.sciencedirect.com/science/article/pii/S2314728816300034).

* Dan suspect Google's attempts to [make it easier to discover datasets](https://www.blog.google/products/search/making-it-easier-discover-datasets/) is quite a big deal.

* Michael wrote a post about [users and their endless neediness](http://smethur.st/posts/176135868) with help from Anya, Robert and [Silver](https://twitter.com/silveroliver). Unfortunately he found it trickier to publish than to write because he's buggered up his computer and can't access his website. Thanks again [@njh](https://twitter.com/njh).
