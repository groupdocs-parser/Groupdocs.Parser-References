---
title: "DocumentPageData"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les données de la page du document."
type: docs
weight: 12
url: /fr/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Représente les données de la page du document. Elle se compose d'objets [FieldData](../../com.groupdocs.parser.data/fielddata) qui contiennent les données de champ de la page du document.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Initialise une nouvelle instance de la classe [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Obtient l'indice de page. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Initialise une nouvelle instance de la classe [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | champs | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | La collection des données des champs. |
|
|  | pageIndex | int | L'index de page basé sur zéro. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtient l'indice de page.


**Returns:**
int - Un index de page basé sur zéro.

