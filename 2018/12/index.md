## 2018 Week 12

### Parliament in the area, [we’re international, we’re continental](https://www.youtube.com/watch?v=pNfHoPIxhXM&t=1m9s)

[Dan](https://twitter.com/dasbarratt) met with a delegation from the [Namibian Parliament](http://www.parliament.na/index.php?option=com_content&view=featured&Itemid=435). He realised he'd been droning on about our website and our data service for a little too long, so they went through the Namibian website instead. There was a good conversation about their users and why they want to make laws more accessible. Dan really liked the [legal database](https://laws.parliament.na/about-us/) they showed.

There was also a good discussion about search with Dan mostly channeling Robert. Where are the people are (not on your website) and what do they expect (to find things) is a fairly easy sell.

### Community

Dan also went along to [ACAS](http://www.acas.org.uk/index.aspx?articleid=1461). Fortunately not because of an industrial dispute, but because they asked him to come and talk to them about data. Which is nice. It was a good 'lunch and learn' session, which was mostly Dan talking about the data and search journey and what we have been doing and why and what's next. He also showed the things. Like the website. And the search. And the ubiquitous 'omelette diagram' without which no talk would be complete. The feedback was good, it was really nice to talk to a receptive audience, and Dan learned a bit too.

[Anya](https://twitter.com/bitten_), [Ben](https://twitter.com/benwoodhams) and [Michael](https://twitter.com/fantasticlife) went along to an [Open Government Partnership](https://www.opengovpartnership.org/) event in the offices of the Speaker, hosted by [Ben Worthy](https://twitter.com/benworthy). It was an interesting excursion to an interesting place with interesting set of questions. And the Speaker turned up. So at least one of our speakers is not missing....

### Domain modelling

Anya and Michael continued working on the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html) which they're now feeling pretty pleased with. They had a brief but pleasant chat with Samu and Raphael which ironed out some of the misunderstandings. [Samu](https://twitter.com/langsamu) pointed out the canSpawnMultiple property was redundant which pleased Anya, who'd always objected to the word 'spawn'. So that's gone now.

Anya added details of the [made affirmative Statutory Instrument procedure](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/affirmative-made.pdf) to the [procedure application](https://procedures.azurewebsites.net/Procedures/3) that Wojciech and Raphael have been building. Both versions of affirmative procedure have now been signed off by Jane from the Lords and Jack from the Commons. We're still waiting on sign off of the negative flows. But it all feels like progress.

### One world, one web, one team

Michael went along to assorted sessions run by the website team working on [Statutory Instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)). There was some kind of 'mood board' session in which he scribbled out some URLs. As is his wont. Though he did get in the spirit and draw some web pages. [Ever so slightly grudgingly](http://smethur.st/posts/176135864).

### Data platform

Team:Samu worked with a variety of other people to finally get Peers' Portraits onto the beta website. You can [see one such portrait here](https://beta.parliament.uk/people/S70cUJGM). There were a variety of last minute snaggles getting House of Lords data into a suitable shape to support the pages to host the images. [Jianhan](https://twitter.com/jianhanzhu) went with the word 'saga' and only a slightly_smiling_face. Matthieu says the final release went fairly smoothly though communication around "go live" time could have been improved. If we'd known in advance, we could have pre-warmed the cache to cope better with demand. But we didn't. So there were some initial complaints about slow responses times but we quickly scaled up our computing, crawled the pictures to warm the cache and response times instantly dropped. The infrastructure is solid and we got there. Top work all.

Back when we released portraits of Members of the House of Commons, [Giuseppe](https://twitter.com/puntofisso) managed to grab them and [calculate the average face of an MP](https://medium.com/@puntofisso/i-calculated-the-average-face-of-a-uk-member-of-parliament-and-heres-what-i-found-37f31b72b5d9). This time around the grabbing was made easier and he managed to use our new data service to get the photos and calculate the [average face of a Peer](https://twitter.com/puntofisso/status/976424407043276802). So that's progress.

Jianhan wondered what the average face in the Parliamentary Computational Service would like. No one's gone there yet.

### Parliamentary search

[Alex](https://twitter.com/alexedwardh) added a new action to the automated [search](http://search-material.parliament.uk/) tests. It now checks for errors with government department terms caused by missing [rdfs:seeAlso](https://www.w3.org/TR/rdf-schema/#ch_seealso) statements in the search and indexing triplestore. These are supposed to link a concept in [the thesauri](http://www.data.parliament.uk/dataset/thesauri) to a matching department in the Members' Names Information Service in a [foaf:focus](http://xmlns.com/foaf/spec/#term_focus) type fashion.

### Corporate data

In the fast moving world of corporate data, work continued on integrating the stock system with the finance system. Lewis continued with development and did some code refactoring and troubleshooting on one of our internal web services. Meanwhile, Matt and Noel investigated an issue in our service desk software that was causing calls to be created multiple times. Noel also continued to review the data held in People Directory.

Dan has instituted a new catch up with [Mat](https://twitter.com/matiasgermanico), Lew, Noel and David. The intention is to meet at 4pm everyday but so far it's looking more like 3 days in 5. Dan thinks it's been pretty good so far. The main thing on his mind is how we move to a better software environment for data integration work.

Dan's also been working with [Toyin](https://uk.linkedin.com/in/toyinsowunmi), the data architect on people data, who's joined us for a short while to help kick off work to improve our corporate data.

### Capability

Dan had a call with the recruitment consultant about the [data analyst job](https://www.parliament.uk/about/working/jobs/pds-job-homepage/data-analyst/) we're currently advertising (great job; crazy URL). He thought the call went well and he's getting better at explaining the team and why, all told, it's really pretty good.

### Did any of our speakers go missing?

Unfortunately yes. To support the work around the release of Peers' portraits we had an assortment of jobs to tidy some of the Peers' pages. It was noticed that the [Lord Speaker](http://www.parliament.uk/business/lords/lord-speaker/)'s page did not include any indication that [Lord Fowler](https://beta.parliament.uk/people/R3ZEnpii) is the current incumbent of that position, because we haven't yet got round to modelling parliamentary positions.

Again unfortunately, it was also noticed that someone at some point in the past had added [a party called Speaker](https://beta.parliament.uk/parties/LfB2y7qm/members/current) to cope with a similar issue for the Speaker of the House of Commons. To cut a long story short a new [Lord Speaker party](https://beta.parliament.uk/parties/lb1kpPXc/members/current) was added to the Members' Names Information Service. And for want of a nail the shoe was lost.

The new 'party' caused a cascade of unintended consequences in downstream systems. Lord Fowler's membership was back dated to September 2016, meaning the Indexing and Data Management Section of the House of Commons Library had to reindex all his contributions back to that point. Except they couldn't because all the details necessary to expose the 'party' in the MNIS API had not been entered though this oversight was not flagged. On adding the missing details, something went wrong and for a short while all the Conservative members of the House of Lords became the Lord Speaker. He also disappeared off the Lords' attendance system which made it more difficult that you'd like to pay his expenses.

There are probably lessons here and the words data and governance have been used.

### Customer service of the week award...

...goes to [Chris](https://twitter.com/chrisalcockdev) for helping Giuseppe to use our data service to grab Peers' portraits. Applause.

### Things that caught our eye

* [What does the Cambridge Analytica scandal mean for access to data?](https://theodi.org/article/what-does-the-cambridge-analytica-scandal-mean-for-access-to-data)

* [A user manual for our Dan](https://medium.com/@dasbarrett/a-user-manual-for-dan-d0a285874f72)

* [Putting users first is not the answer to everything](https://medium.com/doteveryone/putting-users-first-is-not-the-answer-to-everything-dd05b9f11b5?source=linkShare-4cd140afefc2-1521803035)

* [A history of IP in computer programming: Navitaire Inc v Easyjet Airline Co & Another](http://www.5rb.com/case/navitaire-inc-v-easyjet-airline-co-another/)