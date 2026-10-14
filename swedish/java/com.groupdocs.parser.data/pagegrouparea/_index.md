---
title: "PageGroupArea"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en grupp av sidområden som används för att gruppera olika typer av block på dokumentsidan i funktionaliteten för parsning med mall."
type: docs
weight: 19
url: /sv/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Representerar en grupp av sidområden som används för att gruppera olika typer av block på dokumentsidan i funktionaliteten för parsning med mall.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Initierar en ny instans av klassen [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getAreas()](#getAreas--) | Hämtar samlingen av grupperade sidområden. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Initierar en ny instans av klassen [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | områden | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | Samlingen av sidområden som ska grupperas. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller området. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Hämtar samlingen av grupperade sidområden.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - En samling av [PageArea](../../com.groupdocs.parser.data/pagearea) objekt.

