---
title: "HighlightOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för att extrahera en markering av ett textblock runt hittad text i sökscenarier."
type: docs
weight: 22
url: /sv/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Tillhandahåller de alternativ som används för att extrahera en markering (ett textblock runt hittad text i sökscenarier).

En instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klass används som parameter i [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-) metod.
Se användningsexemplen där.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen utan några begränsningar. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen som används för att extrahera en markering med fast längd. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen som används för att extrahera en radbegränsad markering. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen som används för att extrahera en markering med ett fast ordantal. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Hämtar en maximal textlängd. |
|
|  | [getWordCount()](#getWordCount--) | Hämtar ett maximalt ordantal. |
|
|  | [isLineLimited()](#isLineLimited--) | Hämtar värdet som indikerar om markeringsextraktion är begränsad av början (eller slutet) av en textrad. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Ställer in en maximal textlängd. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Ställer in ett maximalt ordantal. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Ställer in värdet som indikerar om markeringsextraktion är begränsad av början (eller slutet) av en textrad. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen utan några begränsningar. Ställ in minst en av #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) innan du skickar den till parsern.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen som används för att extrahera en markering med fast längd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | maxLength | int | Den maximala textlängden. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen som används för att extrahera en radbegränsad markering.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Den maximala textlängden. |
|
|  | isLineLimited | boolean | Värdet som indikerar om markeringsextraktionen begränsas av början (eller slutet) på en textrad. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen som används för att extrahera en markering med ett fast ordantal.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Den maximala textlängden. |
|
|  | wordCount | int | Det maximala antalet ord. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Initierar en ny instans av [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Den maximala textlängden. |
|
|  | wordCount | java.lang.Integer | Det maximala antalet ord. |
|
|  | isLineLimited | boolean | Värdet som indikerar om markeringsextraktionen begränsas av början (eller slutet) på en textrad. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Hämtar en maximal textlängd.


**Returns:**
java.lang.Integer - Ett positivt heltal som representerar den maximala textlängden;  null  om textlängden inte är begränsad.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Hämtar ett maximalt ordantal.


**Returns:**
java.lang.Integer - Ett positivt heltal som representerar det maximala antalet ord;  null  om antalet ord inte är begränsat.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Hämtar värdet som indikerar om markeringsextraktion är begränsad av början (eller slutet) av en textrad.


**Returns:**
boolean -  true  om markeringsextraktionen begränsas av början (eller slutet) på en textrad; annars,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Ställer in en maximal textlängd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Ett icke-negativt heltal;  null  för att ta bort längdbegränsningen. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Ställer in ett maximalt ordantal.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Ett icke-negativt heltal;  null  för att ta bort begränsningen av antalet ord. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Ställer in värdet som indikerar om markeringsextraktion är begränsad av början (eller slutet) av en textrad.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | lineLimited | boolean | true  för att begränsa efter radgränser. |
|

