---
title: "PageArea"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει μια αφηρημένη βασική κλάση για περιοχές σελίδας που χρησιμοποιούνται για την αναπαράσταση μπλοκ στη σελίδα του εγγράφου στη λειτουργία ανάλυσης με πρότυπο."
type: docs
weight: 17
url: /el/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Αντιπροσωπεύει μια αφηρημένη βασική κλάση για περιοχές σελίδας που χρησιμοποιούνται για την αναπαράσταση μπλοκ στη σελίδα του εγγράφου στη λειτουργία ανάλυσης με πρότυπο.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Λαμβάνει την ορθογώνια περιοχή. |
|
|  | [getPage()](#getPage--) | Λαμβάνει τις πληροφορίες σελίδας του εγγράφου, όπως ο δείκτης σελίδας και το μέγεθος σελίδας. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Λαμβάνει την ορθογώνια περιοχή.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Λαμβάνει τις πληροφορίες σελίδας του εγγράφου, όπως ο δείκτης σελίδας και το μέγεθος σελίδας.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

