---
title: DocumentPageData
second_title: GroupDocs.Parser for Java API Reference
description: Represents data of the document page.
type: docs
weight: 12
url: /java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Represents data of the document page. It consists of [FieldData](../../com.groupdocs.parser.data/fielddata) objects which contain field data from the document page.
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Initializes a new instance of the [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) class. |
## Methods

| Method | Description |
| --- | --- |
| [getPageIndex()](#getPageIndex--) | Gets the page index. |
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Initializes a new instance of the [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fields | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | The collection of fields data. |
| pageIndex | int | The zero-based page index. |

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Gets the page index.

**Returns:**
int - A zero-based index of the page.
