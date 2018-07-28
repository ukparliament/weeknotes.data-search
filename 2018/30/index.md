
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









































```















```













```





## 2018 Week 30

This week saw the start of Recess, although the oppressive heat of Westminster carried on. Despite this, strolls were reported, coffee drunk, gifts received and there was an international flavour to the week. It all sounded rather pleasant.

### Showing and telling...

[Dan](https://twitter.com/dasbarrett)  held the second 'open session' on the data strategy he is working on. He advertised this on Yammer. Fortunately for Dan, Debra came along and Dan found it really useful to hear from her about the behaviours and issues that users of some of our internal systems have. It also helped him to think about the language of the data principles he is considering.

### Community
Dan gave a presentation about websites, data and democracy to a delegation of around 20 from [Malaysia](https://en.wikipedia.org/wiki/Malaysia). Despite some technical issues with the big screen, which saw Dan having to kneel and work his laptop upside down, he received the generous gift of a [necklace from Borneo](https://twitter.com/dasbarrett/status/1021752327362039808) for his troubles.

[Samu](https://twitter.com/langsamu) created some instructional material for Marc Adams from the [National Audit Office (NAO)](https://twitter.com/NAOorguk). Marc is interested in tracking changes to committee membership and party affiliation using our [OData Service](https://pds.blog.parliament.uk/2018/01/24/accessing-semantic-data-with-odata-web-interface/). Samu also created a [new endpoint](https://api.parliament.uk/staging/fixed-query/formal_body_membership_and_party_affiliation) on our Query Service that might serve the purpose better. If Samu received a necklace, he has kept very quiet about it.

Dan, Robert, Samu, Mike, [Matthieu](https://twitter.com/cognithive), and [Jianhan](https://twitter.com/jianhanzhu) met with Sukhin and Nick from the New Zealand Government and had a wide-ranging conversation about data, legislation, systems, ways of working, being open by default, and search. They thought it was a really good meeting.

### One world, one web, one team

Samu met Oswin Taylor, Legislation Document Manager in the House of Lords. They discussed the process of drafting Private Members' Bills and how this might be improved through a combination of existing productivity tools and some information management advice. They'll meet again next week to review the process in more detail and decide on  the first implementation step.

[Anya](https://twitter.com/bitten_), Mike, [Sara](https://twitter.com/sarafreis) and Samu met [Oli](https://twitter.com/olihawkins) and [Philip](https://twitter.com/statisticalphil) from the [House of Commons Library](https://twitter.com/commonslibrary) to talk about their new tool for creating email notifications for current awareness and about written parliamentary questions. The data and search team see a lot of potential to help them through both integration of the Indexing and Data Management Section (IDMS) controlled vocabulary and by giving their application a better home on the Data Platform.

[Matt](https://www.linkedin.com/in/matthew-reed-b3b761105/) and Sara visited IDMS and spoke to Steve about helping with the data tasks that IDMS undertake during recess. Steve identified three tasks that could be completed within a relatively short timeframe and found a volunteer, (thanks Jason), within IDMS to do one of these tasks. Matt has already scraped the information that they will be analysing, and potentially changing, before beginning the actual task. This will help them to compare what was and what wasn't changed, and use these differences to predict the change requirements for future tasks. They can then provide these predictions, along with some level of confidence score, to those performing these tasks going forward. They hope it will lead to more informed decision making.

Our Liz and David had a chat about providing people keys to people data users. Currently users are presented with unconnected data sources, all showing people, and are developing individual approaches and tool-specific solutions to make the links between them. They think it would be preferable if Data and Search made those connections instead. Liz thinks it may become an issue that people data doesn't save a history of keys, and that we should look at how we could capture that information.

Naz and Our Liz, with some help from Christine and Allan, added App Insight tracking to more parts of website, the calendar and digital archives. There are still many more parts to track, but they need to get the cookie policy updated before continuing.

Dan arranged the first 'Data and Search II' team meeting, which saw a different combination of people from the team together in a room. It went well. Each person discussed their work for the next month, goals for the year and any issues the team could help with. They also discussed their holidays. The team were particularly envious of Matt, who will be attending an Early Day Motion festival in Zurich. That shows true dedication.

### Domain modelling

Alison got some feedback on the first draft [visiting domain models](https://github.com/ukparliament/domain-models/tree/master/Visiting) and is working to update them. The start of recess has slowed down her quest to make progress with modelling how House of Commons committees are formed. Undeterred, she attended the kickoff meeting for the committee reports project and is looking forward to working more with James and Ed on this next week.

### Data platform

Following [domain modelling](https://ukparliament.github.io/weeknotes.data-search/11/#domain-modelling) work by Michael and team, [ontology authoring](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html) by Chris and [import automation](https://ukparliament.github.io/weeknotes.data-search/2018/19/#data-platform)from Jianhan, not to mention years of [indexing work](https://www.slideshare.net/UKParliData/unlocking-the-indexing-and-search-data-goldmine) by Anya's team, written parliamentary questions is now live on the new website. A great team effort!

The team was busy all this week with the next iteration of work relating to Statutory Instruments: [Matthieu](https://twitter.com/cognithive) implemented the domain model in our physical ontology, Mike supported IDMS, who are constantly entering data, in moving to the latest version of the procedure editor, Wojciech implemented improvements to the editor, and Jianhan imported existing data from Indexing & Search into the [platform](https://ukparliament.github.io/weeknotes.data-search/2018/19/#data-platform).


### On search. And indeed indexing

"Hints", as described in [last week's weeknotes](https://ukparliament.github.io/weeknotes.data-search/2018/29/), went live on [Search](https://beta.parliament.uk/search). Examples of some of the different hints in use can be seen [here](https://beta.parliament.uk/search?q=black+rod). The pull request is [here](https://github.com/ukparliament/Search/pull/2). [Jamie](https://twitter.com/oddtype) thought the associated commit message, written by Matt, was the most beautiful, descriptive and context-aware example he's seen in a long time.

Our Liz, Sara, Matt, Matthieu, [Liz Marley](https://twitter.com/greensideknits), Steve and Anya had a meeting to discuss the work that has been done on website search and IDMS vocabulary, described in [weeknotes 2018 Week 27](https://ukparliament.github.io/weeknotes.data-search/2018/27/). The purpose of this work was to evaluate overall performance of the vocabulary and track changes over time. They identified that the next steps for the analysis should be to match search terms (both website search and parliamentary search) against all vocabulary terms and break it down by class, preferred and non-preferred terms.

Mike found a solution to a long standing issue with bad links in Indexing and Search that went back to the initial population of data in 2012. This had meant that 38,000 items on search.parliament.uk and the external facing [search parliamentary material](http://search-material.parliament.uk/)sites had links that went to the wrong locations.

Mike also found that using more complicated SPARQL that doesn’t use filters is vastly more efficient than using SPARQL with fewer lines but with filters. This meant that 100,000 transactions could be run without affecting performance for users. In future, by not using filters, he thinks we’ll be able to perform big updates to the Indexing triplestore inside business hours.

### Corporate data

BizTalk was on fire this week, which means that David and Lew had a torrid time. They finally resolved last week's BizTalk issue, caused by a recent Windows update, but no sooner was that sorted, than they needed to investigate a more recent issue with one of the core integrations. No time for strolls for them this week.

### Warm Strolls

Dan had a stroll with Robert in the baking heat. With coffee. They talked about [Google on-premises](http://uk.businessinsider.com/google-cloud-available-on-premises-to-take-on-microsoft-amazon-2018-7), amongst other things.

Our Liz took an accidental stroll with Robert, looking for somewhere to eat lunch in the park. It was too hot for strolling, as Robert should really have learned from his stroll with Dan, but neither he or Liz passed out. They talked about decorating cakes.

Samu and Robert talked about the past, present and future of everything. This was an ambitious agenda. They talked in particular about the next steps that they think we should take in building our Search service. What we do know is that it was scorching hot and that the coffee was good. What we don't know is whether strolling was involved during these far-ranging discussions. If it was, Robert has certainly put the miles in this week.


### Things that caught our eye

* Our Liz read about lead and lag indicators, which she found a helpful way of thinking about what we want from the performance indicators we create. Lag indicators being the easier things to measure, they record what happened, but lead indicators proving some input information to understand why the lag indicators change and if those lead activities are having an impact.
* Dan was pointed towards  the [Food Standards Agency](https://www.food.gov.uk/) (FSA) [data strategy](https://www.food.gov.uk/sites/default/files/media/document/datastrategy.pdf).



```

```
