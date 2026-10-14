---
title: "HighlightOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die verwendet werden, um einen hervorgehobenen Textblock um gefundenen Text in Suchszenarien zu extrahieren."
type: docs
weight: 22
url: /de/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Stellt die Optionen bereit, die zum Extrahieren einer Hervorhebung (eines Textblocks um gefundenen Text in Suchszenarien) verwendet werden.

Eine Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) wird als Parameter in der Methode [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-) verwendet.
Siehe dort die Anwendungsbeispiele.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) ohne gesetzte Grenzen. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), die verwendet wird, um ein festlängen‑Highlight zu extrahieren. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), die verwendet wird, um ein zeilenbegrenztes Highlight zu extrahieren. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), die verwendet wird, um ein Highlight mit fester Wortanzahl zu extrahieren. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Liefert die maximale Textlänge. |
|
|  | [getWordCount()](#getWordCount--) | Liefert die maximale Wortanzahl. |
|
|  | [isLineLimited()](#isLineLimited--) | Liefert den Wert, der angibt, ob die Highlight‑Extraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Setzt die maximale Textlänge. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Setzt die maximale Wortanzahl. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Setzt den Wert, der angibt, ob die Highlight‑Extraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) ohne gesetzte Grenzen. Setzen Sie mindestens eines der folgenden: #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean), bevor Sie es an den Parser übergeben.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), die verwendet wird, um ein festlängen‑Highlight zu extrahieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | maxLength | int | Die maximale Textlänge. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), die verwendet wird, um ein zeilenbegrenztes Highlight zu extrahieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Die maximale Textlänge. |
|
|  | isLineLimited | boolean | Der Wert, der angibt, ob die Hervorhebungsextraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions), die verwendet wird, um ein Highlight mit fester Wortanzahl zu extrahieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Die maximale Textlänge. |
|
|  | wordCount | int | Die maximale Wortanzahl. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Initialisiert eine neue Instanz der Klasse [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Die maximale Textlänge. |
|
|  | wordCount | java.lang.Integer | Die maximale Wortanzahl. |
|
|  | isLineLimited | boolean | Der Wert, der angibt, ob die Hervorhebungsextraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Liefert die maximale Textlänge.


**Returns:**
java.lang.Integer - Ein positiver ganzzahliger Wert, der die maximale Textlänge darstellt;  null  wenn die Textlänge nicht begrenzt ist.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Liefert die maximale Wortanzahl.


**Returns:**
java.lang.Integer - Ein positiver ganzzahliger Wert, der die maximale Wortanzahl darstellt;  null  wenn die Wortanzahl nicht begrenzt ist.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Liefert den Wert, der angibt, ob die Highlight‑Extraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist.


**Returns:**
boolean -  true  wenn die Hervorhebungsextraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist; andernfalls  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Setzt die maximale Textlänge.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Ein nicht‑negativer ganzzahliger Wert;  null  um die Längenbegrenzung zu entfernen. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Setzt die maximale Wortanzahl.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Ein nicht‑negativer ganzzahliger Wert;  null  um die Begrenzung der Wortanzahl zu entfernen. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Setzt den Wert, der angibt, ob die Highlight‑Extraktion durch den Anfang (oder das Ende) einer Textzeile begrenzt ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | lineLimited | boolean | true  um nach Zeilenbegrenzungen zu beschränken. |
|

