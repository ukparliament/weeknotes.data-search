## 2018 Week 08

### Community

[Dan](https://twitter.com/dasbarret) went along to the [Institute for Government](https://www.instituteforgovernment.org.uk/) for a 'round table' about Parliamentary data. He felt pretty useful and, unusually, was listened to.

Raphael went to a workshop on explainable AI, data use and consent at Loughborough University. He thought it was well organised and relevant to our work.

### One world, one web, one team

Show and tell was much improved from last week when [Michael](https://twitter.com/fantasticlife) forgot to turn up. This week his memory was much improved so he went along and showed the work he's been doing with [Anya](https://twitter.com/bitten_), [Ben](https://twitter.com/benwoodhams) and [Silver](https://twitter.com/silveroliver) on written parliamentary questions and answers. It seemed to go OK and was well attended. Tim Barnes, the project manager, came bearing a message from Business Systems about their new API for questions. [Jianhan](https://twitter.com/jianhanzhu) went away and spent a bit of time looking at this API and had [some questions around oral answers](https://twitter.com/jianhanzhu/status/966628080113586176).

On Thursday we had a joint website / data and search / business systems / library session about [Statutory Instruments](http://www.parliament.uk/business/bills-and-legislation/secondary-legislation/statutory-instruments/). It was pretty good, all told. There we actual decisions. An acknowledgement of work already done. And some more work still to be done.

Anya and Michael met with the website team working on statutory instruments to talk them through their work so far. There's a general feeling that the bit that's seen as hard (process flow) isn't that hard, and the bit that's seen as easy (all the actual business) is about as hard as modelling the whole of Parliament.

[Samu](https://twitter.com/langsamu)'s introduced some further automation into the way we collaborate with other teams on the code for the queries that run the website. Pull requests from our public, read-only source control repository now automatically create branches in our internal repo, so it's easier and quicker for us to review and approve them.

### Domain modelling

Anya, Silver and Michael continued to work on a fairly abstract model for templating parliamentary procedure. Or process. They can't quite decide which. They're aiming to create something that can be populated with instance data to describe assorted bits of parliamentary procedure flow. So far they've [made a thing](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html) that feels generally right but not specifically right. Work continues.

Anya and Michael met with Gini Griffin and Kevin Gardner from the House of Commons Table Office to talk about [Early Day Motions](http://www.parliament.uk/site-information/glossary/early-day-motions/) and whether some of the modelling they had in mind was more widely applicable to tabled motions and motion amendments in general. It turned out it was, so that saves some work.

On Thursday Anya, Ben and Michael met with Heather Wood and Thomas Balloch. They're the people who look after the [House of Commons Register of Members' Financial Interests](https://www.parliament.uk/mps-lords-and-offices/standards-and-financial-interests/parliamentary-commissioner-for-standards/registers-of-interests/register-of-members-financial-interests/). They talked about process flows and data input and some of the potential benefits of adding more structure.

[Jamie](https://twitter.com/oddtype) and Samu had a second session dedicated to designing a model for content collections, taking into consideration user experience, editorial and technical requirements.

### Data platform

Wojciech and Samu have added [HSTS](https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security) to our new APIs.
The HSTS protocol improves security for users by instructing their browser to only use a secure channel for talking to the service. They've also made changes to ensure that the data service can only ever be accessed over HTTPS, as well as disabling some older security protocols.

[Chris](https://twitter.com/chrisalcockdev) and Samu added isDefinedBy to the ontology to better link together the ontology, its classes and its properties. We hope it helps people looking at it in various contexts to understand it better.

Samu also added unit tests to the ontology project to make sure that we follow our own conventions. Samu notes that Chris has followed them almost perfectly anyway.

Jamie and Samu added webmaster validation to id.parliament.uk and api.parliament.uk, so we can better control how search engines interact with our services.

Chris has created an [index of member portraits](https://api.parliament.uk/query/person_photo_index). The list is available in a variety of formats including [JSON](https://api.parliament.uk/query/person_photo_index.json), [XML](https://api.parliament.uk/query/person_photo_index.xml) and [CSV](https://api.parliament.uk/query/person_photo_index.csv). There's a note to say some Peers have now had their photos taken. They'll be available through the API and beta website in the very near future.

Raphael's found a way to correlate our server and client side logs, so various aspects of telemetry can be grouped by one operation ID. Which should all go to toward helping analysts with measuring things.

### Data toolkit

After various conversations with Steve Wise and Anya, [Aidan](https://twitter.com/aidan_morgan) has started working on a vision and strategy document for the Data Toolkit and Vocabulary Management work. He's also spent some time with Samu getting his input. In a similar vein, he's been working with HR to get two developer roles advertised so we'll actually have people to do the work as well as write the documents.

Chris spent some time looking into existing vocabularies for subject indexing content. He found [MUTO](https://www.researchgate.net/publication/220727264_MUTO_The_modular_unified_tagging_ontology) which could solve some of our problems. Samu read [a paper describing MUTO with a review of other tagging ontologies](https://www.researchgate.net/publication/220727264_MUTO_The_modular_unified_tagging_ontology) which he found most helpful.

### Corporate data

The House of Commons HR system feed is now live. Hurrah.

[Matt](https://twitter.com/matiasgermanico) discovered that the fiance system feed contains tab characters. He needs to modify the pipeline to strip out extended characters.

Noel continued with his review of the data held in People Directory and Lewis continued with development work on the new stock and finance systems integration. He also did a bit of codebase maintenance.
 
David continued development work on the new facilities management system.

### Excellent customer service award...

...has joint winners this week.

[Alex](https://twitter.com/alexedwardh) wrote some automated [Solr](http://lucene.apache.org/solr/) queries to grab all written parliamentary questions between 1997 and 2017 for the [Knesset Archives](https://www.knesset.gov.il/archive/eng/ArchiveIntro_eng.htm). He ended up with over 100 spreadsheets and then used [Python](https://www.python.org/) to strip out unnecessary columns and merge them all into one big CSV file.

Chris spent some time explaining how to make use of our photo API to some people from Sky. Member photos are flying free.

### Are topics fashionable?

We now have presentations about presentations. Or meta presentations if you will. So yes.

### How many doctors have we got?

Still just the two. Must try harder here.

### Did anybody say orthogonal?

Michael said orthogonal. Many times. As is his want.

### Strolls

No strolls reported again this week, though Anya, our Liz, Samu and Ben all made their way to [Newspeak House](https://www.nwspk.com/) for an event Michael organised about [anaytics, user tracking and privacy](https://attending.io/events/analytics-tracking-and-privacy-in-the-public-sector). It was good, he thought. And he was pleased to see friendly faces.

### Things that caught our eye

* [MUTO: The modular unified tagging ontology](https://www.researchgate.net/publication/220727264_MUTO_The_modular_unified_tagging_ontology)

* [What’s your Machine Learning Test Score? A rubric for ML production systems](https://www.eecs.tufts.edu/~dsculley/papers/ml_test_score.pdf) [PDF]