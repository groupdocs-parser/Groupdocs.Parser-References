---
title: "DocumentPageData"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar data för dokumentsidan."
type: docs
weight: 12
url: /sv/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Representerar data för dokumentsidan. Den består av [FieldData](../../com.groupdocs.parser.data/fielddata) objekt som innehåller fältdata från dokumentsidan.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Initierar en ny instans av klassen [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Hämtar sidindexet. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Initierar en ny instans av klassen [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | fields | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | Samlingen av fältdata. |
|
|  | pageIndex | int | Det nollbaserade sidindexet. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Hämtar sidindexet.


**Returns:**
int - Ett nollbaserat index för sidan.

