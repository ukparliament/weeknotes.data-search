## Week 9: 22-09-2017

### Community

Dan met with Rob, Henry and Frank from the ONS data visualisation team thanks to an invite from Oli. All great stuff.

### Parliament in the area, we're international, we're continental. But we're still south of Glasgow



### Domain modelling

Michael continued to investigate Oli's candidate database via the medium of prodding it with a Rails app. There's been some murmuring that this might come in the direction of the Data and Search team so we wanted to check [our data models](https://ukparliament.github.io/ontologies/) can cope. On Wednesday, Anya, Silver and Michael met with Oli to chat through the details of his relational database. Some changes were made to the [Election Ontology](https://ukparliament.github.io/ontologies/election/election-ontology.html) to capture a few things that were missing:

* Individual elections now have a [declaration time](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e245) 

* A [Boundary set](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e431) class was added

* Some existing predicates were reversed to make it more legible

* [Constituency Group](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e499) was moved from between [Constituency Area](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e477) and [Electorate](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e535) when Oli pointed out that population stats are recorded on a completely different cycle to elections

* [Recorded date](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e337) was added to [Population](https://ukparliament.github.io/ontologies/election/election-ontology.html#d4e594)

Michael and Samu met with Colin and Steve to chat through user needs and constraints for adding voting records to member pages on [the new website](https://beta.parliament.uk/). Plans were made to initially target professional users.

Michael met with Ed to chat about committee data and what we do next.

Michael also gave a quick presentation to the website team about where we're at with modelling government departments and positions and incumbencies and some of the data quality issues we're seeing.

Anya, Silver and Michael met Angela to check our modelling of select committees against the data in existing systems. We think we've captured everything worth capturing in the Committee Office Database (used in the House of Lords). We still need to check against Red Book (used in the House of Commons). Anya and Michael continued to revise the [first draft of the government department model](https://github.com/ukparliament/ontologies/blob/master/_government-department/government-department.png).

Anya, Silver and Michael also spent some time tidying our slides for the [Euro IA conference](http://euroia.org/) next week.


### Data quality


### Data platform

Samu implemented content encoding in the API that sites behind the new website. Data travelling from the data service to [the new website](https://beta.parliament.uk/) (and other public consumers) is now compressed, resulting in faster queries and a improved user experience.

Chris set up a local instance of [Webvowl](http://vowl.visualdataweb.org/webvowl.html) for use when theirs is down (which it frequently is).

### Search


### Machines that do learning

Raphael (and a bit of Ben) went along to [THINK AI for the Public Sector](http://www.thinkdigitalpartners.com/event/think-ai-publicsector/). Michael poured some scorn.


### Measuring things



### Excellent customer service awards

After spending a part of last week helping a political science PhD student from the [Federal University of Minas Gerais](https://en.wikipedia.org/wiki/Federal_University_of_Minas_Gerais) get data on gender representation in the House of Commons, Mike received a note to say, "You have no idea how much time and money you've saved me - I really can't thank you enough." Thanks also to the usual expert help from Joe Foster.


### Capability


### Corporate data

Dan met with Rupert, king of the architects, to talk about getting a new architect for our internal, 'corporate' data work - what we do over the coming years and things of that nature.

### Did anybody say blockchain?

One person said blockchain ¯\_(ツ)_/¯

### Strolls

No strolls were reported.

### Things that caught our eye

* [The Open Data Institute on why we need the Data Ethics Canvas](https://theodi.org/blog/why-we-need-the-data-ethics-canvas)

* [Knowledge and the Shock of Hypermedia: Thoughts From ISKO UK 2017](https://16blue.me/2017/09/18/knowledge-and-the-shock-of-hypermedia-thoughts-from-isko-uk-2017/)
