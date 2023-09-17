---
title: PageGroupArea
second_title: GroupDocs.Parser for Java API Reference
description: Represents a group of page areas which is used to group different types of blocks of the document page in the parsing by template functionality.
type: docs
weight: 19
url: /java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Represents a group of page areas which is used to group different types of blocks of the document page in the parsing by template functionality.
## Constructors

| Constructor | Description |
| --- | --- |
| [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Initializes a new instance of the [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) class. |
## Methods

| Method | Description |
| --- | --- |
| [getAreas()](#getAreas--) | Gets the collection of grouped page areas. |
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Initializes a new instance of the [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | The collection of page areas to be grouped. |
| page | [Page](../../com.groupdocs.parser.data/page) | The page that contains the area. |

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Gets the collection of grouped page areas.

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - A collection of [PageArea](../../com.groupdocs.parser.data/pagearea) objects.
