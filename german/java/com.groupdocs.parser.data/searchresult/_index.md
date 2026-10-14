---
title: "SearchResult"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt das Suchergebnis in der Suchfunktion dar."
type: docs
weight: 27
url: /de/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Stellt das Suchergebnis in der Suchfunktion dar.

Eine Instanz der SearchResult-Klasse wird als Rückgabewert von [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-) verwendet
und den Methoden [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-). Siehe dort die Anwendungsbeispiele.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Initialisiert eine neue Instanz der [SearchResult](../../com.groupdocs.parser.data/searchresult)-Klasse. |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Initialisiert eine neue Instanz der [SearchResult](../../com.groupdocs.parser.data/searchresult)-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getPosition()](#getPosition--) | Liefert die Position im Dokumenttext. |
|
|  | [getText()](#getText--) | Liefert den Text. |
|
|  | [getPageIndex()](#getPageIndex--) | Liefert den Seitenindex, an dem der Text gefunden wird. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Liefert die linke Hervorhebung. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Liefert die rechte Hervorhebung. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Initialisiert eine neue Instanz der [SearchResult](../../com.groupdocs.parser.data/searchresult)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Position | int | Die Position im Dokumenttext. |
|
|  | Text | java.lang.String | Der gefundene Text. |
|
|  | pageIndex | java.lang.Integer | Der Seitenindex, an dem der Text gefunden wird. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Die linke Hervorhebung. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Die rechte Hervorhebung. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Initialisiert eine neue Instanz der [SearchResult](../../com.groupdocs.parser.data/searchresult)-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Position | int | Die Position im Dokumenttext. |
|
|  | Text | java.lang.String | Der gefundene Text. |
|
|  | pageIndex | java.lang.Integer | Der Seitenindex, an dem der Text gefunden wird. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Liefert die Position im Dokumenttext.


**Returns:**
int - Ein nullbasierter Index der Startposition des Suchergebnisses.

### getText() {#getText--}
```
public String getText()
```


Liefert den Text.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den gefundenen Text darstellt.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Liefert den Seitenindex, an dem der Text gefunden wird.


**Returns:**
java.lang.Integer - Ein nullbasierter Index der Seite, auf der der Text gefunden wird;  null  wenn die Suche im gesamten Dokumenttext durchgeführt wird.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Liefert die linke Hervorhebung.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Liefert die rechte Hervorhebung.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

