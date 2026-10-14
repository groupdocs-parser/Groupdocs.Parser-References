---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Handler für OCR-Ereignisse bereit."
type: docs
weight: 26
url: /de/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Stellt einen Handler für OCR-Ereignisse bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Initialisiert eine neue Instanz der [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Gibt eine Liste von Warnmeldungen zurück. |
|
|  | [hasWarnings()](#hasWarnings--) | Gibt den Wert zurück, der angibt, ob die Liste der Warnungen nicht leer ist. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Gibt eine Liste von Warnmeldungen für die Seite mit  pageIndex  zurück. |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Setzt Warnmeldungen für die Seite. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Initialisiert eine neue Instanz der [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) Klasse.


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Gibt eine Liste von Warnmeldungen zurück.


**Returns:**
java.util.List<java.lang.String> - Eine Liste von Warnmeldungen für alle Seiten.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Gibt den Wert zurück, der angibt, ob die Liste der Warnungen nicht leer ist.


**Returns:**
boolean -  true  wenn die Liste der Warnungen nicht leer ist; andernfalls  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Gibt eine Liste von Warnmeldungen für die Seite mit  pageIndex  zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

**Returns:**
java.util.List<java.lang.String> - Eine Liste von Warnmeldungen für die Seite; leere Liste, wenn keine Warnmeldungen für die Seite vorhanden sind.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Setzt Warnmeldungen für die Seite.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | Die Liste der Warnmeldungen für die Seite. |
|

