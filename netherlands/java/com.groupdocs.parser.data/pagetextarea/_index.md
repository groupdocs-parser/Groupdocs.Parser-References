---
title: "PageTextArea"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een paginatekstgebied voor dat wordt gebruikt om een tekstwaarde te representeren in de functionaliteit voor parsing op basis van sjablonen of formulierparsing."
type: docs
weight: 24
url: /nl/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Stelt een paginatekstgebied voor dat wordt gebruikt om een tekstwaarde te representeren in de functionaliteit voor parsing op basis van sjablonen of formulierparsing.

Een instantie van [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse wordt gebruikt als retourwaarde van de volgende methoden:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Ook een instantie van [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse wordt gebruikt als waarde van de [PageArea](../../com.groupdocs.parser.data/pagearea) eigenschap.
\*

Zie daar de gebruiksvoorbeelden.

Het tekstgebied kan enkel of samengesteld zijn. In het eerste geval bevat het een tekst die begrensd wordt door een rechthoekig gebied.
In het tweede geval bevat het andere tekstgebieden; tekst- en tabel-eigenschappen worden berekend door onderliggende tekstgebieden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuwe instantie van de [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse. |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuwe instantie van de [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse. |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Initialiseert een nieuwe instantie van de [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getText()](#getText--) | Haalt de tekst op. |
|
|  | [getBaseLine()](#getBaseLine--) | Haalt de basislijn op. |
|
|  | [getTextStyle()](#getTextStyle--) | Haalt de tekststijl op, zoals lettergrootte, lettertype enzovoort. |
|
|  | [getAreas()](#getAreas--) | Haalt de collectie van onderliggende tekstpagina-gebieden op. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Initialiseert een nieuwe instantie van de [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tekst | java.lang.String | De waarde van de tekst. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die het tekstgebied bevat. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het tekstgebied bevat. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Initialiseert een nieuwe instantie van de [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tekst | java.lang.String | De waarde van de tekst. |
|
|  | baseLine | java.lang.Double | De basislijn van de tekst. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | De stijl van de tekst. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die het tekstgebied bevat. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het tekstgebied bevat. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Initialiseert een nieuwe instantie van de [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | De collectie van onderliggende tekstpagina-gebieden. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die het tekstgebied bevat. |
|

### getText() {#getText--}
```
public String getText()
```


Haalt de tekst op.


**Returns:**
java.lang.String - Een stringwaarde die een waarde van het tekstpagina-gebied weergeeft.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Haalt de basislijn op.


**Returns:**
double - Een double-waarde die de basislijn weergeeft.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Haalt de tekststijl op, zoals lettergrootte, lettertype enzovoort.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Haalt de collectie van onderliggende tekstpagina-gebieden op.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Een collectie van onderliggende tekstpagina-gebieden; leeg als het tekstpagina-gebied geen kinderen heeft.

