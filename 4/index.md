## Week 4: 18-08-2017

### Community

On Thursday we announced our 4th Parliament, data and democracy meetup, again at [Newspeak House](https://www.nwspk.com/). There'll be three speakers this time (four if you include our [Dan](https://twitter.com/dasbarrett)):

* [Anna Scott](https://twitter.com/Anna_D_Scott) from the [Open Data Institute](https://theodi.org/) on the impact of open data on democracies around the world.

* [Rachel Coldicutt](https://twitter.com/RachelColdicutt) of [doteveryone](https://doteveryone.org.uk/) on things related to her rather excellent piece on [Taming the Gods of the Anthropocene](https://medium.com/doteveryone/first-do-no-harm-taming-the-gods-of-the-anthropocene-261f33d9462d).

* And our own [Samu Lang](https://twitter.com/langsamu) on the new Parliament data platform.

If you're desperate enough to be reading this and anywhere in or around London you can [sign up here](https://attending.io/events/parliament-data-and-democracy-meetup-4).

[Raphael](https://twitter.com/raphaelleung) hosted a team of data analysts from the Department of Work and Pension Universal Credit data team on Tuesday. They also attended the show and tell. 

### Capability

Tuesday was invite your friends to work day so [Michael](https://twitter.com/fantasticlife) invited [Nic Ferrier](https://twitter.com/nicferrier) to talk about (proper) agile, continuous delivery and testing (or not).

Nic met with Robert in the [hotbed of activity](https://www.youtube.com/watch?v=QUYKSWQmkrg) that is the Millbank Canteen, then gave a talk to assorted developers and otherwise on how to do agile and continuous delivery with more emphasis on conversations and actually shipping software, less on the veneer of [ceremony](https://www.youtube.com/watch?v=H5UK40sSo8I).

Wednesday was Data Day which, given lots of people are on holiday, was low on numbers but [high on sun and smiles](https://twitter.com/benwoodhams/status/897823501272309761). And generally [getting stuff done](https://twitter.com/benwoodhams/status/897825226586763264).

Matthieu and Liz spent some time tidying up our email distribution lists, shared email addresses, and SharePoint site. We are now data *and search*.

### Domain modelling

Angela, [Ben](https://twitter.com/benwoodhams), Michael and [Silver](https://twitter.com/silveroliver) spent Thursday going back over the select committee domain modelling work and starting to split the model into more manageable chunks of [core stuff](https://github.com/ukparliament/ontologies/blob/master/_formal-body/formal-body.png), [events](https://github.com/ukparliament/ontologies/blob/master/_event/event.png), [calls and contributions](https://github.com/ukparliament/ontologies/blob/master/_calls-and-contributions/calls-and-contributions.png), and the [start of a document model](https://github.com/ukparliament/ontologies/blob/master/_document/document.png).

They also checked it against the Committee Office Database (CODA) used by committees in the House of Lords. Everything seemed to fit. At least in principle.

Ben's currently revising his data integrity paper with input from [Steve Goodrich](https://twitter.com/steveJgoodrich). [Anya](https://twitter.com/bitten_) and Michael plan to discuss with Commons colleagues who look after the register of Members' financial interests.

Ben also met with a Commons colleague to discuss their plans for building an [Statutory Instrument](http://www.parliament.uk/business/bills-and-legislation/secondary-legislation/statutory-instruments/) tracker, and discussed with Samu.

### Data service

[Chris](https://twitter.com/chrisalcockdev) integrated Northern Ireland postcode search into the Data Service. For now it's an an interim solution but Chris and [Aidan](https://twitter.com/aidan_morgan) are working on fixing things properly.

[Jianhan](https://twitter.com/jianhanzhu) investigated accessing internal databases from the cloud data platform by setting up a database gateway and an on-premise data gateway on his machine to talk to local databases. The attempt was successful, and a logic app application was set up to read database record rows.

Jianhan also continued to work with cleaning and filling gaps in Members Names Information Service (MNIS) committee data. We had had 24 unmatched current committees and we're now down to 17. We're still waiting for the Commons to get back with their mappings. 43 former committees are still unmatched and we need to work on this next.

Raphael met with [Liz Marley](https://twitter.com/greensideknits) from the Indexing and Data Management Section of the Commons Library to give an update on topic tagging project and the data toolkit.

He also went to the [GDS](https://gds.blog.gov.uk/) data science accelerator on Thursday. The chat with Liz provided more context around the [current topic page term hierarchy](https://bl.ocks.org/lcyraphael/raw/421f3f14854cb49a8fd199f9e326ecaa/). He's now tweaked the approach to treat it as a multiclass classification problem.

### Search

Work continues apace on search in the run-up to our 8th September launch. Search stands-ups are going well and the 'low-tech' post-it kanban seems preferable to trying to drag boxes around screens.

Robert met with [Laurence](https://twitter.com/laurencegrinyer) on page design for search. He also met with colleagues from Data and Search to learn more about the options for the display of search results and forthcoming work.

[Dia](https://twitter.com/DN78) also worked on user interface side of things and prepared for putting the feedback mechanism in place.

Robert and Dia agreed to showcase search as part of website show and tell.

Matthieu did the last round of tests on search before we switch to live.

### Measuring things

Ben and Liz took over show and tell to present on measuring civic value and how you might and whether you could.

Matthieu worked on linking our dashboard software to our cloud insights data.

Liz met with Jeremy Hardacre to agree an approach for migrating library enquiries reporting away from a manual export process. She also sent Gavin Berman a basic report on enquiries workload for one library section and corrected some dodgy records.

Liz also talked to [Jeanette](https://twitter.com/clementgraphics) about establishing a review process for website surveys and a log for user research.

### Comings and goings

We got the good news that Alexander (an engineer) is going to be joining us at the end of September.

And the sad news that Ben's reached the end of his attachment and is off on holiday, then back to the Lords.


### Links

Robert uncovered:

* [PyGraphistry is library to extract, transform, and visually explore big graphs
](https://github.com/graphistry/pygraphistry/)

* [Peach family tree](https://twitter.com/tsukijiichiba/statuses/895564616398327808)

* [Charity arcade machines for the Red Cross](https://twitter.com/mobcrush/statuses/897171365752705024)

* [A blog post on the old chestnut, How buildings learn](http://www.gyford.com/phil/writing/2004/10/24/how_buildings_le.php)

Raphael found:

* [A handy AI and Machine Learning cheat sheet](https://becominghuman.ai/cheat-sheets-for-ai-neural-networks-machine-learning-deep-learning-big-data-678c51b4b463)

* [An essay on data visualisation and histograms](https://tinlizzie.org/histograms/)

* [A D3 tag hierarchy visualisation tool](https://bl.ocks.org/lcyraphael/421f3f14854cb49a8fd199f9e326ecaa)

* [An xdcd on statistics and data science](http://livefreeordichotomize.com/2016/12/15/hill-for-the-data-scientist-an-xkcd-story/)

* [word2vec - an algorithm to transform words into vectors](http://p.migdal.pl/2017/01/06/king-man-woman-queen-why.html





