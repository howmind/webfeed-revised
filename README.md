# WebFeed Revised

[![Pub](https://img.shields.io/pub/v/webfeed_revised.svg)](https://pub.dev/packages/webfeed_revised)

A dart package for parsing RSS and Atom feed.

Forked from [WebFeed - V0.7.0](https://pub.dev/packages/webfeed) and improved upon

### Features

- [x] RSS (0.9, 1.0, & 2.0)
- [x] Atom
- [x] Namespaces
    - [x] Media RSS
    - [x] Dublin Core
    - [x] iTunes
    - [x] Syndication

### Installing

Add this line into your `pubspec.yaml`
```
webfeed_revised: ^0.8.0
```

Import the package into your dart code using:
```
import 'package:webfeed_revised/webfeed_revised.dart';
```

### Example

To parse string into `RssFeed` object use:
```
var rssFeed = RssFeed.parse(xmlString); // for parsing RSS feed
var atomFeed = AtomFeed.parse(xmlString); // for parsing Atom feed
```

### Preview

**RSS**
```
feed.title
feed.description
feed.link
feed.author
feed.items
feed.image
feed.cloud
feed.categories
feed.skipDays
feed.skipHours
feed.lastBuildDate
feed.language
feed.generator
feed.copyright
feed.docs
feed.managingEditor
feed.rating
feed.webMaster
feed.ttl
feed.dc

RssItem item = feed.items.first;
item.title
item.description
item.link
item.categories
item.guid
item.pubDate
item.author
item.comments
item.source
item.media
item.enclosure
item.dc
```

**Atom**
```
feed.id
feed.title
feed.updated
feed.items
feed.links
feed.authors
feed.contributors
feed.categories
feed.generator
feed.icon
feed.logo
feed.rights
feed.subtitle

AtomItem item = feed.items.first;
item.id
item.title
item.updated
item.authors
item.links
item.categories
item.contributors
item.source
item.published
item.content
item.summary
item.rights
item.media
```

## License

WebFeed Revised is licensed under the BSD 3-clause License - see the [LICENSE](LICENSE) file for details

WebFeed, from which this repository is forked, is licensed under the MIT License - see the [LICENSE-ORIGINAL](LICENSE-ORIGINAL) file for details
