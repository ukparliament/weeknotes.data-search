## 2018 Week 17

### Community

[Dan](https://twitter.com/dasbarrett) went down to Newport to visit the [ONS](https://www.ons.gov.uk/) and had, we're told, a really great day. The ONS folks talked about some of the work they're doing around search (including some practical applications of machines that do learning) and got Dan involved in some design activities. Dan says they have some great people and their lab space is really very good. He came away with lots to think about.

### Showing. And indeed telling

[Anya](https://twitter.com/bitten_), [Samu](https://twitter.com/langsamu), [Chris](https://twitter.com/chrisalcockdev) and Raphael gave a reprise of the work they've been doing to [model parliamentary procedure](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html) and [visualise process maps](https://procedures.azurewebsites.net/) to several clerks from the House of Commons. [Ben](https://twitter.com/benwoodhams) tried to film it, but Anya wouldn't let him. It went, says Michael, surprisingly well. There were some really good questions and no one seemed to suggest it was a nutbag endeavour. Phew.

At the regular show and tell, Liz showed the work to date on grouping search terms by applying basic string matching of a 'rule' to a search term. This includes a mechanism for people requesting terms and groups of terms they want search stats on. The sources for this are currently the new [website search](https://beta.parliament.uk/search), intranet search and an external search engine. For the rules we've used user defined terms, the [controlled vocabulary](http://www.data.parliament.uk/dataset/thesauri) and the [data platform's list of MP names](https://beta.parliament.uk/houses/1AFu55Hs/members/current).

### Searching. And indexing

[Sara](https://twitter.com/sarafreis) has been working on the analysis of the indexing data in [Solr](http://lucene.apache.org/solr/). She's currently exploring ways to use [machine learning studio](https://gallery.azure.ai/Notebook/Connect-Azure-ML-Studio-with-R-using-the-AzureML-package-2) to structure, analyse and visualise the data. She thinks it's a great way to share code and thinking with colleagues.

### One world, one web, one team

Liz has spent a bit of time looking at the [beta website](https://beta.parliament.uk/) and how it serialises what's in the data platform. She feels more familiar with the website now she knows what the opaque identifiers in the URLs represent. She got a little confused by places, which don't quite align across the data platform and the website since the website treats [constituency places](https://beta.parliament.uk/constituencies/current) separately and only lists [regions as places](https://beta.parliament.uk/places). We don't currently have the ONS region codes, only ONS constituency codes, so Liz wasn't able to look them up.

### Domain modelling

On Wednesday, Anya and [Michael](https://twitter.com/fantasticlife) made a number of tweaks to the [procedure model flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#examples) based on feedback from Jane in the House of Lords and Jack in the House of Commons. Every week I type, "they think they're almost there now", and every week they're not. They think they're almost there now.

They also made a tweak to the laying model to add [statutory days to laid papers](https://ukparliament.github.io/ontologies/laying/laying-ontology.html#d4e169) and to the procedure model to [associate procedural steps to Houses](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e130). At least I think that was this week. It all blurs to be honest.

On Thursday Anya, [James](https://twitter.com/thevinternet) and Michael met to add 'requires' arrows to the [Statutory Instrument](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) flowcharts. And made a few additional tweaks to some other arrows. Requires relationships allow us to state some kind of backwards causality and say for this thing to happen this other thing must have happened. Which makes the whole thing a little tighter. Michael notes he's [forgotten to add this to the procedure model comments](https://trello.com/c/0YAKVdnG/230-add-requires-comment-to-procedure-ontology).

Anya, Samu and Michael also met to chat about procedural data and business item data and where we could populate it from and what we'd need to do in cases where it couldn't be populated. They also spoke about [praying day periods](https://ukparliament.github.io/ontologies/time-period/time-period-ontology.html#d4e459) and the assorted clocks associated with SI procedure. Samu spoke at some length about SI procedure, clocks, the nature of time, server vs client side state, [REST](https://en.wikipedia.org/wiki/Representational_state_transfer), JavaScript and general relativity. The suggestion seemed to be, if time was relative, any concept of "now" could only exist in the agent of the beholder. Anya's and Michael's brains hurt. They went off to smoke and everything was better.

### Corporate data

[Matt](https://twitter.com/matiasgermanico) has started on a thorough documentation process for People Data (the corporate data hub that holds all our data about people...) and its integrations. Matt also announced he is leaving. The two things being not connected. Or "orthogonal" as us digital types say.

### Strolls

Once again, very few strolls were reported. Robert and Michael took a walk to the [Rag and Bone Coffee Company](https://twitter.com/ragbonecoffee). They intended to walk further but their little legs were tired.

[Edward](https://twitter.com/ewhitur) and Michael took a stroll down to Waterloo to chat about the procedure model and step names and Statutory Instrument clocks and other stuff.

Anya and Michael staged a final invasion of Robert's office and caught of a glimpse of his MASSIVE DELL. Which is now in a crate. To be shipped somewhere. Several fleeces of indeterminate age and ownership hung on a coat rack. The ceiling had collapsed and the ingress of rain water had formed an odd, Turin shroud like shape over a pin board. There was some evidence of mouses.

### Waving goodbye to Millbank

It was the final(ish) week in [7 Millbank](https://platform.carbonculture.net/places/7-millbank/45/) for the [Parliamentary Computational Section](https://pds.blog.parliament.uk/). Tears were shed as pencil cases and Garfield posters were packed and bits of falling masonry sidestepped for the last time. [Julie](https://twitter.com/julietouring) shouted at people for not putting sellotape over their stickers. Dan [thought he'd lost his mug](https://twitter.com/dasbarrett/status/989554975503241216) but [Julie found it](https://twitter.com/julietouring/status/989558806563704833). [Again](https://twitter.com/dasbarrett/status/938095115628875776). Makes a change from bloody [teapots](https://twitter.com/dasbarrett/status/985204521755402240). From next week we'll be over in [Richmond House](https://en.wikipedia.org/wiki/Richmond_House), which looks like a mad man tried to design a castle from sticklebricks. We will miss our mouses. Unless they're coming too.






