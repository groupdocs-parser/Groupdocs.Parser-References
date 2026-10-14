---
title: "PageTableAreaOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för extrahering av sidtabellområden."
type: docs
weight: 31
url: /sv/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Tillhandahåller de alternativ som används för extrahering av sidtabellområden.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Initierar en ny instans av klassen [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) med en sökrektangel och utan fast layout. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Hämtar tabelllayouten som definierar tabellen på en sida. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Initierar en ny instans av klassen [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tabelllayouten som definierar tabellen på en sida. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Initierar en ny instans av klassen [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) med en sökrektangel och utan fast layout.

Användbart för att begränsa automatiskt upptäckta tabeller till ett område på sidan. Speglar C#

new PageTableAreaOptions(null) { Rectangle = ... }
mönster.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området på sidan där tabeller ska upptäckas; skicka  null  för att söka på hela sidan. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Hämtar tabelllayouten som definierar tabellen på en sida.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

