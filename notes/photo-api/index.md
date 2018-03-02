# Data platform photo API

There's an index of Member portraits here:

[https://api.parliament.uk/query/person_photo_index](https://api.parliament.uk/query/person_photo_index)

You can request the index in a bunch of different formats, e.g.

* [https://api.parliament.uk/query/person_photo_index.json](https://api.parliament.uk/query/person_photo_index.json)

* [https://api.parliament.uk/query/person_photo_index.xml](https://api.parliament.uk/query/person_photo_index.xml)

* [https://api.parliament.uk/query/person_photo_index.csv](https://api.parliament.uk/query/person_photo_index.csv)

From this you can get the URIs of the photos in our triple store, e.g. 

[https://id.parliament.uk/iXSJ5Acp](https://id.parliament.uk/iXSJ5Acp)

If you take the ID from the end of this and go to our photo API, you get the full size image, with metadata embedded,
e.g.

[https://api.parliament.uk/photo/iXSJ5Acp](https://api.parliament.uk/photo/iXSJ5Acp)

As you can see from our media pages ([https://beta.parliament.uk/media/iXSJ5Acp](https://beta.parliament.uk/media/iXSJ5Acp)), you can add parameters to crop and resize the photos from our API rather than on your end, e.g.

* [https://api.parliament.uk/photo/iXSJ5Acp.jpeg?crop=MCU_3:2&quality=80&download=true](https://api.parliament.uk/photo/iXSJ5Acp.jpeg?crop=MCU_3:2&quality=80&download=true)

* [https://api.parliament.uk/photo/iXSJ5Acp.jpeg?crop=MCU_3:4&quality=80&download=true](https://api.parliament.uk/photo/iXSJ5Acp.jpeg?crop=MCU_3:4&quality=80&download=true)

* [https://api.parliament.uk/photo/iXSJ5Acp.jpeg?crop=CU_1:1&quality=80&download=true](https://api.parliament.uk/photo/iXSJ5Acp.jpeg?crop=CU_1:1&quality=80&download=true)

The examples above are all in use, so should be cached and fast to serve. If you ask for custom parameters it may take a while per photo.

Your use will be subject to rate limiting – 10 calls per second per IP address for /query, 60 calls per second per IP address for /photo

Returning to the results from [https://api.parliament.uk/query/person_photo_index](https://api.parliament.uk/query/person_photo_index), please notice that the person URI (e.g. [https://id.parliament.uk/nerwVGrY](https://id.parliament.uk/nerwVGrY)) is Parliament’s canonical URI for, in this case, a person and will resolve to [https://beta.parliament.uk/people/nerwVGrY](https://beta.parliament.uk/people/nerwVGrY). 

Some Lords have had their photos taken and will be available in the near future.

The images are released under a [Creative Commons Attribution Licence](https://creativecommons.org/licenses/by/3.0/).