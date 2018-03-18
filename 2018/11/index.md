## 2018 Week 11

### [Naughty 40](https://www.youtube.com/watch?v=u3ZvO4pcTHs)

Wednesday was [dator day 40](https://twitter.com/dasbarrett/status/973990252556836864). For once it was a short one, clocking in at a little over two hours. But we churned through a fair bit. There was lots of talk of [statutory instruments](https://en.wikipedia.org/wiki/Statutory_instrument_(UK)) and the data trail they produce through Parliament. And some discussion of interim data sources and where the responsibility for populating these should sit.

This time we were not joined by [Jamie](https://twitter.com/oddtype), so there's no list of things agreed to.

### Domain modelling

Toward the end of data day, when everyone else had gone home, [Anya](https://twitter.com/bitten_), [Samu](https://twitter.com/langsamu) and [Michael](https://twitter.com/fantasticlife) had a good chat about the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html) and how we might improve it. Our first draft had used assorted predicates to map link types through a process. Samu suggested removing these and introducing a route type class to differentiate links that cause from links that allow from links that preclude. Anya and Michael had a quick chat with [Silver](https://twitter.com/silveroliver), who agreed this was a better approach. So we've now made that change.

Anya, [Ben](https://twitter.com/benwoodhams) and Michael spent some time with Jane White (House of Lords) and Jack Dent (House of Commons) drawing flow charts for affirmative SIs. There's one for [made affirmatives](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/made-affirmative.pdf) and a separate one for [unmade affirmatives](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/unmade-affirmative.pdf). Although the two procedures share most of their steps. Anya and Michael have started a chat with Samu about mapping routes into multiple procedures.

On Tuesday Anya and Silver taught Michael how to use spreadsheets. Including that thing were you can poke one table into the cells of another. Which Michael thinks is pretty advanced foo. He's now accepting Linked In endorsements for spreadsheets.

Together they made [a series of spreadsheets](https://docs.google.com/spreadsheets/d/1Aq7qvFwnbMv6SQdRPChHRi6xI72Y5QYMuivkP6sMsFo/edit?ouid=117992679121049900737&usp=sheets_home&ths=true) to capture the pertinent parts of the procedure model. Anya and Silver then populated with the details of the [negative SI procedure](https://github.com/ukparliament/ontologies/blob/master/procedure/sis/negative.pdf). Which still needs some work.

Elsewhere, Wojciech took the spreadsheet, imported it into the data platform and started to make [a browsable version](https://procedures.azurewebsites.net/Procedure/Details/1). This is extremely cool. The team looks forward to the commissioning of an edition of [How Parliament Works](https://www.amazon.co.uk/How-Parliament-Works-Robert-Rogers/dp/0273790374) for a more machine based audience.

Away from the world of procedure and SIs, Anya, Silver and Michael spent a chunk of Tuesday morning taking another look at the [Register of Members' Financial Interests](https://www.parliament.uk/mps-lords-and-offices/standards-and-financial-interests/parliamentary-commissioner-for-standards/registers-of-interests/register-of-members-financial-interests/). They got part way into [designing a more structured model](https://github.com/ukparliament/ontologies/blob/master/member-interest/member-interest.png) for capturing this stuff but the whole area is riddled with complications and complexities.

### One world, one web, one team

Liz and [Alex](https://twitter.com/alexedwardh) continued to work on a report of subject indexing terms and their usage for Anya and Michael. Alex wrote a script to query [data.parliament](http://www.data.parliament.uk/) for information on a big list of [subject heading IDs](http://www.data.parliament.uk/dataset/thesauri) and output the results to a CSV. It was originally sending a request for each subject heading in turn. Which is fine if you have a day or two to spare. But Wojciech helped rewrite so it now gets information in chunks of 10. Thanks Wojciech.

Anya and Michael intend to use the data to automatically match subject headings to [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) concepts and use the usage counts to prioritise the human checking that will be required.

Liz was passed a query about 'the average time to make committee report amendments' from Anya. Anya wasn't sure that the average was a good representation of the data. Which Liz thought was a great question. She'd always [encourage more suspicion over the use of the average average](https://towardsdatascience.com/on-average-youre-using-the-wrong-average-geometric-harmonic-means-in-data-analysis-2a703e21ea0) (the arithmetic one, that is, as Anya pointed out).

Anyway, Liz has used the data on 83 reports to make some plots in [R](https://en.wikipedia.org/wiki/R_(programming_language)) to help colleagues see the distribution of the data and identify outliers. Indeed the average isn't a great point estimate of these report timescales.

### Data platform

Now the Lords' Inflation work (don't ask) is done, we're able to add [seat incumbency interruptions](https://ukparliament.github.io/ontologies/house-membership/house-membership-ontology.html#d4e324) to take account of when Peers are [on leaves of absence or disqualified from attending](https://www.parliament.uk/mps-lords-and-offices/lords/-ineligible-lords/). [Chris](https://twitter.com/chrisalcockdev) has spent some time adding this to the physical ontology and the instance data. He's also updated the query API to prevent them from being considered "current" and showing up on lists of current Peers in various places on [beta.parliament.uk](https://beta.parliament.uk).

Chris has also added an end point that [lists constituencies who are currently without MPs](https://api.parliament.uk/query/vacant_constituency_index) because someone asked him which constituency didn't currently have a Member and he struggled to answer them quickly.

### Things that caught our eye

* [Everything to do with cryptocurrencies and blockchains is the domain of fast-talking conmen](https://twitter.com/jonpinnock/status/973170603841736704)
