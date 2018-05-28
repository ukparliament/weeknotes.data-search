## 2018 Week 21

### More visions

[Dan](https://twitter.com/dasbarrett) has continued to have visions. Like Saul, shortly before he fell of his donkey. He's done a fair bit of data strategy stuff, chatting to people from all over the place about things like reporting data for projects, digital forms, data about spaces and places, and the requisite Customer Relationship Management systems.

He also took two inches forward on the long journey toward "providing a [register](https://gds.blog.gov.uk/2015/09/01/registers-authoritative-lists-you-can-trust/) of Members" type thingy. Two inches forward, one back. As they say.

### Showing and telling

Tuesday was show and tell day. [Sara](https://twitter.com/sarafreis) and [Matthieu](https://twitter.com/cognithive) recapped their trip to [TICTeC](http://tictec.mysociety.org/). Dan reports that it was *really good* with lots of learning and reflection on the international state of civic tech. Dan say it's the kind of stuff that gets him into work. As opposed to getting paid for instance. He's put Matthieu in touch with [Ed Saperia](https://twitter.com/edsaperia) at [Newspeak House](https://www.nwspk.com/) in the hope we can run or participate in an event on this theme. And next year, hopefully, we might even present at TICTeC ourselves.

### Community

No time for community this week. Really much too busy for friendships.

### Domain modelling

On Tuesday, Robert, [Silver](https://twitter.com/silveroliver) and [Michael](https://twitter.com/fantasticlife) took a trip to [The National Archives](http://www.nationalarchives.gov.uk/) to compare legislation models in the hope they could get to a minimum model to support the new [statutory instrument](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) tracker. [Previous efforts](https://github.com/ukparliament/ontologies/blob/master/legislation/legislation.png) had made [John Sheridan](https://twitter.com/johnlsheridan) sad enough to lose sleep over. There's a [new sketch](https://github.com/ukparliament/ontologies/blob/master/legislation/legislation-redux.png) now, which they hope will give John a better night's rest.

In the afternoon, they spent some time with [Oli](https://twitter.com/olihawkins) and [Carl](https://twitter.com/carlbaker), both statistic researchers from the [House of Commons Library](https://www.parliament.uk/commons-library). They went back over [where they've got to on the model for publishing Research Briefings and documents in general](https://github.com/ukparliament/ontologies/blob/master/document/document.png). Oli and Carl seemed happy enough or at least pretended to be. On Wednesday [Anya](https://twitter.com/bitten_) and Michael spent some time with [Lucinda](https://twitter.com/lucindamaer), from the Parliament and Constitution Centre in the Library, going over much the same thing. There was a good chat about anonymity and privacy and the need for individual opt-ins for researchers having a URI, [ORCID IDs](https://orcid.org/) and modelled contributions. But, other than that, Lucinda also seemed happy. They still need to run the model by people in the [House of Lords Library](https://www.parliament.uk/business/lords/work-of-the-house-of-lords/lords-library/) and [POST](https://www.parliament.uk/post). 

### Data platform

The week, like many others, has been mainly dedicated to the tracking of SIs. The Indexing and Data Management Section in the House of Commons Library have started to enter test data for [business items](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e193) in [assorted SI procedures](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples). Many conversations have been had about the correct way to add dates to business items which might be slightly 'off-stage' and which pages to link to for each item.

[James](https://twitter.com/thevinternet) has been using the [workpackage visualisations](http://procedures.azurewebsites.net/packages_staging.html), made by Raphael and fine-tuned by [Samu](https://twitter.com/langsamu), to cross check the data entered by IDMS. He's been looking at whether business item data is correct, according to the relevant procedural model their [work package](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e284) is subject to. He's also been checking that the workpackage flowcharts render correctly according to the data ingested from IDMS. He's planning to report back to Anya shortly.

Jenna and James have both been focussed on surfacing all the data related to a work package and understanding the challenges around presenting information from a 'this is what *has* happened' perspective compared to a 'this is what *should* happen' perspective. The consensus is that we can't create a comprehensive view of what has *and* should happen. So we either have to pick one representation, or the other. For now the primary focus is on what *has* happened (via the recording of Business Items), but they have every intention of also creating a 'what *should* happen' view (according to the procedure data). Once they figure out a meaningful way of showing it.

The problem here is that we're attempting to render a tree from model of procedure that is most definitely a graph. Most of the business items have dates attached, but for some, like the Speaker's consideration of [EVEL certification](https://en.wikipedia.org/wiki/English_votes_for_English_laws), we have a date for the decision being published but not for the actual consideration. Which means we have to take into consideration when procedure determines they should have happened. Which means we have to span the procedure graph to get some sense of what led to what. Which is hard. Luckily we have Samu, who sat down to write some SPARQL and [40 hours later](https://twitter.com/langsamu/status/997583754720882694) came up with this [absolute unit of a query](https://gist.github.com/langsamu/37db908d8ba2633221aa161934193f24).

In non-SI related news [Jianhan](https://twitter.com/jianhanzhu) has now ingested over 176k written questions and 145 answer corrections into the staging environment. He's also fixed the synchronisation issue between [tabled questions](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) and their accompanying answers. There was an issue here whereby, when a question is originally tabled, it's given a URI. And when the question gets answered, the tabled one disappears and a new question with a new URI gets created. Jianhan has managed to link the two by their UIN and table date so we can now update the tabled question with its answers.

Jianhan would also like to point out our new [OData](http://www.odata.org/) API got used as an example in a post about [troubleshooting data refresh performance](https://blog.crossjoin.co.uk/2018/05/03/troubleshooting-data-refresh-performance-issues-with-odata-data-sources-in-power-bi-and-excel-using-fiddler/). So that's good.

### Data toolkit

Wojciech's been busy creating improved data entry mechanisms for procedural data using. Mike has helped out with testing and sharing with team:Anya who are laboriously entering data in preparation for launch of the thing formerly known as SI tracker. Applause team:Anya.

### On searching and indeed indexing

Samu and Mike dealt with an issue that involved an outage to [parliamentary search](http://search-material.parliament.uk/). It was initially caused by a brief failure to the cloud infrastructure under one of our VMs but fixing it took them on a journey through Parliamentary limits on registry changes, Windows patching, security vulnerabilities preventing communication between machines, and Java updates changing folder names because someone thought having the version number of the [JRE](https://en.wikipedia.org/wiki/Java_virtual_machine#Java_Runtime_Environment) in a file path was a great idea. Another win for the Parliamentary Computational Section.

[Alex](https://twitter.com/alexedwardh) spent some time with Liz to find a better temporary process in Python for downloading many JSON files from a blob store, merging them and processing for analytics work. Dear reader, I have no idea what this means either. Something to do with computers I suspect.

### Corporate data

Lewis has continued his work on restructuring the existing reporting solution, as well as preparing more parts of the new stock system integration for testing.

Noel has continued with the data cleansing work for records on People Data.

### Joiners and leavers

[Mat](https://twitter.com/matiasgermanico) has now left the building, heading toward the more enlightened climes of Denmark. Or somewhere in the general direction of Scandiland. Farewell Mat. Alison joined as our new data architect to the usual reception of an incorrect security pass and a bricked laptop. Welcome aboard Alison.

### Strolls

Dan took a couple of strolls with Robert. They ate their packed lunches in the gardens on the Embankment. Like tramps. They talked about search and the data strategy, and shared general reflections on how to work. Unlike tramps.

Anya, Robert and Michael took a trip to the [RAF Museum at Hendon](https://www.rafmuseum.org.uk/london/) where they say a real life [atomic plane](https://twitter.com/fantasticlife/status/997843968414142469). Wows. Then they accidentally went to a party.

### Things that caught our eye

* [10 Problems With Impact Measurement in Civic Tech](https://civichall.org/civicist/10-problems-with-impact-measurement-in-civic-tech/)

* [Why we have produced a Beta version of a new ONS API](https://digitalblog.ons.gov.uk/2018/05/24/why-we-have-produced-a-beta-version-of-a-new-ons-api/)

* [Using the new Beta ONS API](https://digitalblog.ons.gov.uk/2018/05/24/using-the-new-beta-ons-api/)

* [A bot writing poems from twitter](http://www.longestpoemintheworld.com/)

* [Understanding legacy technology in government](https://gdstechnology.blog.gov.uk/2018/05/24/understanding-legacy-technology-in-government/)

* Our Liz pointed to [Validate](https://cran.r-project.org/web/packages/validate/vignettes/introduction.html), an R package intended to make checking your data easy, maintainable and reproducible. She says it's less important that it's an R package and she's more interested in what it's trying to achieve. Validate allows you to test your data set(s) against predefined rules (either in- or cross-data set), import and export rule sets from structured or free-format files, investigate and visualize the results of a data validation step, perform basic rule maintenance tasks and define and maintain data quality indicators separately from the data.