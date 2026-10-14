---
title: "PageTextArea"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett sidområde för text som används för att representera ett textvärde i funktionaliteten för parsning med mall eller formulärparsning."
type: docs
weight: 24
url: /sv/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Representerar ett sidområde för text som används för att representera ett textvärde i funktionaliteten för parsning med mall eller formulärparsning.

En instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) används som returvärde för följande metoder:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Även en instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) används som värde för egenskapen [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

Se användningsexemplen där.

Textområdet kan vara enkelt eller sammansatt. I det första fallet innehåller det en text som är avgränsad av ett rektangulärt område.
I det andra fallet innehåller det andra textområden; text- och tabellegenskaper beräknas av underordnade textområden.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Initierar en ny instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getText()](#getText--) | Hämtar texten. |
|
|  | [getBaseLine()](#getBaseLine--) | Hämtar baslinjen. |
|
|  | [getTextStyle()](#getTextStyle--) | Hämtar textstilen såsom teckenstorlek, teckensnittsnamn och så vidare. |
|
|  | [getAreas()](#getAreas--) | Hämtar samlingen av underordnade textsidområden. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | text | java.lang.String | Värdet av texten. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller textområdet. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller textområdet. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | text | java.lang.String | Värdet av texten. |
|
|  | baseLine | java.lang.Double | Baslinjen för texten. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Stilen på texten. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller textområdet. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller textområdet. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Initierar en ny instans av klassen [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | områden | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Samlingen av underordnade textsidområden. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller textområdet. |
|

### getText() {#getText--}
```
public String getText()
```


Hämtar texten.


**Returns:**
java.lang.String - Ett strängvärde som representerar ett värde för textsidområdet.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Hämtar baslinjen.


**Returns:**
double - Ett dubbelvärde som representerar baslinjen.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Hämtar textstilen såsom teckenstorlek, teckensnittsnamn och så vidare.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Hämtar samlingen av underordnade textsidområden.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - En samling av underordnade textsidområden; tom om textsidområdet inte har några barn.

