---
title: "SearchResult"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar sökresultatet i sökfunktionen."
type: docs
weight: 27
url: /sv/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Representerar sökresultatet i sökfunktionen.

En instans av klassen SearchResult används som returvärde för [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-)
och [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-) metoder. Se användningsexemplen där.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Initierar en ny instans av klassen [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Initierar en ny instans av klassen [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getPosition()](#getPosition--) | Hämtar positionen i dokumenttexten. |
|
|  | [getText()](#getText--) | Hämtar texten. |
|
|  | [getPageIndex()](#getPageIndex--) | Hämtar sidindex där texten hittas. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Hämtar den vänstra markeringen. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Hämtar den högra markeringen. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Initierar en ny instans av klassen [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | int | Positionen i dokumenttexten. |
|
|  | text | java.lang.String | Den hittade texten. |
|
|  | pageIndex | java.lang.Integer | Sidindex där texten hittas. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Den vänstra markeringen. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Den högra markeringen. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Initierar en ny instans av klassen [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | int | Positionen i dokumenttexten. |
|
|  | text | java.lang.String | Den hittade texten. |
|
|  | pageIndex | java.lang.Integer | Sidindex där texten hittas. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Hämtar positionen i dokumenttexten.


**Returns:**
int - Ett nollbaserat index för startpositionen för sökresultatet.

### getText() {#getText--}
```
public String getText()
```


Hämtar texten.


**Returns:**
java.lang.String - Ett strängvärde som representerar den hittade texten.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Hämtar sidindex där texten hittas.


**Returns:**
java.lang.Integer - Ett nollbaserat index för sidan där texten hittas;  null  om sökningen utförs på hela dokumentets text.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Hämtar den vänstra markeringen.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Hämtar den högra markeringen.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

