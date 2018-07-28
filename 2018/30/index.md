
## 2018 Week 30

As the oppressive heat continued, summer [recess](https://www.parliament.uk/site-information/glossary/recess/) began. Strolls were reported, coffee drunk, a gift received and there was an international flavour to the week. It was all rather pleasant.

### Showing and telling...

[Dan](https://twitter.com/dasbarrett)  held the second 'open session' on the data strategy. He advertised this on Yammer. Fortunately for Dan, Debra came along. Dan says he found it useful to hear about the behaviours and issues of users of some internal systems. It's not entirely clear to us whether the systems or the users have the behaviours, or indeed the issues. It also helped him to think about the language of the data principles.

### Community
Dan gave a presentation about websites, data and democracy to a delegation from Malaysia. As is the way with these things, there were technical issues. Unphased, Dan got to his knees and worked his laptop upside down. He earned a handmade [necklace from Borneo](https://twitter.com/dasbarrett/status/1021752327362039808) for his troubles.

Marc Adams from the [National Audit Office](https://twitter.com/NAOorguk) got in touch. Marc is interested in tracking changes to committee membership and party affiliation using our [OData service](https://pds.blog.parliament.uk/2018/01/24/accessing-semantic-data-with-odata-web-interface/). [Samu](https://twitter.com/langsamu) put together some instructional material for him, and also created a [new endpoint](https://api.parliament.uk/staging/fixed-query/formal_body_membership_and_party_affiliation) on our query service that might serve the purpose better. If Samu received a necklace, he's kept very quiet about it.

Dan, Robert, Samu, Mike, [Matthieu](https://twitter.com/cognithive), and [Jianhan](https://twitter.com/jianhanzhu) met with Sukhin and Nick from the [New Zealand Government](https://www.govt.nz/). They talked about about data, legislation, systems, ways of working, being open by default, and search. All the good stuff.

### One world, one web, one team

Samu met up with Oswin Taylor, Legislation Document Manager in the House of Lords, to  discuss the processes involved in drafting [Private Members' Bills](https://www.parliament.uk/site-information/glossary/private-members-bills/). Samu thinks this could be improved through a combination of existing productivity tools and some information management advice.

[Anya](https://twitter.com/bitten_), Mike, [Sara](https://twitter.com/sarafreis) and Samu met with [Oli](https://twitter.com/olihawkins) and [Phil](https://twitter.com/statisticalphil) from the [House of Commons Library](https://commonslibrary.parliament.uk/). Oli and Phil are developing tools for subject based email alerts to [written questions](https://www.parliament.uk/site-information/glossary/written-questions/) and news articles. We think there's potential to help here, through both integration with the [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri) managed by  the Indexing and Data Management Section (IDMS), and by giving their application a better home on the Data Platform.

[Matt](https://www.linkedin.com/in/matthew-reed-b3b761105/) and Sara called by Tothill Street to visit Steve in IDMS. Over recess periods, IDMS take a breather from the daily round of subject tagging parliamentary business, to review and revise the subject tagging of parliamentary business. Steve identified three tasks that could be completed within a relatively short timeframe and found a volunteer (thanks Jason). Matt has scraped the information that Jason will be reviewing, and potentially changing, before Jason gets to work. This will help Sara and Matt to compare what has and what hasn't changed. Matt and Sara hope to use these differences to predict the change requirements for future tasks. They could provide these predictions, along with some level of confidence score, to IDMS. They hope it will lead to more informed decision making.

Our Liz and David had a chat about providing people keys to People Data users. Currently, users are presented with unconnected data sources and are developing individual approaches and tool-specific solutions to make links between them. 'Twas ever thus. Liz and David have an idea that it would be preferable if Data and Search made those connections instead. Liz notes that People Data doesn't save a history of keys; this could prove to be an issue and we should look at how we could capture that information.

Naz and Liz, with help from Christine and Allan, added App Insight tracking to more parts of website, the calendar and digital archives. There's still many more things to track, on pause for now though whilst the cookie policy is updated.

Dan arranged the first 'Data and Search II' team meeting. It went well. Everyone discussed their work for the next month, goals for the year and any issues the team could help with. Holidays were also on the agenda. The team were particularly envious of Matt, who's heading off to an EDM festival in Zurich. No, not that [one](https://www.parliament.uk/site-information/glossary/early-day-motions/). This [one](https://en.m.wikipedia.org/wiki/Electronic_dance_music).

### Domain modelling

Alison's had some feedback on the first draft of the [Visiting](https://github.com/ukparliament/domain-models/tree/master/Visiting) domain models and is working to update them. Recess has slowed down her quest to model House of Commons committee formation. Undeterred, she attended the kickoff meeting for the committee reports project and is looking forward to working more with James and Ed on this next week.

### Data platform

Written questions went live on beta this week, initially linked to from  [Members'](https://beta.parliament.uk//people/members/current) pages. A lot of work went into the domain and the data here,  roll credits: [domain modelling](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) by Michael, [Silver](https://twitter.com/silveroliver) and Anya, ontology authoring by [Chris](https://twittwr.com/chrisalcockdev), [import automation](https://ukparliament.github.io/weeknotes.data-search/2018/19/#data-platform) from Jianhan, and years and years of [indexing](https://www.slideshare.net/UKParliData/unlocking-the-indexing-and-search-data-goldmine) by IDMS.

The next round of work on the [Statutory Instrument service](https://beta.parliament.uk/statutory-instruments) is underway. [Matthieu](https://twitter.com/cognithive) implemented  [laying](https://ukparliament.github.io/ontologies/laying/laying-ontology.html) and [legislation](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) domain models in our physical ontology. Mike supported IDMS, who are constantly entering data, in moving to the latest version of the procedure editor, Wojciech implemented improvements to the editor, and Jianhan imported existing data from Search & Indexing into the data platform.


### On search. And indeed indexing

[Hints](https://ukparliament.github.io/weeknotes.data-search/2018/29/#showing-and-telling) went live on website [search](https://beta.parliament.uk/search?q=black+rod). [Jamie](https://twitter.com/oddtype) thinks Matt's [commit message](https://github.com/ukparliament/Search/commits/master) was the most beautiful, descriptive and context-aware example he's seen in a long time.

Our Liz, Sara, Matt and Matthieu, met with [Liz Marley](https://twitter.com/greensideknits), Steve and Anya from IDMS to discuss work to evaluate overlaps and gaps between the controlled vocabulary and search terms, and track changes over time. Next steps for the analysis will be to match search terms (both website search and the internal service Parliamentary Search) against all controlled terms and to break it down by class, preferred and non-preferred terms.

Mike found a solution to a longstanding issue with bad links in Search & Indexing. 38,000 items on Parliamentary Search and the external facing [search parliamentary material](http://search-material.parliament.uk/) were all linked to one of two incorrect locations in [Hansard](https://www.parliament.uk/site-information/glossary/hansard-official-report/). Mike found that using more complicated SPARQL without filters is vastly more efficient than using SPARQL with fewer lines but with filters. This meant that 100,000 transactions could be run without affecting performance for users. He's pretty confident we’ll be able to perform big updates to Search & Indexing inside business hours.

### Corporate data

Smouldering most weeks, BizTalk caught fire this week. No sooner had David and Lew resolved last week's problems (we're looking at you Windows update), than another issue flared up with one of the core integrations. David and Lew have had a torrid time. No time for strolls for them this week.

### Warm Strolls

This week's strolls are brought to you by Robert.

Dan had a stroll with Robert. In the baking heat. With coffee. They talked about [Google on-premises](http://uk.businessinsider.com/google-cloud-available-on-premises-to-take-on-microsoft-amazon-2018-7), amongst other things.

Our Liz inadvertently went for a stroll with Robert, whilst looking for somewhere to eat lunch in the park. As should have been obvious to everyone, it was too hot for strolling. Happily neither Robert nor Liz passed out. They talked about decorating cakes.

On their stroll, Samu and Robert talked about the past, present and future of everything. An ambitious agenda. They talked in particular about the next steps they think we should take in building our search service. What we do know is that it was scorching hot and the coffee was good. What we don't know is whether strolling itself came up during these far-ranging discussions.

Anya and Robert went for two strolls. Both involving coffee, conversation and yes, it was too hot. Search and controlled vocabularies, constructed and real data, pigeons and pirate ships all featured.

Robert has certainly put in the miles this week.

### Things that caught our eye

* Dan was pointed towards  the [Food Standards Agency](https://www.food.gov.uk/) (FSA) [data strategy](https://www.food.gov.uk/sites/default/files/media/document/datastrategy.pdf)


```

```
