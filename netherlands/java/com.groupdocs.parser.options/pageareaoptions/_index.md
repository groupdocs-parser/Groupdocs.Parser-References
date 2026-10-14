---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor het extraheren van paginagebieden."
type: docs
weight: 28
url: /nl/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Biedt de opties die worden gebruikt voor het extraheren van paginagebieden.

Een instantie van de [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) klasse wordt gebruikt als parameter in [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
en [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-) methoden. Zie daar de gebruiksvoorbeelden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuwe instantie van de [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) klasse met de grootte van de genegeerde rand. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Initialiseert een nieuwe instantie van de [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op dat pagina‑gebieden bevat. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Haalt de grootte van de rand op die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Initialiseert een nieuwe instantie van de [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) klasse met de grootte van de genegeerde rand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat pagina‑gebieden bevat. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Initialiseert een nieuwe instantie van de [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat pagina‑gebieden bevat. |
|
|  | rectangleTolerance | double | De grootte van de rand die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Deze wordt gemeten als een fractie van de hoogte van een tekstelement. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op dat pagina‑gebieden bevat.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Haalt de grootte van de rand op die wordt genegeerd wanneer deze wordt vastgelegd door het rechthoekige gebied. Deze wordt gemeten als een fractie van de hoogte van een tekstelement.


**Returns:**
double - De double‑waarde van 0 (geen rand) tot 1 (negeer het hele element).

