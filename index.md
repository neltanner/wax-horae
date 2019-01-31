---
layout: wax/page
show_title: false
banner:
  collection: qatar
  pid: obj10
  y: 25%
---

__Wax__ is a [minimal computing](http://go-dh.github.io/mincomp/) project for producing digital exhibitions focused on impact, durability, ease, and flexibility. Our underlying technology is made to learn and to teach, and can produce beautifully rendered, high-quality image collections and scholarly exhibits. To start using Wax, please see our [documentation](https://minicomp.github.io/wiki/#/wax/) for installation instructions and more.

Please note that __Wax is in rapid development__ and is still in the experimentation/testing phase. Wax and its accompanying documentation will become stable and semantically versioned after the beta release.

### Browse the Collection


This site's sample collection comprises a set of objects, each of which is represented by one or more images.

In the parlance of [IIIF](http://iiif.io/), each collection item is represented by a [manifest](https://iiif.io/api/presentation/2.0/#manifest) (like [this one]({{ '/img/derivatives/iiif/obj1/manifest.json' | absolute_url }})), and each image asset is a [canvas](https://iiif.io/api/presentation/2.0/#canvas) (like [this]( {{ '/img/derivatives/iiif/canvas/obj1.json' | absolute_url }})). These JSON files are interpreted by a IIIF-compliant viewer. Wax includes two viewer options: [LeafletIiif](https://github.com/mejackreed/Leaflet-IIIF) (as seen [here]({{ '/qatar/obj1/' | absolute_url }})) and [Mirador](http://projectmirador.org/), used for _[The Book of Horses]({{ '/qatar/obj12/' | absolute_url }})_. You can use either or both however you like, though Mirador is much larger to load and is best suited for documents.

The collection items in this demo are from The Museum of Islamic Art, Qatar, (courtesy of [WikiMedia](https://commons.wikimedia.org/wiki/Category:Google_Art_Project_works_in_The_Museum_of_Islamic_Art,_Qatar) and [Google Art Project](https://www.google.com/culturalinstitute/about/artproject/)) and The Qatar National Library (via [World Digital Library](https://www.wdl.org/en/)).


{% include wax/collection/gallery.html facet_by='object_type' collection='qatar' %}
