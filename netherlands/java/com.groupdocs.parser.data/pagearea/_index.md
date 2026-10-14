---
title: "PageArea"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een abstracte basisklasse voor paginagebieden voor die worden gebruikt om blokken op de documentpagina te representeren in de functionaliteit voor parsing op basis van sjablonen."
type: docs
weight: 17
url: /nl/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Stelt een abstracte basisklasse voor paginagebieden voor die worden gebruikt om blokken op de documentpagina te representeren in de functionaliteit voor parsing op basis van sjablonen.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op. |
|
|  | [getPage()](#getPage--) | Haalt de paginainformatie van het document op, zoals paginanummer en paginagrootte. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Haalt de paginainformatie van het document op, zoals paginanummer en paginagrootte.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

