---
title: DocumentInfo
second_title: GroupDocs.Parser for Java API Reference
description: Represents the document information.
type: docs
weight: 10
url: /java/com.groupdocs.parser.options/documentinfo/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.parser.options.IDocumentInfo](../../com.groupdocs.parser.options/idocumentinfo)
```
public abstract class DocumentInfo implements IDocumentInfo
```

Represents the document information.

**Learn more:**

 *  [Get document info][]
 *  [Detect encoding][]


[Get document info]: https://docs.groupdocs.com/display/parserjava/Get+document+info
[Detect encoding]: https://docs.groupdocs.com/display/parserjava/Detect+encoding
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getFileType()](#getFileType--) | Gets the document type. |
| [getPageCount()](#getPageCount--) | Gets the total number of document pages. |
| [getRawPageCount()](#getRawPageCount--) | Gets the total number of document raw pages. |
| [getSize()](#getSize--) | Gets the size of the document in bytes. |
| [getPages()](#getPages--) | Gets the information about pages such as the index and page size. |
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Gets the document type.

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class that represents the type of the document.
### getPageCount() {#getPageCount--}
```
public abstract int getPageCount()
```


Gets the total number of document pages.

**Returns:**
int - An integer value that represents a total number of pages.
### getRawPageCount() {#getRawPageCount--}
```
public abstract int getRawPageCount()
```


Gets the total number of document raw pages.

Use [getRawPageCount()](../../com.groupdocs.parser.options/documentinfo\#getRawPageCount--) property instead of [getPageCount()](../../com.groupdocs.parser.options/documentinfo\#getPageCount--) property for raw text extraction. Some documents have different page numbers in accurate and raw text extraction modes. [getPageCount()](../../com.groupdocs.parser.options/documentinfo\#getPageCount--) property may perform extra calculations which impacts on text extraction speed in raw mode.

**Returns:**
int - An integer value that represents a total number of raw pages.
### getSize() {#getSize--}
```
public abstract long getSize()
```


Gets the size of the document in bytes.

**Returns:**
long - An integer value that represents the size of the document in bytes.
### getPages() {#getPages--}
```
public abstract List<PageInfo> getPages()
```


Gets the information about pages such as the index and page size.

**Returns:**
java.util.List<com.groupdocs.parser.options.PageInfo> - A collection with instances of [PageInfo](../../com.groupdocs.parser.options/pageinfo) classes.
