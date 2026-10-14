---
title: "SearchResult"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt het zoekresultaat voor in de zoekfunctionaliteit."
type: docs
weight: 27
url: /nl/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Stelt het zoekresultaat voor in de zoekfunctionaliteit.

Een instantie van de SearchResult-klasse wordt gebruikt als retourwaarde van [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-)
en [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) methoden. Zie daar de gebruiksvoorbeelden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Initialiseert een nieuwe instantie van de [SearchResult](../../com.groupdocs.parser.data/searchresult) klasse. |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Initialiseert een nieuwe instantie van de [SearchResult](../../com.groupdocs.parser.data/searchresult) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getPosition()](#getPosition--) | Haalt de positie op in de documenttekst. |
|
|  | [getText()](#getText--) | Haalt de tekst op. |
|
|  | [getPageIndex()](#getPageIndex--) | Haalt het paginanummer op waar de tekst is gevonden. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Haalt de linkermarkering op. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Haalt de rechtermarkering op. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Initialiseert een nieuwe instantie van de [SearchResult](../../com.groupdocs.parser.data/searchresult) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | positie | int | De positie in de documenttekst. |
|
|  | tekst | java.lang.String | De gevonden tekst. |
|
|  | pageIndex | java.lang.Integer | Het paginanummer waar de tekst is gevonden. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | De linkermarkering. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | De rechtermarkering. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Initialiseert een nieuwe instantie van de [SearchResult](../../com.groupdocs.parser.data/searchresult) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | positie | int | De positie in de documenttekst. |
|
|  | tekst | java.lang.String | De gevonden tekst. |
|
|  | pageIndex | java.lang.Integer | Het paginanummer waar de tekst is gevonden. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Haalt de positie op in de documenttekst.


**Returns:**
int - Een nulgebaseerde index van de startpositie van het zoekresultaat.

### getText() {#getText--}
```
public String getText()
```


Haalt de tekst op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de gevonden tekst weergeeft.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Haalt het paginanummer op waar de tekst is gevonden.


**Returns:**
java.lang.Integer - Een nulgebaseerde index van de pagina waar de tekst is gevonden; null als de zoekopdracht wordt uitgevoerd op de volledige documenttekst.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Haalt de linkermarkering op.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Haalt de rechtermarkering op.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

