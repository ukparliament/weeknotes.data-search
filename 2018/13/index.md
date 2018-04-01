## 2018 Week 13

### Parliament in the area, [we’re international, we’re continental](https://www.youtube.com/watch?v=pNfHoPIxhXM&t=1m9s)

On Tuesday, [Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) had arranged for [Tony Ageh](https://twitter.com/tonyageh) to give a talk to assorted folks from the House of Commons Library and the Parliamentary Computational Section. Tony has travelled through much of the British media and now works as the Chief Digital Officer for the [New York Public Library](https://www.nypl.org/).

He gave a great talk on what it means to be a library in the early years of the 21st Century, touching on issues around trust, consent and privacy, and making the point that many of the tools supplied to us by the Silicon Valley giants incentivise commercial gain rather than public values. Applause.

On Thursday, Anya, [Silver](https://twitter.com/silveroliver) and Michael met with Ciaran Doyle who's the Head of IT at the [Houses of the Oireachtas](http://www.oireachtas.ie/parliament/). They went back over the [slides they wrote for the Euro IA conference](https://docs.google.com/presentation/d/1bQnE8elOkTPmyGP4Wei4YNobExeiS_gQLoI_sMSFEWs/edit), whilst repeatedly and tediously making the point that *if your data doesn't link, your website won't link*. And nobody wants a unlinked website.

### Community

Michael stood in for Anya at a meeting of assorted civil servants, parliamentary clerks and [National Archives People](http://www.nationalarchives.gov.uk/). The main topic was proposals for [pre-legislative scrutiny of secondary legislation](https://www.parliament.uk/business/committees/committees-a-z/commons-select/procedure-committee/news-parliament-2017/exiting-eu-scrutiny-delegated-legislation-interim-report-published-17-19/) as a result of Brexit. Rather than laying [Statutory Instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) directly into Parliament, it's possible that a preliminary paper (henceforth known as a baby SI) will be laid first and sent to sifting committees in both Houses. Anya and Michael have added 'baby SI' procedure flow to their [to do list](https://trello.com/b/Z1nrm0Vr/parliament-ontology).

### Domain modelling

Anya and Michael went back over the [assorted Statutory Instrument procedure flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples) following feedback from Jane (House of Lords) and Jack (House of Commons). They've now updated the [made affirmative SI procedure](https://procedures.azurewebsites.net/Procedures/3) in the application Wojciech, Raphael and Chris have been building. Raphael has started to add [graph visualisations to work package pages](https://procedures.azurewebsites.net/WorkPackages/5/graph) to show completed steps and what might happen next. Which is all pretty cool.

Anya, Silver and Michael had a meeting with Gail Barlett from the House of Commons Public Bill Office to try to figure out what bill amendments have in common with motions and motion amendments. It felt like there was some commonality but the [sketch so far](https://github.com/ukparliament/ontologies/blob/master/motion-amendment/motion-amendment.png) might be pushing it. Michael is still confused about what an [Early Day Motion](https://www.parliament.uk/site-information/glossary/early-day-motions/) might be. Ontologically speaking.

There was also an Anya, Silver, Michael meeting with [Samu](https://twitter.com/langsamu) to talk about introducing logic gates to the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html), allowing for multiple conditions having to be met before the next step gets triggered. Conversations got as far as implementing the whole thing as logic gates and printing procedure at chip level before they steered back and decided logic gates might be a complication too far. But they did settle on adding a new [route type](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e222) of something like 'requires' to specify which preceding steps must be complete to trigger the next step. Which feels a neat solution.

Samu also showed some 3D plots of procedure models he's been playing with. Next step is to print them and hang them from office ceilings mobile style.

### One world, one web, one team

[Dan](https://twitter.com/dasbarrett) and Michael (and Anya for the first one) had a good couple of sessions with the 'People' website product team looking at their plans for what's next and how this turns into work for Data and Search.

[Sara](https://twitter.com/sarafreis90) and [Alex](https://twitter.com/alexedwardh) gave a great show and tell about the work they've been doing to analyse indexing work for the Indexing and Data Management Section of the House of Commons Library. And how they're automating some of the tasks previously performed by [Phil](https://twitter.com/philbgorman) before he left for newer pastures.

### Did any of our speakers go missing?

Neither of our speakers went missing this week, although we still have way too many parties.

### Customer service of the week award...

...goes to [Chris](https://twitter.com/chrisalcockdev) who cobbled together a query for a customer in a couple of hours. [Steve](https://twitter.com/stevejgoodrich) (a friend of this parish) had been trying to use [data.parliament](http://www.data.parliament.uk/) to get a list of Members who hold or have held government positions. He'd got in touch with Michael when the API he was using didn't return a reasonable number of results. Being forever baffled by data.parliament, Michael passed on the question to Chris who wrote [a query on the new data platform](https://api.parliament.uk/query/government_position_index) in double quick time. Steve got back to say we'd saved him hours of pain. Top work Chris.

### Things that caught our eye

* [Three years of Visual.ONS – what we’ve learned](https://digitalblog.ons.gov.uk/2018/03/27/three-years-of-visual-ons-what-weve-learned/)

* [Open APIs in the Telecoms Industry](https://openapis.projectsbyif.com/)

* [Our Sara on what it's like to work as a data analyst in the Parliamentary Computational Section](https://pds.blog.parliament.uk/2018/03/28/being-a-data-analyst-in-pds/)