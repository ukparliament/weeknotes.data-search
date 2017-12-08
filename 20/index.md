## Week 20: 08-12-2017

### International, continental, Leeeeeds

[Anya](https://twitter.com/bitten_), [Ben](https://twitter.com/benwoodhams), [Michael](https://twitter.com/fantasticlife) and [Dan](https://twitter.com/dasbarrett) went to Leeds for the 5th in our continuing series of Parliament, Data and Democracy meetups. In all honesty the turnout was... not great. On the other hand the speakers *were* great and Dan did not have a meltdown. And the conversation was the best yet and the most relevant to the whole 'working with our users' thing.

Thanks to [Cristina](https://twitter.com/estrangeirada), [Nicole](https://twitter.com/mm16nn), [Tom](https://twitter.com/thomasforth) and [Edward](https://twitter.com/edwardwood99). And second thanks to Tom for introducing us to [a very nice pub](https://twitter.com/WhitelocksLeeds).

### Community

Sara gave a [talk](http://www.ucl.ac.uk/medical-image-computing/seminars/mark-graham-sara-ferreira-reis) at her old [research department at UCL](http://www.ucl.ac.uk/medical-image-computing) about what it's like to work in the Parliamentary Digital Service and her experience transitioning from a medical imaging PhD to a data analyst. These seminars are usually very technical and serious, so we think everyone in the audience appreciated the change of topic.

Michael had a meeting with [Paul Seaward](https://twitter.com/pseaward1) at the [History of Parliament Trust](http://historyofparliamentonline.org). Although that was more of a side-project thing. The view was admired. Satsumas were served. Thanks Paul.

### Excellent customer service badges...

...go to Mike for helping some more researchers and students use our data. We had a student working on a dissertation who needed debates on Sexual Offences Acts from 1861-2003 which brought us into the realm of data that predates our systems. We had a source of these called [Historic Hansard](http://hansard.millbanksystems.com/) that has the data but doesn’t have a sophisticated search function. To work around that we leveraged the site: operator that can be used by Google and Bing to allow the user to search the site more easily. We also provided advice concerning some of the arcane parliamentary language. In this case when searching for debates about an act you should refer to the act as a bill as well, as up until the legislation is passed all debates will refer to the bill rather than the act. On a related note - we’ve agreed with our colleagues in the Indexing and Data Management Section of the House of Commons Library to share our communications with external users of Parliamentary data. It’s a great way of us learning some of the business knowledge of IDMS and IDMS getting extra information on how external users search Parliamentary materials.

### data.parliament migration
 
We've made some great progress on the migration of the external [data.parliament](http://www.data.parliament.uk/) components to our new cloud provider. We now have a working copy to start testing with, and hope to have the new version running in parallel with the old version by Christmas. Although the new version will not yet be publicly available. The savings are pretty astounding and we hope to have removed at least one bottleneck in the data flow.

### Corpcomms

Several members of the team posted words to Yammer. It's not yet clear if any trees fell in woods.

#### Who is L Ron Hubbard?

We're not sure but we're beginning to think the poor bloke might be trapped in there.

### One world, one web, one team

On Wednesay, [Matius](https://twitter.com/matiasgermanico) and [Samu](https://twitter.com/langsamu) attended a workshop about enterprise architecture, [CRM](https://en.wikipedia.org/wiki/Customer_relationship_management) and modern data practices.

Samu also met with Jenna and [Jamie](https://twitter.com/oddtype) from the web team. Together they designed the model and process for getting content from our headless CMS into the data platform and onto the website. In the first instance for the Guide to Procedure project. [Chris](https://twitter.com/chrisalcockdev) chipped in later and added valuable insights.

Anya and Michael went along to a meeting with the team working on the Guide to Procedure. A half plan was hatched to bring the navigation of the guide into line with the Parliament Thesauri maintained by IDMS.

### Domain modelling

Anya and Michael made a few changes to the [tabling model](https://ukparliament.github.io/ontologies/tabling/tabling-ontology.html) to cover the tabling of things into a House.

### Data platform

On Wednesday we finally got id.parliament.uk fully working. We are now fully [HTTPRange-14](https://en.wikipedia.org/wiki/HTTPRange-14) compliant. And not many people can say that. Thanks be to Mike.

Matthieu met with Daxa from the End User Team and renewed our key to automatic deployments. He validated our security protocol while he was on the job. It was cool.

### Search

[Raphael](https://twitter.com/raphaelleung) and Robert worked with Callum on search hints. Raphael pushed some edits as requested.

Raphael continued with triple store benchmarking tests and did some research into prior runs of the [Berlin SPARQL benchmark](http://wifo5-03.informatik.uni-mannheim.de/bizer/berlinsparqlbenchmark/). He also looked at other RDF benchmarks and plotted some early results.

Sara and Raphael had a chat about nonparametric significance tests. Not a clue mate.

### Measuring things

At least according to Slack no things got measured. Which is unusual. Maybe we're approaching a more Zen-like acceptance of existence. Or finally learning the lessons of quantum mechanics.

### Corporate data

Matias has been testing the new integration on the HR system. Implementation will happen as soon as we're happy with the testing.

Matias had a meeting with the stakeholders on the asset management integration project. They're now starting to work on testing the chosen data fields and ensuring they meet the requirements. They've also been looking at CostCentre (again not a clue) feeds to check they expose everything needed to build the integration.

Matias has also continued work on generating dashboard reports from JIRA.

There was some other stuff involving words like Cherwell and HardCat but I have no idea how to turn it into English.

### Capability

[Julie](https://twitter.com/julietouring), Selina and [Aidan](https://twitter.com/aidan_morgan) met with Samu and Robert to talk all things Dynamic, Purchasing and Frameworks. They want to capture current and possibly future procurement needs and prioritise.

### Did the machines learn owt?

Perhaps unsurprisingly, no. Like concerned middle-class parents we continue to hold out hope.

### Did anyone say blockchain?

For months there is not a sight of a blockchain. Then 3 come along at once.

Robert was the first person to say blockchain when he slacked a link to [this tweet](https://twitter.com/felix_cohen/status/937685645383864320).

Matthieu followed up with a link to [this story about a digital cats trading game](https://www.technologyreview.com/the-download/609669/ethereums-first-killer-app-is-here-and-its-a-game-where-you-create-digital-cats/) accounting for 12% of transactions on the second largest cryptocurrency network. Which caused a significant backlog of pending transactions. One cat went for more than $114,000. We're sure it's a lovely cat.

On Wednesday night Tom Forth definitely said blockchain, but he was in a pub with a pint in his hand and didn't seem serious.

### Strolls

Many strolls were taken. A strolling venn digram of Anya, Michael, Robert and Dan would probably place Robert at the centre.

### Things that caught our eye

* [Multi-Label Classification with Meta Labels (slides)](https://jmread.github.io/talks/ICDM2014-slides.pdf) [PDF]

* [Multi-Label Classification with Meta Labels](https://users.ics.aalto.fi/jesse/papers/Read,%20Puurula,%20Bifet%20-%20Multi-label%20Classification%20with%20Meta-Labels.pdf) [PDF]

* [Python + TensorFlow implementation of the DropoutNet model](https://github.com/layer6ai-labs/DropoutNet)

* [All That Jazz – Writing and thinking with music](https://500ish.com/all-that-jazz-38969a086bcb)

* [It's Gonna Get a Lot Easier to Break Science Journal Paywalls](https://www.wired.com/story/its-gonna-get-a-lot-easier-to-break-science-journal-paywalls/)

* [A Berkeley View of Systems Challenges for AI](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2017/EECS-2017-159.pdf)

* [Mastering Chess and Shogi by Self-Play with a General Reinforcement Learning Algorithm](https://arxiv.org/abs/1712.01815v1)