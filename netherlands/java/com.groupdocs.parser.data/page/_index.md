---
title: "Page"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de paginainformatie van het document voor, zoals paginanummer en paginagrootte."
type: docs
weight: 16
url: /nl/java/com.groupdocs.parser.data/page/
---
**Inheritance:**
java.lang.Object
```
public class Page
```

Stelt de paginainformatie van het document voor, zoals paginanummer en paginagrootte. Het wordt gebruikt om de pagina weer te geven die overervingen van de [PageArea](../../com.groupdocs.parser.data/pagearea) klasse bevat in de parsing‑op‑sjabloon functionaliteit.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Page(int index, Size size)](#Page-int-com.groupdocs.parser.data.Size-) | Initialiseert een nieuw exemplaar van de [Page](../../com.groupdocs.parser.data/page) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getIndex()](#getIndex--) | Haalt het paginanummer op. |
|
|  | [getSize()](#getSize--) | Haalt de paginagrootte op. |
|
### Page(int index, Size size) {#Page-int-com.groupdocs.parser.data.Size-}
```
public Page(int index, Size size)
```


Initialiseert een nieuw exemplaar van de [Page](../../com.groupdocs.parser.data/page) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | Het paginanummer. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | De paginagrootte. |
|

### getIndex() {#getIndex--}
```
public int getIndex()
```


Haalt het paginanummer op.


**Returns:**
int - Een nulgebaseerde index van de pagina.

### getSize() {#getSize--}
```
public Size getSize()
```


Haalt de paginagrootte op.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the page.

