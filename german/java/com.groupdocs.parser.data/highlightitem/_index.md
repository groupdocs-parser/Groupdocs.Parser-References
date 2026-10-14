---
title: "HighlightItem"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine Hervorhebung eines Textabschnitts dar, die üblicherweise verwendet wird, um den Kontext des gefundenen Textes in der Suchfunktion zu erklären."
type: docs
weight: 14
url: /de/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Stellt eine Hervorhebung dar, einen Teil des Textes, der normalerweise verwendet wird, um den Kontext des gefundenen Textes in der Suchfunktion zu erklären.

Eine Instanz der Klasse [HighlightItem](../../com.groupdocs.parser.data/highlightitem) wird als Rückgabewert der Methode [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-) verwendet,
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getPosition()](#getPosition--) | Liefert die Position im Dokumenttext. |
|
|  | [getText()](#getText--) | Liefert den Text der Hervorhebung. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Initialisiert eine neue Instanz der Klasse [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Position | int | Die Position im Dokumenttext. |
|
|  | Text | java.lang.String | Der Text der Hervorhebung. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Liefert die Position im Dokumenttext.


**Returns:**
int - Ein nullbasierter Index der Startposition der Hervorhebung.

### getText() {#getText--}
```
public String getText()
```


Liefert den Text der Hervorhebung.


**Returns:**
java.lang.String - Ein String‑Wert, der den Text der Hervorhebung darstellt.

