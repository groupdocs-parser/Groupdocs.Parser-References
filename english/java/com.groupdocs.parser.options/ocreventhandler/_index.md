---
title: OcrEventHandler
second_title: GroupDocs.Parser for Java API Reference
description: Provides a handler for OCR events.
type: docs
weight: 26
url: /java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Provides a handler for OCR events.
## Constructors

| Constructor | Description |
| --- | --- |
| [OcrEventHandler()](#OcrEventHandler--) | Initializes a new instance of the [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class. |
## Methods

| Method | Description |
| --- | --- |
| [getWarnings()](#getWarnings--) | Gets a list of warning messages. |
| [hasWarnings()](#hasWarnings--) | Gets the value that indicates whether the list of warnings isn't empty. |
| [getWarnings(int pageIndex)](#getWarnings-int-) | Returns a list of warning messages for the page with  pageIndex . |
| [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Sets warning messages for the page. |
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Initializes a new instance of the [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class.

### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Gets a list of warning messages.

**Returns:**
java.util.List<java.lang.String> - A list of warning messages for all pages.
### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Gets the value that indicates whether the list of warnings isn't empty.

**Returns:**
boolean -  true  if the list of warnings isn't empty; otherwise,  false .
### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Returns a list of warning messages for the page with  pageIndex .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |

**Returns:**
java.util.List<java.lang.String> - A list of warning messages for the page; empty list if no warning messages for the page.
### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Sets warning messages for the page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int | The zero-based page index. |
| warnings | java.lang.Iterable<java.lang.String> | The list of warning messages for the page. |

