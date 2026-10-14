---
title: "PageArea"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en abstrakt basklass för sidområden som används för att representera block på dokumentsidan i funktionaliteten för parsning med mall."
type: docs
weight: 17
url: /sv/java/com.groupdocs.parser.data/pagearea/
---
**Inheritance:**
java.lang.Object
```
public abstract class PageArea
```

Representerar en abstrakt basklass för sidområden som används för att representera block på dokumentsidan i funktionaliteten för parsning med mall.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området. |
|
|  | [getPage()](#getPage--) | Hämtar dokumentets sidinformation såsom sidindex och sidstorlek. |
|
### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area of the page that contains the page area.

### getPage() {#getPage--}
```
public Page getPage()
```


Hämtar dokumentets sidinformation såsom sidindex och sidstorlek.


**Returns:**
[Page](../../com.groupdocs.parser.data/page) - An instance of [Page](../../com.groupdocs.parser.data/page) class that represents the page that contains the page area.

