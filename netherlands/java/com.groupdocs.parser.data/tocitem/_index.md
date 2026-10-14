---
title: "TocItem"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt het item voor dat wordt gebruikt in de functionaliteit voor het extraheren van de inhoudsopgave."
type: docs
weight: 31
url: /nl/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Stelt het item voor dat wordt gebruikt in de functionaliteit voor het extraheren van de inhoudsopgave.

Een instantie van de [TocItem](../../com.groupdocs.parser.data/tocitem) klasse wordt gebruikt als retourwaarde van de [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) methode. Zie de gebruiksvoorbeelden daar.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Initialiseert een nieuwe instantie van de TocItem‑klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDepth()](#getDepth--) | Haalt het diepte‑niveau op. |
|
|  | [getText()](#getText--) | Haalt de tekst op. |
|
|  | [getPageIndex()](#getPageIndex--) | Haalt het paginanummer op. |
|
|  | [extractText()](#extractText--) | Haalt een tekst uit het document waarnaar het TocItem‑object verwijst. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Initialiseert een nieuwe instantie van de TocItem‑klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | diepte | int | Het diepte‑niveau van het item. |
|
|  | tekst | java.lang.String | De tekst van het item. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarnaar het item verwijst |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Haalt het diepte‑niveau op.


**Returns:**
int - Een gehele getalwaarde die het diepte‑niveau van het item weergeeft.

### getText() {#getText--}
```
public String getText()
```


Haalt de tekst op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de tekst van het item weergeeft.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Haalt het paginanummer op.


**Returns:**
java.lang.Integer - Een gehele getalwaarde die de index van de pagina waarnaar het item verwijst weergeeft;  null  als deze niet is ingesteld.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Haalt een tekst uit het document waarnaar het TocItem‑object verwijst.

Het volgende voorbeeld laat zien hoe een tekst te extraheren via een item uit de inhoudsopgave:

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

