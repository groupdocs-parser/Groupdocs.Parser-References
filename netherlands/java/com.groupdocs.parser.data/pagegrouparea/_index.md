---
title: "PageGroupArea"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een groep paginagebieden voor die wordt gebruikt om verschillende soorten blokken van de documentpagina te groeperen in de functionaliteit voor parsing op basis van sjablonen."
type: docs
weight: 19
url: /nl/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Stelt een groep paginagebieden voor die wordt gebruikt om verschillende soorten blokken van de documentpagina te groeperen in de functionaliteit voor parsing op basis van sjablonen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Initialiseert een nieuw exemplaar van de [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getAreas()](#getAreas--) | Haalt de verzameling van gegroepeerde pagina‑gebieden op. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Initialiseert een nieuw exemplaar van de [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | De verzameling van pagina‑gebieden die gegroepeerd moeten worden. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die het gebied bevat. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Haalt de verzameling van gegroepeerde pagina‑gebieden op.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - Een verzameling van [PageArea](../../com.groupdocs.parser.data/pagearea) objecten.

