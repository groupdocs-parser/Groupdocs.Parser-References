---
title: "PageArea"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt eine abstrakte Basisklasse für Seitenbereiche dar, die verwendet wird, um Blöcke auf der Dokumentseite in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren."
type: docs
weight: 17
url: /de/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Stellt eine abstrakte Basisklasse für Seitenbereiche dar, die verwendet wird, um Blöcke auf der Dokumentseite in der Vorlagen‑Parsing‑Funktionalität zu repräsentieren.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Liefert den rechteckigen Bereich. |
|
|  | [getPage()](#getPage--) | Ruft die Dokumentseiteninformationen wie Seitenindex und Seitengröße ab. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Liefert den rechteckigen Bereich.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Ruft die Dokumentseiteninformationen wie Seitenindex und Seitengröße ab.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

