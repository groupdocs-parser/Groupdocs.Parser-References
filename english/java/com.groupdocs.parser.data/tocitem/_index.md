---
title: TocItem
second_title: GroupDocs.Parser for Java API Reference
description: Represents the item which is used in the table of contents extraction functionality.
type: docs
weight: 31
url: /java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Represents the item which is used in the table of contents extraction functionality.

An instance of [TocItem](../../com.groupdocs.parser.data/tocitem) class is used as return value of [Parser.getToc()](../../com.groupdocs.parser/parser\#getToc--) method. See the usage examples there.
## Constructors

| Constructor | Description |
| --- | --- |
| [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Initializes a new instance of the TocItem class. |
## Methods

| Method | Description |
| --- | --- |
| [getDepth()](#getDepth--) | Gets the depth level. |
| [getText()](#getText--) | Gets the text. |
| [getPageIndex()](#getPageIndex--) | Gets the page index. |
| [extractText()](#extractText--) | Extracts a text from the document to which TocItem object refers. |
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Initializes a new instance of the TocItem class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| depth | int | The depth level of the item. |
| text | java.lang.String | The text of the item. |
| pageIndex | java.lang.Integer | The index of the page referenced by the item |

### getDepth() {#getDepth--}
```
public int getDepth()
```


Gets the depth level.

**Returns:**
int - An integer value that represents the depth level of the item.
### getText() {#getText--}
```
public String getText()
```


Gets the text.

**Returns:**
java.lang.String - A string value that represents the text of the item.
### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Gets the page index.

**Returns:**
java.lang.Integer - An integer value that represents the index of the page referenced by the item;  null  if it isn't set.
### extractText() {#extractText--}
```
public TextReader extractText()
```


Extracts a text from the document to which TocItem object refers.

The following example how to extract a text by the an item of table of contents:

```
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
```

**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.
