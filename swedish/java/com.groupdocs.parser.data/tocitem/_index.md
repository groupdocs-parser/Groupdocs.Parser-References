---
title: "TocItem"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar objektet som används i funktionaliteten för extrahering av innehållsförteckning."
type: docs
weight: 31
url: /sv/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Representerar objektet som används i funktionaliteten för extrahering av innehållsförteckning.

En instans av klassen [TocItem](../../com.groupdocs.parser.data/tocitem) används som returvärde för metoden [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--). Se användningsexemplen där.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Initierar en ny instans av klassen TocItem. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDepth()](#getDepth--) | Hämtar djupnivån. |
|
|  | [getText()](#getText--) | Hämtar texten. |
|
|  | [getPageIndex()](#getPageIndex--) | Hämtar sidindexet. |
|
|  | [extractText()](#extractText--) | Extraherar en text från dokumentet som TocItem-objektet refererar till. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Initierar en ny instans av klassen TocItem.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | depth | int | Djupnivån för objektet. |
|
|  | text | java.lang.String | Texten för objektet. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan som objektet refererar till |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Hämtar djupnivån.


**Returns:**
int - Ett heltalsvärde som representerar djupnivån för objektet.

### getText() {#getText--}
```
public String getText()
```


Hämtar texten.


**Returns:**
java.lang.String - Ett strängvärde som representerar objektets text.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Hämtar sidindexet.


**Returns:**
java.lang.Integer - Ett heltalsvärde som representerar indexet för sidan som objektet refererar till;  null  om det inte är satt.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Extraherar en text från dokumentet som TocItem-objektet refererar till.

Följande exempel visar hur man extraherar en text med ett objekt i innehållsförteckningen:

````
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
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

