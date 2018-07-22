

## 2018 Week 29

Your regular correspondent [Michael](https://twitter.com/fantasticlife) has nipped across the pond this week, resulting in fewer strolls and a strangely empty sofa in the Tothill Street cafe. Meanwhile, the rest of the team struggle bravely on.


### Showing and telling...

At a well-attended Show and Tell, [Matt](https://www.linkedin.com/in/matthew-reed-b3b761105/) and [Sara]((https://twitter.com/sarafreis)) presented their work on "hints" for [search](https://beta.parliament.uk/search) on the parliamentary website. Search hints are used to describe search results. For example, two current hints indicate whether the link is to a [pdf](https://beta.parliament.uk/search?q=pdf), or to a [historic hansard](https://beta.parliament.uk/search?q=oats+rations) page. Picking up on work done by [Raphael](https://github.com/lcyraphael) (formerly of this parish), Sara and Matt analysed a long list of further possible hints. They identified which ones would add the greatest number of hints to the greatest number of results. They've identified a list of 65 hints that describe the content of a result for 98% of all links clicked.

### Community
[Anya](https://twitter.com/bitten_) and Robert went along to [Friends House](https://www.friendshouse.co.uk/) to hear about the [Hansard at Huddersfield](https://twitter.com/hansardhuds) project. Led by a team of linguists at Huddersfield University, and building on the [SAMUELS project](https://www.hansard-corpus.org/x.asp), the new project aims to produce a user-friendly web-based version of Hansard.

[Dan](https://twitter.com/dasbarrett) attended [OneTeamGov Global](https://www.oneteamgov.uk/). He says it was a great day.

### One world, one web, one team

Data analysts and performance analysts spent time talking about measurement. As is their wont. They also considered the kinds of information about the website that could be used to create indicators. Our Liz says the conversations were really useful. She notes that it's challenging to think about measures that reflect the whole website, and not just part of it.

[Alison](https://twitter.com/oliala) took product managers and Liz, [Steve](https://twitter.com/Steve_Bromley) and Trine through a modelling session on product measurement. Liz says the session helped identify an overlap between needs and goals. They all thought it was particularly useful to understand this point. Liz enjoyed it (thank you Alison). Next up is a session involving data and performance analysts, expanding on measurement and indicators.

[Matt Rayner](https://twitter.com/mattrayner) gave a presentation on the architecture of the website to [Samu](https://twitter.com/langsamu), [Matthieu](https://twitter.com/cognithive) and [Jianhan](https://twitter.com/jianhanzhu).  [Usman](https://twitter.com/_UsmanAfzal) joined them for conversations about componentization, markup optimisation, presentation APIs and future development. Matthieu found the whole thing delightful.

Alison, Matthieu and Wojciech went along to the first of [Dan](https://twitter.com/dasbarrett)'s weekly open sessions on the Data strategy. They discussed the merits of high level principles for managing Parliament's data. It felt like really good organisational groundwork.

Liz and Matthieu prepared for the technical interviews for a data analyst post. They interviewed four candidates, and are looking forward to working with the successful interviewee. Meanwhile, [Julie](https://twitter.com/julietouring) and Liz are hatching plans for a workshop on developing career paths for roles involving data analysis.

### Domain modelling

Alison delved into world of [parliamentary committees](https://www.parliament.uk/business/committees/). Parliament has many committees. And things called committees that aren't committees. And things that aren't called committees but are in fact committees. Alison's challenge is to discover whether procedures that relate to committees can be represented using our [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html). Gail, Ed and James helped to shed some light; there will no doubt be many more sessions to follow.

Not content with this challenge, Alison is also exploring how well our [document model](https://ukparliament.github.io/ontologies/document/document-ontology.html) holds up against committee reports. Much model, many committee.

### Data platform

Matthieu built a dashboard to analyse the API use of the [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri). Building something to sample the 7 milion requests took some serious PowerBI modelling and a lot of patience. Finding the team workstations to be somewhat workshy, Matthieu drifted into dreaming of a "bring your own laptop to work" scheme. We hope he wakes up soon.

[Jianhan](https://twitter.com/jianhanzhu) helped Bryony with constructing [SPARQL](https://en.wikipedia.org/wiki/SPARQL) queries. Their queries will be used to power features for [written questions](https://www.parliament.uk/site-information/glossary/written-questions/) on the [beta website](https://beta.parliament.uk/).


### On search. And indeed indexing

Matt has been analysing the performance of the internal and [external](search-material.parliament.uk) versions of Parliamentary Search. He explored how filters are being used and produced some very colourful graphs to summarise his findings. Matt notes that the internal facing version of these search services is used about 15 times more often than the external version.

[Alex](https://twitter.com/AlexEdwardH) undertook some bulk correction for Parliamentary Search, to fix records missing data such as Department IDs. The only way to find the affected records is by partial string matching. This is easy in Apache Solr but not so much in the triplestore where the data needs to be inserted. Alex wrote some Powershell scripts that allows bulk editing of data based only on given Solr search results by exporting URIs from Solr and sending POST requests to the Triplestore.

### Corporate data

The entire team has been hard at work resolving an issue with BizTalk and its interfaces with People Data. Unfortunately records are not being updated automatically. Investigations are continuing. Lewis has been looking into BizTalk maintenance issues and how the team can improve their monitoring of BizTalk.


### Strolls

No strolls have been reported this week. We think this is probably because Michael hasn't been around. He's in America (or the US as he calls it) working on becoming an American.

Regular readers will know that Michael takes strolling seriously, and despite being on holiday (or vacation as he calls it) he did attempt a stroll. Through Salem. Where the witches were. (Though they weren't really witches we're told.) Before setting off he went to grab some stuff from the boot, or trunk as he would say, of the car. What Michael didn't realise is that American cars have a thing that makes them open when you stand next to them with the keys. Michael admits that he doesn't know much about cars. He checked if the car was locked. And it was unlocked. Because the key was in his hand. This happened several times before he gave up. He tried shouting, which is possibly the first time anyone's shouted in Salem since 1692. No one heard. No one noticed he was missing. So he ended up sitting on the pavement for an hour and getting told off for smoking. Luckily, [American cars can send texts](https://twitter.com/fantasticlife/status/1020679971109470209). So people were alerted to his predicament. And the predicament of the massive American car.


### Things that caught our ear

* Matthieu listened to [a guy interviewing a can of cola](https://99percentinvisible.org/episode/everything-is-alive/). He liked it.








































```

```
