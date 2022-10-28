---
title: PageArea
second_title: GroupDocs.Parser for Java API Reference
description: Represents an abstract base class for page areas which are used to represent blocks on the document page in the parsing by template functionality.
type: docs
weight: 16
url: /java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Represents an abstract base class for page areas which are used to represent blocks on the document page in the parsing by template functionality.
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area. |
| [getPage()](#getPage--) | Gets the document page information such as page index and page size. |
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.
### getPage() {#getPage--}
```
public Page getPage()
```


Gets the document page information such as page index and page size.

**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.
