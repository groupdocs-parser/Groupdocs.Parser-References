---
title: "Page"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar information om dokumentsidan såsom sidindex och sidstorlek."
type: docs
weight: 16
url: /sv/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Representerar dokumentets sidinformation såsom sidindex och sidstorlek. Den används för att representera sidan som innehåller arvtagare av klassen [PageArea](../../com.groupdocs.parser.data/pagearea) i parsning med mallfunktionalitet.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Initierar en ny instans av klassen [Page](../../com.groupdocs.parser.data/page). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getIndex()](#getIndex--) | Hämtar sidindexet. |
|
|  | [getSize()](#getSize--) | Hämtar sidstorleken. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Initierar en ny instans av klassen [Page](../../com.groupdocs.parser.data/page).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Sidindexet. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Sidstorleken. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar sidindexet.


**Returns:**
int - Ett nollbaserat index för sidan.

### getSize() {#getSize--}
```
public Size getSize()
```


Hämtar sidstorleken.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

