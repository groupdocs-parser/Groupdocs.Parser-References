---
title: Page
second_title: GroupDocs.Parser for Java API Reference
description: Represents the document page information such as page index and page size.
type: docs
weight: 16
url: /java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Represents the document page information such as page index and page size. It's used to represent the page that contains inheritors of [PageArea](../../com.groupdocs.parser.data/pagearea) class in the parsing by template functionality.
## Constructors

| Constructor | Description |
| --- | --- |
| [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Initializes a new instance of the [Page](../../com.groupdocs.parser.data/page) class. |
## Methods

| Method | Description |
| --- | --- |
| [getIndex()](#getIndex--) | Gets the page index. |
| [getSize()](#getSize--) | Gets the page size. |
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Initializes a new instance of the [Page](../../com.groupdocs.parser.data/page) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The page index. |
| size | [Size](../../com.groupdocs.parser.data/size) | The page size. |

### getIndex() {#getIndex--}
```
public int getIndex()
```


Gets the page index.

**Returns:**
int - A zero-based index of the page.
### getSize() {#getSize--}
```
public Size getSize()
```


Gets the page size.

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.
