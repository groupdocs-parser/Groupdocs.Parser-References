---
title: "HighlightItem"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een markering van een deel van de tekst voor die meestal wordt gebruikt om de context van de gevonden tekst in de zoekfunctionaliteit uit te leggen."
type: docs
weight: 14
url: /nl/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Stelt een markering voor, een deel van de tekst dat meestal wordt gebruikt om de context van de gevonden tekst in de zoekfunctionaliteit uit te leggen.

Een instantie van [HighlightItem](../../com.groupdocs.parser.data/highlightitem) klasse wordt gebruikt als retourwaarde van [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) methode,
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Initialiseert een nieuwe instantie van de [HighlightItem](../../com.groupdocs.parser.data/highlightitem) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getPosition()](#getPosition--) | Haalt de positie op in de documenttekst. |
|
|  | [getText()](#getText--) | Haalt de tekst van de markering op. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Initialiseert een nieuwe instantie van de [HighlightItem](../../com.groupdocs.parser.data/highlightitem) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | positie | int | De positie in de documenttekst. |
|
|  | tekst | java.lang.String | De tekst van de markering. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Haalt de positie op in de documenttekst.


**Returns:**
int - Een nulgebaseerde index van de startpositie van de markering.

### getText() {#getText--}
```
public String getText()
```


Haalt de tekst van de markering op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de tekst van de markering weergeeft.

