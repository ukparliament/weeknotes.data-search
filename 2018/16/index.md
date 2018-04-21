## 2018 Week 16

### On visions and strategy and things related

No visions were had this week, although both Robert and [Michael](https://twitter.com/fantasticlife) had very odd dreams. Blaming cheese.

### Parliament in the area, [we’re international, we’re continental](https://www.youtube.com/watch?v=pNfHoPIxhXM&t=1m9s)

[Sara](https://twitter.com/sarafreis) and [Matthieu](https://twitter.com/cognithive) left the confines of the [Parliamentary Computational Section](https://pds.blog.parliament.uk/) and took off to Portugal for the rather excellent looking [TICTeC conference](http://tictec.mysociety.org/). They met many interesting people working in the general area of civic tech and [made a friend or two on route](https://twitter.com/LudwigKayser/status/986530728035921920). Matthieu says it was a marvellous opportunity to learn about the international ecosystem of initiatives that exist in the field. And that it's energising and exciting to feel a part of the effort and meet some of the people interested in consuming our data.

Sara also enjoyed the whole thing and [tweeted extensively](https://twitter.com/search?f=tweets&q=sarafreis%20%23tictec&src=typd).

On Tuesday, they went to a seminar organised by the [Information Management School](https://twitter.com/NOVAIMS) and [The Gov Lab](https://twitter.com/TheGovLab) on the topic of open data in government institutions. [Joao Tremoceiro](https://twitter.com/joaotremoceiro) from Lisbon municipality spoke about their issues in dealing with over 300 legacy systems and their project to develop a data platform for intelligent management of the city.

On Friday they participated in a workshop led by [Matt Stempeck](https://twitter.com/mstem) and [Micah Sifry](https://twitter.com/Mlsif) from [Civic Hall](https://civichall.org/) on the the development of a global council to ensure that their [Field Guide to Civic Tech](https://docs.google.com/spreadsheets/d/1FzmvVAKOOFdixCs7oz88cz9g1fFPHDlg0AHgHCwhf4A/edit) properly represents the full range of creative technology and collaboration occurring around the world. They're looking forward to meeting again and seeing that published.

They also introduced our work and the data platform which raised interest in hearing more and sharing experience. A call for show and tell to go international. Or at least continental.

In short, they've come back with too many notes and ideas to share here. But rest assured, there's a blogpost in the making.

### Showing. And indeed telling

This week's show and tell was in the hands of [Chris](https://twitter.com/chrisalcockdev), who talked through some work he's been doing to monitor changes to instance data in source systems. It should give us a more timely and accurate understanding of what's changed as well as notifying parliamentary staff when changes have to be made to other systems.

### Community

[Dan](https://twitter.com/dasbarrett) had 3 opportunities to talk about the data strategy. One at the [Institute for Government](https://www.instituteforgovernment.org.uk/) (nice, says Dan); one with colleagues from the portfolio projects and programmes team (also nice apparently and very receptive); and one with the data steering group. Though the final one didn't quite happen because they ran out of time. Two out of three isn't bad.

On Monday, [Anya](https://twitter.com/bitten_) and Michael headed to the terrace to meet [Stephen Betts](https://twitter.com/stephenbetts) over a bad coffee rather than an average beer. Stephen and Michael were once [future mice](https://twitter.com/futuremice) at the [Big British Castle](https://www.youtube.com/watch?v=_IR4l1FoiIY). Stephen now works at the [NYPL](https://www.nypl.org/) doing stuff that's not entirely disimilar to the data and search team. They talked about data management and models and [SKOS](https://en.wikipedia.org/wiki/Simple_Knowledge_Organization_System) and [FRBR](https://en.wikipedia.org/wiki/Functional_Requirements_for_Bibliographic_Records) and libraries and librarians. And [Tony](https://twitter.com/tonyageh). Then Stephen went off to spend a pleasant couple of hours with Samu, Wojciech and Matthieu.

### One world, one web, one team

Dan, [Jamie](https://twitter.com/oddtype) and [Gavin](https://twitter.com/GavBerman) worked on an approach to data visualisation and decided on a few starting points. All informed by the work of [the other Tony](https://twitter.com/https://twitter.com/psychemedia). Which is as it should be.

### Domain modelling

Tuesday saw yet another meeting where Anya and Michael double (triple? more?) checked the various [Statutory Instrument flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples) with Jane and Jack and James and Jenna. And [Ben](https://twitter.com/benwoodhams). Or Jen, as he likes to be known. There's still some minor tinkering to do but they mostly think they're mostly there. Please god.

They also published a first draft of the [proposed (or baby) SI flow](https://github.com/ukparliament/ontologies/blob/master/procedure/proposed-sis/proposed-sis.pdf) which is about as detailed as they can get until Parliament decides how this will work.

Finally, there's also a first draft of a very basic [legislation model](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html). It will need more work to cope with primary legislation and some gaps between [Statutory Instruments](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e264) and [work packages](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e260) and [Statutory Instruments](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html#d4e264) and [layable things](https://ukparliament.github.io/ontologies/laying/laying-ontology.html#d4e213) still need to be [plugged](https://trello.com/c/2ucuhWhp/81-interface-classes). At least in the physical ontology. But it's all getting there. We think.

### Data platform

The past couple of days have seen some fairly major issues with [data.parliament.uk](http://www.data.parliament.uk/). Wojciech's been working on that and, right now, it looks like it's resolved.

On Monday evening Chris, [Samu](https://twitter.com/langsamu) and Matthieu decided to get competitive and kicked off a race to deploy the latest version of [LODE](http://www.essepuntato.it/lode) on a local service. It took around 30 minutes with some trial and some error. Unfortunately, is wasn't exactly enough as the version they deployed choked on the text/plain turtle files our [GitHub account](https://github.com/ukparliament/ontologies) exposes. [Samu picture redacted here.] To be continued...

And last but not least, our triple store vendor got in touch to say the the mysterious SPARQL bug Matthieu reported last week should be fixed in their next release. Hurrah.

### Corporate data

More in the way of breaking news from the world of corporate data:

[Matt](https://twitter.com/matiasgermanico) had a meeting with the different parties involved in the asset management system integration project. They discussed modifications to the already existing (though not yet deployed) feed of people data. The system owner has received approval from the information security folks to deploy the integrations once a few changes have been made. This will ensure that different types of data (people, organisation structure, cost centres and asset ownership) are updated from the sources in an automatic fashion instead of having them manually updated.

Lewis has continued work on stock system integrations, and started to consolidate some performance reports into raw datasets to enable use by other systems.

Noel performed some testing on the new interface for our Library payment system. He also addressed an issue where some records where not being shown on the system used to monitor people signing in and out using their security pass.

### Was sarcasm deployed?

Sparingly.

### Things that caught our eye

* [Can this robot build an IKEA chair faster than you?](http://www.sciencemag.org/news/2018/04/can-robot-build-ikea-chair-faster-you)
