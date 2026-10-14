---
title: "DocumentPageData"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de gegevens van de documentpagina voor."
type: docs
weight: 12
url: /nl/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Stelt de gegevens van de documentpagina voor. Het bestaat uit [FieldData](../../com.groupdocs.parser.data/fielddata) objecten die veldgegevens van de documentpagina bevatten.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Initialiseert een nieuw exemplaar van de [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Haalt het paginanummer op. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Initialiseert een nieuw exemplaar van de [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | velden | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | De verzameling van veldgegevens. |
|
|  | pageIndex | int | De nulgebaseerde page index. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Haalt het paginanummer op.


**Returns:**
int - Een nulgebaseerde index van de pagina.

