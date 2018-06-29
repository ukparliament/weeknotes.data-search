## 2018 Week 26

### Parliament in the area, [we’re international, we’re continental](https://www.youtube.com/watch?v=pNfHoPIxhXM&t=1m9s)

[Matthieu](https://twitter.com/cognithive) dabbled with some top of the range  international collaboration, sitting in on a WebEx organised by [Derek Alton](https://twitter.com/DerekAlton) from the Canadian Government. A bunch of people talked about the development of an open source suite of digital tools and platforms designed to help people come together to work on civic issues.

### Community

Not an awful lot in the way of community this week, although [Anya](https://twitter.com/bitten_), Robert and [Michael](https://twitter.com/fantasticlife) did meet [Paul](https://twitter.com/psd) for a pint or four down the [Strangers' Bar](https://en.wikipedia.org/wiki/Strangers%27_Bar). They attempted to put their [small corner of the world to rights](https://twitter.com/fantasticlife/status/1011714343979945984). But got distracted by beer. Quite heavily distracted if we're honest.

Anya and [Silver](https://twitter.com/silveroliver) met with [Helen](https://twitter.com/octodude) to plan the talks around ontologies and domain models they're due to give at [NetIKX](http://www.netikx.org/) later in the year. It went well, we're told. Some beer, but perhaps unsurprisingly, in smaller quantities.

### One world, one web, one team

[Alison](https://twitter.com/oliala), [Jamie](https://twitter.com/oddtype), [Matt](https://twitter.com/mattrayner) and [Samu](https://twitter.com/langsamu) talked to Tim Barnes and Gary Moore from the Business Systems Development team about their new Committee Management System. They discussed the data model, the import of data to the platform, the website and many other things. Samu says it was all very promising.

Thanks to the efforts of our Liz, [AppInsight](https://docs.microsoft.com/en-us/azure/application-insights/app-insights-overview) tracking is now live on [www.parliament.uk](https://www.parliament.uk/). Liz would like to thank Matt and Naz for approving the change.

For the past few weeks we've had something of a problem with parliament.uk subdomains not working on Parliament issued laptops as soon as they wander too far from [the Palace](https://en.wikipedia.org/wiki/Palace_of_Westminster). [Universality](https://technologyvoice.com/2010/11/23/tim-berners-lee-three-principles-of-the-web-universality-decentralisation-and-separation/) taking something of a kicking here. Given the number of people working remotely this is a bit of a bugger. Anyway, [Aidan](https://twitter.com/aidan_morgan)'s been busy working with John Hudson and they've managed to make some progress. Which means we can never escape work. Thumbs up Aidan.

Samu, Wojciech, and Mike met with some PDS colleagues to talk about how they rebuilt the systems they recently migrated to the cloud. They talked about using [PaaS](https://en.wikipedia.org/wiki/Platform_as_a_service) solutions and automated monitoring. They also spoke about assorted benefits, pitfalls and mitigations. David talked about the challenges the Data Integration Team are facing in moving cloudwards.

### Domain modelling

On Monday Anya and Michael went along to a House of Commons lecture on [statutory instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)). In truth they didn't learn all that much. But that's because Jane and [Jack](https://twitter.com/jackpdent) have been such excellent teachers. There's pretty much nothing left to learn here. Which should stand them in good stead should they ever wish to attend a clerks' pub quiz.

Anya, Alison, Silver, Michael and Robert spent most of Tuesday [drawing lines between the assorted models they've created to date](https://twitter.com/fantasticlife/status/1011602653208612865). And spotting errors. And duplications. And typos. Actually Frankenstein was the scientist's name.

Thursday was a flowchart day. As was Friday. We really don't have enough flowchart days. Anya and Michael made a few changes to the [statutory instrument flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples). Opposing decisions now preclude each other, decisions on motions preclude motions being withdrawn, deferred divisions have been added, and new bubbles to account for debates being rescheduled also made the cut.

Thursday also saw a meeting with Jane, Jack and [Ben](https://twitter.com/benwoodhams) to go back through [the flowchart for proposed negative SIs](https://github.com/ukparliament/ontologies/blob/master/procedure/proposed-negative-sis/proposed-negative-sis.pdf). Jane brought counterfeit smarties. Probably from some bloke in Camden. Now that the EU Withdrawal Bill has received [royal assent](https://en.wikipedia.org/wiki/Royal_assent), we finally know the shape of the procedure. Given several amendments didn't make it, the final version actually got simpler. So that's good. Thanks again to Jane and Jack. They've both been an absolute delight to work with. Not to mention patient.

Jane, Anya, Jack, Ben and Michael all went along to a big meeting on SIs in light of Brexit with assorted people from the [Parliamentary Computational Section](https://pds.blog.parliament.uk/), wider Parliament, the [Department for Exiting the European Union](https://www.gov.uk/government/organisations/department-for-exiting-the-european-union), the [government computational section](https://gds.blog.gov.uk/) and [The National Archives](http://www.nationalarchives.gov.uk/). Everything seems to be on track. [John](https://twitter.com/johnlsheridan)'s sleeping patterns were added to the risk register.

Alison and our Liz had a chat about modelling measurement. Alison also spoke to the workspace management project team about space data and tried to identify stakeholders for future modelling sessions. There was another meeting with Mary-Jane and Emma from the [Collections team](https://www.parliament.uk/about/art-in-parliament/collection-administration/) about how space data impacts their work. She's also been spending time comparing the physical ontology to the [domain models](https://ukparliament.github.io/ontologies/) and looking at understanding and improving the product data information architecture for the [online shop](https://www.shop.parliament.uk/).

### Data platform

Our Samu converted the Query Service to use a new content management vendor. We launched a [first iteration of long-form article "content"](https://beta.parliament.uk/collections/6i8XQAfD) (dread word, we know, we're sorry) on the new website a while ago. [Chris](https://twitter.com/chrisalcockdev), Jamie, Jenna, Joshua, [Librarian Liz](https://twitter.com/greensideknits) and Samu all chipped in, with actual words from Joanna Dodd and John Newton.

Platform changes included an enhancement to the Query Service which connects to the CMS provider and converts the data into a form the website can easily consume. 


A variety of commercial and technical issues were identified during the initial work, requiring a move to a different [headless CMS](https://en.wikipedia.org/wiki/Headless_CMS). Sam Thompson orchestrated and managed the business relations and Samu made the software change to accommodate the new solution. This part of the transition went well.

There's still some outstanding work to migrate the actual words from the previous place to the new one. As well as some touch up work on [beta.parliament.uk](https://beta.parliament.uk/).

Elsewhere, in hot, fresh [OData](http://www.odata.org/) news, our service has once again been used as [an example for querying endpoints more efficiently](https://blog.crossjoin.co.uk/2018/06/27/odata-performance-power-bi/). More applause [Jianhan](https://twitter.com/jianhanzhu).


### On search. And indeed indexing

Matt started looking at how people use filters on [Parliamentary Search](http://search-material.parliament.uk/). Unsurprisingly, different filters are used differently. Since the start of 2017, the content type filters have been used over 250,000 times, the transferred question filter has been used only 74 times, and the poor old EC document number filter has been used a grand total of twice. Though they are rather well hidden.

### Corporate data

[Dan](https://twitter.com/dasbarrett) made it to four of the five data integration daily sit downs. They've been working on establishing the [Kanban](https://en.wikipedia.org/wiki/Kanban) board to support the team's delivery and workflow. Progress is being made. Albeit slowly.

He also did some Service Ownership for the Interaction Management Programme, including a workshop about the language we use and making preparations for building a new software development function. And he’s been working with Bridget (new Data Architect for internal stuff) on the data strategy. And putting her in touch with assorted data architects across the UK public sector.

Our Liz and Lew met Jane and Ronke to talk about progress on untangling corporate [KPI](https://en.wikipedia.org/wiki/Performance_indicator) reporting from the linguine soup that is SharePoint. They agreed that managing reference data would be best done in Excel, so long as they can enable auditing. Liz had a slightly red face as she admitted she didn't know Excel had track changes. She’d like to thank Lew for pointing it out, although she has some understandable concerns that the feature is labelled ‘legacy’. They're planning to go along to the Performance Managers' meeting next month to share the work. Which should cover a few more teams' KPIs by then.

Lew began creating guidelines to help the data integration team with requirements gathering. Particularly around project work with other teams. He also continued development on the new finance transaction integration for the House of Lords.

Lew's also continued work with [Power BI](https://en.wikipedia.org/wiki/Power_BI) and his restructuring of the existing reporting solution, as well as preparing more parts of the new stock system integration for testing.

Noel’s had his head buried in People Data. The way in which primary jobs are assigned to people and the way in which a person's organisation is obtained have changed. The process for creating people records is currently under review. Hopefully we can achieve a more accurate interpretation of the various data sources.

David's been spending time with the space / location management system. Again it's under review. Again they aim to make the data more accurate. 

### Customer service of the week award...

...goes to mighty Samu, who helped a chap called Alasdair with [a query about searching the House of Commons division API](https://twitter.com/langsamu/status/1012322076517117952). Samu gave him a workaround and [Alasdair went away happy](https://twitter.com/Hulavoo/status/1012336350807384065).

### Employee of the week award...

...goes once again to Jayne, because if we don't keep giving it her, she might stop frantically adding statutory instrument data and then we wouldn't have an [SI tracker](https://beta.parliament.uk/statutory-instruments). Which would make us all sad. It's basically just bribery at this point.

### Strolls

Don't be silly. It's been way too hot for walks. Though Anya, Robert and Ben did make it as far as the park before promptly falling into the grass. And Dan met Robert a couple of times over fizzy water. They talked about search. Unsurprisingly. Which is suddenly and perhaps surprisingly looking promising again.

Other than that, what would usually have been Anya, Michael and Robert's strolling time has been spent sheltering from the sun and turning the Tothill Street canteen into an improvised junior common room. Or a fairly casual atelier. Or at the very least a salon. There's been some talk of replacing the sofas. CVs are being sharpened.

### Things that caught our eye

* [Design Thinking is Kind of Like Syphilis](https://medium.com/@sts_news/design-thinking-is-kind-of-like-syphilis-its-contagious-and-rots-your-brains-842ed078af29)

* [Data literacy should be the hottest skill to brag about in 2018](https://www.dataiq.co.uk/blog/data-literacy-should-be-hottest-skill-brag-about-2018)

* [Why You Don’t Need Data Scientists](https://medium.com/@kurtcagle/why-you-dont-need-data-scientists-a9654cc9f0e4)

* [Mozilla: Creating value from open practice](https://medium.com/mozilla-open-innovation/a-framework-of-open-practices-9a17fe1645a3)

* [The ODI Summit 2018](https://theodi.org/event/odi-summit-2018/)

* [Building the GOV.UK of the future](https://gds.blog.gov.uk/2018/06/27/building-the-gov-uk-of-the-future/) in which [Neil Williams](https://twitter.com/neillyneil) talks about a consistent domain model for government

* [Design, Modelling and Control of Aerial Robot DRAGON](https://www.youtube.com/watch?v=zMi5v2KznU4)

* [Microsoft Releases 125 million Building Footprints in the US as Open Data](https://blogs.bing.com/maps/2018-06/microsoft-releases-125-million-building-footprints-in-the-us-as-open-data/)

* [They drained a canal in Amsterdam and put everything they found online](https://belowthesurface.amsterdam/en/vondsten)