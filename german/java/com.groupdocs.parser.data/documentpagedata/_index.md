---
title: "DocumentPageData"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt Daten der Dokumentseite dar."
type: docs
weight: 12
url: /de/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Stellt Daten der Dokumentseite dar. Sie besteht aus [FieldData](../../com.groupdocs.parser.data/fielddata)-Objekten, die Felddaten der Dokumentseite enthalten.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Initialisiert eine neue Instanz der Klasse [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Liefert den Seitenindex. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Initialisiert eine neue Instanz der Klasse [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Felder | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | Die Sammlung von Felddaten. |
|
|  | pageIndex | int | Der nullbasierte Seitenindex. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Liefert den Seitenindex.


**Returns:**
int – Ein nullbasierter Index der Seite.

