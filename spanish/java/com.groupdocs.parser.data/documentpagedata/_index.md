---
title: "DocumentPageData"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa los datos de la página del documento."
type: docs
weight: 12
url: /es/java/com.groupdocs.parser.data/documentpagedata/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.DocumentData](../../com.groupdocs.parser.data/documentdata)
```
public class DocumentPageData extends DocumentData
```

Representa los datos de la página del documento. Consiste en objetos [FieldData](../../com.groupdocs.parser.data/fielddata) que contienen datos de campo de la página del documento.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [DocumentPageData(Iterable<FieldData> fields, int pageIndex)](#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-) | Inicializa una nueva instancia de la clase [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getPageIndex()](#getPageIndex--) | Obtiene el índice de página. |
|
### DocumentPageData(Iterable<FieldData> fields, int pageIndex) {#DocumentPageData-java.lang.Iterable-com.groupdocs.parser.data.FieldData--int-}
```
public DocumentPageData(Iterable<FieldData> fields, int pageIndex)
```


Inicializa una nueva instancia de la clase [DocumentPageData](../../com.groupdocs.parser.data/documentpagedata).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | campos | java.lang.Iterable<com.groupdocs.parser.data.FieldData> | La colección de datos de campos. |
|
|  | pageIndex | int | El índice de página basado en cero. |
|

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtiene el índice de página.


**Returns:**
int - Un índice basado en cero de la página.

