---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller en hanterare för OCR-händelser."
type: docs
weight: 26
url: /sv/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Tillhandahåller en hanterare för OCR-händelser.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Initierar en ny instans av klassen [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Hämtar en lista med varningsmeddelanden. |
|
|  | [hasWarnings()](#hasWarnings--) | Hämtar värdet som indikerar om listan med varningar inte är tom. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Returnerar en lista med varningsmeddelanden för sidan med  pageIndex . |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Ställer in varningsmeddelanden för sidan. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Initierar en ny instans av klassen [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Hämtar en lista med varningsmeddelanden.


**Returns:**
java.util.List<java.lang.String> - En lista med varningsmeddelanden för alla sidor.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Hämtar värdet som indikerar om listan med varningar inte är tom.


**Returns:**
boolean -  true  om listan med varningar inte är tom; annars,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Returnerar en lista med varningsmeddelanden för sidan med  pageIndex .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

**Returns:**
java.util.List<java.lang.String> - En lista med varningsmeddelanden för sidan; tom lista om inga varningsmeddelanden finns för sidan.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Ställer in varningsmeddelanden för sidan.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pageIndex | int | Det nollbaserade sidindexet. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | Listan med varningsmeddelanden för sidan. |
|

