## Week 11: 06-10-2017

### Community

[Dan](https://twitter.com/dasbarrett) and Robert went to [City Hall](https://en.wikipedia.org/wiki/City_Hall,_London) for a search chat with colleagues from the [GLA](https://www.london.gov.uk/). It was a good meeting, with plenty of potential for future collaboration and maybe even a loose community of practice. Robert left with the feeling that what we're doing isn't so mad after all. It also prompted him to start working out what we should be measuring as search moves onto the beta. 

Wojciech and Mike met up with [Dan Leedham](https://twitter.com/danleedham) from [Bowtie Productions](http://www.bowtietv.com/) who has been putting together an app using the Members Name Information System, data.parliament, and the new data platform. His app, among other things, allows people to search for members by department, committee, name or position. It then displays historical information about the member’s positions and incumbencies. Dan’s app also makes great use of our photo API. It was very useful finding out some of the things which have worked well. He particularly liked being able to specify the aspect ratios of photos when calling the API, and was excited about the work we’ve been doing to accurately link Parliamentary data. We look forward to seeing more great work like this develop as the new data platform grows.

### One world, one web, one team

Aidan and Dan continued to take it in turns to attend website [stand ups](https://www.youtube.com/watch?v=fgXqDmhECxc) though Dan only managed to make one this week. Because circumstances. He did go to a website backlog review session though, and then sat in on a really great session on ideas to improve the pages based on feedback from user testing.

Aidan went to more website stand ups than Dan across both the 'members' and 'committees' teams.

### Domain modelling

[Anya](https://twitter.com/bitten_) and [Michael](https://twitter.com/fantasticlife) spent most of Wednesday sketching [domain model stuff around written questions and answers](https://github.com/ukparliament/domain-models/blob/master/Written%20questions/written-questions.pdf). The usual questions of cardinality came up. Is a question sent to many answering bodies one question or many? Can a question have multiple answers from the same body (holding answer, actual answers, corrections) and from different bodies? Can an answer respond to several questions (it can) and how does the current data model cope with this (it doesn't)? A general feeling there is wasted work here and we could do better.

They also spent some time adding first draft comments to the [event ontology](https://ukparliament.github.io/ontologies/event/event-ontology.html). Feedback, as ever, more than welcome.

Anya, [Silver](https://twitter.com/silveroliver) and Michael were interviewed by [Susan Halford](https://twitter.com/susanjhalford) and [Mark Weal](https://twitter.com/mark_weal) from the [Web Science Institute](https://www.southampton.ac.uk/wsi/index.page) who are conducting research into the 'Everyday Practices of Semantic Linked Data'. We talked about our approach to domain modelling and ontology development. Michael had a rant. It was cathartic.

### Data quality

Aidan, Wojciech, [Chris](https://twitter.com/chrisalcockdev) and Michael spent Tuesday at the Ordnance Survey discussing constituency data. There were three main things discussed:

* Missing links between some constituencies and the [NUTS regions](https://en.wikipedia.org/wiki/NUTS_statistical_regions_of_the_United_Kingdom) they're contained in. This is now being fixed.

* Lack of postcode data for Northern Ireland. We still have a problem here since none of the OS datasets containing Northern Ireland postcodes are available as APIs. This lead to an interesting discussion about data dumps vs APIs in the context of licencing. That if we can directly use OS APIs we won't have to store the data in our platform. If we rely on data dumps we would have to store the data which would mean we'd need to partition the store to only expose data with an [Open Parliament Licence](https://www.parliament.uk/site-information/copyright-parliament/open-parliament-licence/).

* Postcodes that span more than one constituency (occasionally referred to here as 'grey zones'), a problem very well described in this [post by Sym](https://democracyclub.org.uk/blog/2017/03/20/4314-times-when-postcodes-arent-good-enough/). The OS has done some analysis and found that of the 1.7 million postcodes, about 24,000 span more than one parliamentary constituency. Restricting that to addresses classified in [AddressBase Plus](https://www.ordnancesurvey.co.uk/business-and-government/products/addressbase-products.html) as residential, excluding non-postal addresses, and including only those addresses derived from [PAF](http://www.royalmail.com/business/services/marketing/data-optimisation/paf), reduces that to around 5600 postcodes out of 1.48 million current residential postcodes (0.38%). For this set of 5600 postcodes there are around 96,000 residential addresses (0.36% of 26 million residential addresses). We also found, out of the postcodes which span parliamentary constituencies, 72,000 individual addresses fall into the same parliamentary constituency as the codepoint for their postcode. And 24,000 don't. Just less than 0.1% of all residential addresses.

Discussions continue on how we might join the [Public Sector Mapping Agreement](https://www.ordnancesurvey.co.uk/business-and-government/public-sector/mapping-agreements/public-sector-mapping-agreement.html).

### Data platform

Chris fixed the incumbency naming clash allowing us to progress with modelling various jobs in the physical ontology. This includes the first set of goals for Government (ministerial) Positions.

Aidan completed the procurement of the licence for the triple store.

Dan and Aidan met with Steve Wise from the House of Commons Library to discuss the data toolkit and project funding.

### Search

Robert drowned in a sea of admin-esoterica this week. Monday was a revisiting of the contributions of product and delivery management to the search work, some updates on Archives requirements, learning more about search feedback and analysis. 

[Raphael](https://twitter.com/raphaelleung) showed Robert the search ‘hints’ work to decorate search results with document types. This was great.

### Capability

Robert went along to a really quite animated meeting and discussion with Julie’s capability group.

### Did anybody say blockchain?

Samu came closest to saying blockchain when he slacked a link to an article about [turning electricity into money](https://spectrum.ieee.org/computing/networks/why-the-biggest-bitcoin-mines-are-in-china). He made a dextrous dive to his right and pulled off an audacious save just before the ball crossed the line. Well done Samu.

### Strolls

Dan and Robert took a stroll along the river from the GLA back to Parliament. They stopped for a coffee in Borough Market. It was all very civilised.

Robert and Michael went for a chilly walk through Westminster. The note from Robert says he listened to Michael talking but Michael's sure he shut up at some point. They did not stop for coffee but it was still civilised.

### Things that caught our eye

* [Who gets held accountable when a facial recognition algorithm fails?](https://medium.com/@ellenbroad/who-do-we-hold-accountable-when-facial-recognition-algorithms-fail-47feba3aae92)

* [Forget Killer Robots—Bias Is the Real AI Danger](https://www.technologyreview.com/s/608986/forget-killer-robotsbias-is-the-real-ai-danger/)

* [Koch snowflake](https://en.wikipedia.org/wiki/Koch_snowflake#/media/File:Kochsim.gif)