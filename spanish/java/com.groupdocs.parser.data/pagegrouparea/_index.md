---
title: "PageGroupArea"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un grupo de áreas de página que se utiliza para agrupar diferentes tipos de bloques de la página del documento en la funcionalidad de análisis mediante plantillas."
type: docs
weight: 19
url: /es/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Representa un grupo de áreas de página que se utiliza para agrupar diferentes tipos de bloques de la página del documento en la funcionalidad de análisis mediante plantillas.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Inicializa una nueva instancia de la clase [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getAreas()](#getAreas--) | Obtiene la colección de áreas de página agrupadas. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Inicializa una nueva instancia de la clase [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | areas | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | La colección de áreas de página que se agruparán. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene el área. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Obtiene la colección de áreas de página agrupadas.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - Una colección de objetos [PageArea](../../com.groupdocs.parser.data/pagearea).

