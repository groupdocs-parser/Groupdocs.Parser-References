---
title: "Seite"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Informationen der Dokumentseite dar, wie Seitenindex und Seitengröße."
type: docs
weight: 16
url: /de/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Stellt die Dokumentseiteninformationen wie Seitenindex und Seitengröße dar. Sie wird verwendet, um die Seite zu repräsentieren, die Erben der Klasse [PageArea](../../com.groupdocs.parser.data/pagearea) im Parsing‑nach‑Vorlage‑Funktionalität enthält.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Initialisiert eine neue Instanz der Klasse [Page](../../com.groupdocs.parser.data/page). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getIndex()](#getIndex--) | Liefert den Seitenindex. |
|
|  | [getSize()](#getSize--) | Ruft die Seitengröße ab. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Initialisiert eine neue Instanz der Klasse [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der Seitenindex. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Die Seitengröße. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Liefert den Seitenindex.


**Returns:**
int – Ein nullbasierter Index der Seite.

### getSize() {#getSize--}
```
public Size getSize()
```


Ruft die Seitengröße ab.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

