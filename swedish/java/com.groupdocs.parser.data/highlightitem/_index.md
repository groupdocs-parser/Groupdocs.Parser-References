---
title: "HighlightItem"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en markering av en del av texten som vanligtvis används för att förklara sammanhanget för den hittade texten i sökfunktionen."
type: docs
weight: 14
url: /sv/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Representerar en markering, en del av texten som vanligtvis används för att förklara sammanhanget för den hittade texten i sökfunktionen.

En instans av klassen [HighlightItem](../../com.groupdocs.parser.data/highlightitem) används som returvärde för metoden [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-),
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Initierar en ny instans av klassen [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getPosition()](#getPosition--) | Hämtar positionen i dokumenttexten. |
|
|  | [getText()](#getText--) | Hämtar texten för markeringen. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Initierar en ny instans av klassen [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | int | Positionen i dokumenttexten. |
|
|  | text | java.lang.String | Texten för markeringen. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Hämtar positionen i dokumenttexten.


**Returns:**
int - Ett nollbaserat index för startpositionen för markeringen.

### getText() {#getText--}
```
public String getText()
```


Hämtar texten för markeringen.


**Returns:**
java.lang.String - Ett strängvärde som representerar texten för markeringen.

