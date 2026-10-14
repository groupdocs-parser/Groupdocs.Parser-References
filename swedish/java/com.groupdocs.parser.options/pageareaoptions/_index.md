---
title: "PageAreaOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för extrahering av sidområden."
type: docs
weight: 28
url: /sv/java/com.groupdocs.parser.options/pageareaoptions/
---
**Inheritance:**
java.lang.Object
```
public class PageAreaOptions
```

Tillhandahåller de alternativ som används för extrahering av sidområden.

En instans av klassen [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) används som parameter i [Parser.getImages(PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-PageAreaOptions-)
och [Parser.getImages(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getImages-int--PageAreaOptions-) metoder. Se användningsexemplen där.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageAreaOptions(Rectangle rectangle)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) med storleken på den ignorerade kanten. |
|
|  | [PageAreaOptions(Rectangle rectangle, double rectangleTolerance)](#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-) | Initierar en ny instans av klassen [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området som innehåller sidområden. |
|
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Hämtar storleken på kanten som ignoreras när den fångas av det rektangulära området. |
|
### PageAreaOptions(Rectangle rectangle) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageAreaOptions(Rectangle rectangle)
```


Initierar en ny instans av klassen [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions) med storleken på den ignorerade kanten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller sidområden. |
|

### PageAreaOptions(Rectangle rectangle, double rectangleTolerance) {#PageAreaOptions-com.groupdocs.parser.data.Rectangle-double-}
```
public PageAreaOptions(Rectangle rectangle, double rectangleTolerance)
```


Initierar en ny instans av klassen [PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller sidområden. |
|
|  | rectangleTolerance | double | Storleken på kanten som ignoreras när den fångas av det rektangulära området. Den mäts som en bråkdel av en textrads höjd. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området som innehåller sidområden.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Hämtar storleken på kanten som ignoreras när den fångas av det rektangulära området. Den mäts som en bråkdel av en textrads höjd.


**Returns:**
double - Det dubbla värdet från 0 (ingen kant) till 1 (ignorera hela elementet).

