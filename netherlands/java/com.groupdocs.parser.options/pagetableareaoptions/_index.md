---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor het extraheren van paginatabelgebieden."
type: docs
weight: 31
url: /nl/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Biedt de opties die worden gebruikt voor het extraheren van paginatabelgebieden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Initialiseert een nieuw exemplaar van de klasse [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuw exemplaar van de klasse [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) met een zoekrechthoek en zonder vaste lay-out. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Haalt de tabelindeling op die de tabel op een pagina definieert. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Initialiseert een nieuw exemplaar van de klasse [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | De tabelindeling die de tabel op een pagina definieert. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van de klasse [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) met een zoekrechthoek en zonder vaste lay-out.

Handig om automatisch gedetecteerde tabellen te beperken tot een regio van de pagina. Spiegelt de C#.

new PageTableAreaOptions(null) { Rectangle = ... }
patroon.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied op de pagina waar tabellen moeten worden gedetecteerd; geef  null  door om de hele pagina te doorzoeken. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Haalt de tabelindeling op die de tabel op een pagina definieert.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

