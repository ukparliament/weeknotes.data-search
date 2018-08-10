## 2018 Week 32

### Is there anybody out there?

It's [summer recess](https://www.parliament.uk/business/news/2018/july/house-of-commons-rises-for-summer-recess-2018/) time at Parliament which means lots of people took off on holidays just as the rains came. So we're quieter than normal. And have less to report. Nevertheless, for the sake of completeness, if nothing else, these are our notes from the week.

### Is [Samu](https://twitter.com/langsamu) morality?

Yup. We're expecting little change here.

### Community

[Michael](https://twitter.com/fantasticlife) met [Paul](https://twitter.com/psd) for a pint and a chummer about users and their needs and how designing for a [complex community](https://twitter.com/fantasticlife/status/1009802788145188865) of users with off stage, unmeasurable and unknowable communication channels is different to making iPlayer. Or Spotify. Or [gov.uk](https://www.gov.uk/). Michael is still threatening a blog post. When he pulls his finger out.

### Showing and telling

This week [Matt](https://twitter.com/mattrayner) [took to the stage](https://www.youtube.com/watch?v=rgEw_YtfxYM) and promptly showed and told some of the work he's been doing (with Christine and Allan) on the new website application. Matt being Matt he chose to go with a whiteboard rather than a projector. Having talked through some of the problems we've found with our current application framework (implementation inconsistencies and developer hostility) he talked through the new approach which we're hoping will bring the website into closer alignment with the data model. 

For those with an interest in such things we're building a new back-end framework called [Thorney](https://github.com/ukparliament/thorney), built on [Rails](https://rubyonrails.org/) and a new front-end framework called [Augustus](https://github.com/ukparliament/augustus), built on top of [Shunter](https://github.com/springernature/shunter), built on top of [Node](https://nodejs.org/en/). Almost makes you pine for FTP.

Having assembled these assorted onion layers we're hoping [search](https://beta.parliament.uk/search) will be the first piece of the jigsaw to get refactored. Stay tuned.

### One world, one web, one team

Daniel and Joe from the [House of Commons Scrutiny Unit](https://www.parliament.uk/mps-lords-and-offices/offices/commons/scrutinyunit/), have started using the data from the ways of working dashboard to do some analysis. Our Liz is planning to share some of the structuring work she did on the data, so they don't have to re-create it all. Hopefully they'll be able to do what they need to do a little more quickly.

[Alison](https://twitter.com/oliala) met with both [Jamie](https://twitter.com/oddtype) and Michael to begin plotting out URLs for our forthcoming visit Parliament pages.

Michael met [Sarah](https://twitter.com/SarahPurssell), [James](https://twitter.com/thevinternet) and [Victor](https://twitter.com/_victorhwang) to chat about the [committee evidence submission model](https://ukparliament.github.io/ontologies/submission/submission-ontology.html) and look through some of their wireframes. Most things seem to match up but there's a lack of reference data here and some fuzziness around how we reconcile people and organisations submitting evidence. Use cases exist for tracking this but as yet we're not quite sure how we meet them.

[Jianhan](https://twitter.com/jianhanzhu) worked with Jamie to get 53 MP and Peer reshoot photos onto the [beta website](https://beta.parliament.uk/). [Creative Commons licenced](https://creativecommons.org/licenses/by/3.0/) as ever. Please continue to fill your boots.

Michael went along to a session on service design but left no less confused than when he arrived. Which is not unusual. He can be quite dim.

### Did Mike discriminate?

No way. He's a sweet lad.

### Domain modelling

Alison had another session with [Fred](https://twitter.com/_mcghief), House of Lords Ed and House of Commons James, diving into [committee reports](https://www.parliament.uk/business/publications/committees/select-committee-publications/) and identifying bits that are authored specially for the report and bits that are outputs of prior committee business. The [committee report domain model](https://github.com/ukparliament/domain-models/blob/master/Committee%20Report/Committee%20Report.pdf) has been updated accordingly.

Michael poked [Tony](https://twitter.com/psychemedia) about similar matters. It still feels there's something [Jupyter Notebook](http://jupyter.org/) like here, with reports (and [library briefings](https://researchbriefings.parliament.uk/)) being an ordered set of decorated [transclusions](https://en.wikipedia.org/wiki/Transclusion). Building an example committee report, transcluding as much as possible would be an interesting experiment.

### Data platform

Work continued on enhancements to the [Statutory Instrument tracker](https://beta.parliament.uk/statutory-instruments) service. [Matthieu](https://twitter.com/cognithive)'s been slaving away to bring the [legislation](https://ukparliament.github.io/ontologies/legislation/legislation-ontology.html) and [laying](https://ukparliament.github.io/ontologies/laying/laying-ontology.html) models into the data platform. Wojciech battled the machines to make a better Procedure Editor for the Indexing and Data Management Section in the House of Commons Library. And Jianhan worked on extracting  SI data from the Solr index and saving it into the Procedure Editor database, which reduces the burden of duplicate data entry for IDMS.

Mike and Michael spent a pleasant afternoon (or the best part of one) picking through assorted [SI flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples) and comparing them to the [swanky visualisatons of actual data](https://procedures.azurewebsites.net/) in actual machines. They ran through a spreadsheet [Anya](https://twitter.com/bitten_) had provided and used the Procedure Editor to make the changes. They also noticed a few other discrepancies. Which they fixed. Or believe they fixed. Next week they plan to sit on a floor with Anya and Jayne, surround themselves with scraps of paper and check things.

In updating the procedure data they stumbled across a few bugs with the Procedure Editor. Form [inputs in one section being accidentally linked to labels in another section](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label) not least of them. Heads were scratched and computers cursed. On top of that, [cache control headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control) were not being set, so views were getting cached in the browser. If you deleted a thing, you got taken back to a list with the deleted thing still on it. Confusion was not lessened by the use of [soft deletes](https://stackoverflow.com/questions/2549839/are-soft-deletes-a-good-idea). If you tried to delete the same thing again the computer just said, yup, deleted. And took you back to look at it.

Luckily, Mike and Michael were sat just behind Wojciech who could not help but overhear their anguish, and jumped in with fixes to the usual tune of [Sheiße](https://www.urbandictionary.com/define.php?term=sheisse).

In the unlikely event you're reading this, the even more unlikely event you have an interest in UK secondary legislation and the vanishingly small chance you want to help, spending some minutes checking our hand-drawn flowcharts against their machine drawn counterparts would be lovely:

#### Draft negative procedure

[Hand drawn](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/draft-negative.pdf) vs [Machine drawn](https://procedures.azurewebsites.net/Procedures/5/graph)

#### Made negative procedure

[Hand drawn](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/made-negative.pdf) vs [Machine drawn](https://procedures.azurewebsites.net/Procedures/4/graph)

#### Draft affirmative procedure

[Hand drawn](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/draft-affirmative.pdf) vs [Machine drawn](https://procedures.azurewebsites.net/Procedures/3/graph)

#### Made affirmative procedure

[Hand drawn](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/made-affirmative.pdf) vs [Machine drawn](https://procedures.azurewebsites.net/Procedures/1/graph)

#### Proposed negative statutory instrument procedure

[Hand drawn](https://github.com/ukparliament/ontologies/blob/master/procedure/proposed-negative-sis/proposed-negative-sis.pdf) vs [Machine drawn](https://procedures.azurewebsites.net/Procedures/2/graph)

[Feedback](mailto:smethurstm@parliament.uk), as ever, more than welcome.

### On search. And indeed indexing

Mike called upon the expertise of Samu and Wojciech to write a script to update the subject tagging of [Early Day Motions](https://en.wikipedia.org/wiki/Early_day_motion). They had been indexed with the somewhat limited website taxonomy but those indexings have now been updated to point to [Concepts](https://www.w3.org/2009/08/skos-reference/skos.html#Concept) in the much more expressive [Thesauri](http://www.data.parliament.uk/dataset/thesauri). Given we have around 45k EDMs in the system this was quite a big bit of work. The script runs 311 sequential [SPARQL](https://en.wikipedia.org/wiki/SPARQL) updates to change the Concept IDs in the Search and Indexing triple store and push the updates to [Solr](http://lucene.apache.org/solr/) for the purposes of [parliamentary search](http://search-material.parliament.uk/).

### Measuring things

Our Liz reports that Naz has now finished adding [AppInsight](https://www.appdirect.com/products/appinsights) code onto more of the website. Which means we can now see things like the traffic for this [map search](http://archivesmapsearch.labs.parliament.uk/mapsearch). 

### Corporate data

Flames died down on the burning platform that is [BizTalk](https://en.wikipedia.org/wiki/Microsoft_BizTalk_Server) though it continued to smoulder. Other than that I'm not exactly sure what happened in the fast moving world of corporate data. Because nobody told me. If you know, do shout.

### Strolls

So for the past few weeks it's been too damned hot to put the required effort into strolling. And now it's too bloody wet. It's rubbish being British.

Despite inclement circumstances, Robert and Michael did manage to fit in a stroll to Victoria. Where they talked about "products" and users and their never-ending neediness.

Alison also snuck in an impromptu and somewhat sedentary chat with Robert. Many things were discussed, not least search, communication channels and the [4-dog dog walking limit in Wandsworth](http://www.wandsworth.gov.uk/info/200512/dog_control_and_animal_welfare/349/dog_control).

### Things that caught our eye

* [The top data structures you should know for your next coding interview](https://medium.freecodecamp.org/the-top-data-structures-you-should-know-for-your-next-coding-interview-36af0831f5e3)