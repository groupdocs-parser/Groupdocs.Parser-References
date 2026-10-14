---
title: "PageGroupArea"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine Gruppe von Seitenbereichen dar, die verwendet wird, um verschiedene Arten von Blöcken der Dokumentseite in der Vorlagen‑Parsing‑Funktionalität zu gruppieren."
type: docs
weight: 19
url: /de/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Stellt eine Gruppe von Seitenbereichen dar, die verwendet wird, um verschiedene Arten von Blöcken der Dokumentseite in der Vorlagen‑Parsing‑Funktionalität zu gruppieren.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Initialisiert eine neue Instanz der Klasse [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getAreas()](#getAreas--) | Ruft die Sammlung gruppierter Seitenbereiche ab. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Initialisiert eine neue Instanz der Klasse [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Bereiche | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | Die Sammlung von Seitenbereichen, die gruppiert werden sollen. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die den Bereich enthält. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Ruft die Sammlung gruppierter Seitenbereiche ab.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> – Eine Sammlung von [PageArea](../../com.groupdocs.parser.data/pagearea)-Objekten.

