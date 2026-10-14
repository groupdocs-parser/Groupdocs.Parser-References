---
title: "HighlightOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt om een markering van een tekstblok rond gevonden tekst in zoekscenario's te extraheren."
type: docs
weight: 22
url: /nl/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Biedt de opties die worden gebruikt om een markering te extraheren (een blok tekst rond gevonden tekst in zoekscenario's).

Een instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse wordt gebruikt als parameter in de [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-) methode.
Zie daar de gebruiksvoorbeelden.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse zonder ingestelde limieten. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse die wordt gebruikt om een markering met vaste lengte te extraheren. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse die wordt gebruikt om een regel-beperkte markering te extraheren. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse die wordt gebruikt om een markering met een vast aantal woorden te extraheren. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Haalt een maximale tekstlengte op. |
|
|  | [getWordCount()](#getWordCount--) | Haalt een maximaal aantal woorden op. |
|
|  | [isLineLimited()](#isLineLimited--) | Haalt de waarde op die aangeeft of markeringsextractie beperkt is door het begin (of het einde) van een tekstregel. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Stelt een maximale tekstlengte in. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Stelt een maximaal aantal woorden in. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Stelt de waarde in die aangeeft of markeringsextractie beperkt is door het begin (of het einde) van een tekstregel. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse zonder ingestelde limieten. Stel minstens één van #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) in voordat u deze aan de parser doorgeeft.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse die wordt gebruikt om een markering met vaste lengte te extraheren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | maxLength | int | De maximale tekstlengte. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse die wordt gebruikt om een regel-beperkte markering te extraheren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | De maximale tekstlengte. |
|
|  | isLineLimited | boolean | De waarde die aangeeft of de markeringsextractie beperkt is door het begin (of het einde) van een tekstregel. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse die wordt gebruikt om een markering met een vast aantal woorden te extraheren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | De maximale tekstlengte. |
|
|  | wordCount | int | Het maximale aantal woorden. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Initialiseert een nieuwe instantie van de [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | De maximale tekstlengte. |
|
|  | wordCount | java.lang.Integer | Het maximale aantal woorden. |
|
|  | isLineLimited | boolean | De waarde die aangeeft of de markeringsextractie beperkt is door het begin (of het einde) van een tekstregel. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Haalt een maximale tekstlengte op.


**Returns:**
java.lang.Integer - Een positieve gehele waarde die de maximale tekstlengte vertegenwoordigt;  null  als de tekstlengte niet beperkt is.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Haalt een maximaal aantal woorden op.


**Returns:**
java.lang.Integer - Een positieve gehele waarde die het maximale aantal woorden vertegenwoordigt;  null  als het aantal woorden niet beperkt is.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Haalt de waarde op die aangeeft of markeringsextractie beperkt is door het begin (of het einde) van een tekstregel.


**Returns:**
boolean -  true  als markeringsextractie beperkt is door het begin (of het einde) van een tekstregel; anders,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Stelt een maximale tekstlengte in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Een niet-negatief geheel getal;  null  om de lengtelimiet te verwijderen. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Stelt een maximaal aantal woorden in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Een niet-negatief geheel getal;  null  om de limiet op het aantal woorden te verwijderen. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Stelt de waarde in die aangeeft of markeringsextractie beperkt is door het begin (of het einde) van een tekstregel.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | lineLimited | boolean | true  om te beperken tot de lijngrenzen. |
|

