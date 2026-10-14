---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt een handler voor OCR-gebeurtenissen."
type: docs
weight: 26
url: /nl/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Biedt een handler voor OCR-gebeurtenissen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Initialiseert een nieuw exemplaar van de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Haalt een lijst met waarschuwingsberichten op. |
|
|  | [hasWarnings()](#hasWarnings--) | Haalt de waarde op die aangeeft of de lijst met waarschuwingen niet leeg is. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Retourneert een lijst met waarschuwingsberichten voor de pagina met pageIndex. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Stelt waarschuwingsberichten in voor de pagina. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Initialiseert een nieuw exemplaar van de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) klasse.


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Haalt een lijst met waarschuwingsberichten op.


**Returns:**
java.util.List<java.lang.String> - Een lijst met waarschuwingsberichten voor alle pagina's.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Haalt de waarde op die aangeeft of de lijst met waarschuwingen niet leeg is.


**Returns:**
boolean -  true  als de lijst met waarschuwingen niet leeg is; anders,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Retourneert een lijst met waarschuwingsberichten voor de pagina met pageIndex.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|

**Returns:**
java.util.List<java.lang.String> - Een lijst met waarschuwingsberichten voor de pagina; lege lijst als er geen waarschuwingsberichten voor de pagina zijn.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Stelt waarschuwingsberichten in voor de pagina.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pageIndex | int | De nulgebaseerde page index. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | De lijst met waarschuwingsberichten voor de pagina. |
|

