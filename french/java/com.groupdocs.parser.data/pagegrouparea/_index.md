---
title: "PageGroupArea"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente un groupe de zones de page utilisé pour regrouper différents types de blocs de la page du document dans la fonctionnalité d'analyse par modèle."
type: docs
weight: 19
url: /fr/java/com.groupdocs.parser.data/pagegrouparea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageGroupArea extends PageArea
```

Représente un groupe de zones de page utilisé pour regrouper différents types de blocs de la page du document dans la fonctionnalité d'analyse par modèle.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageGroupArea(Iterable<PageArea> areas, Page page)](#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-) | Initialise une nouvelle instance de la classe [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getAreas()](#getAreas--) | Obtient la collection des zones de page groupées. |
|
### PageGroupArea(Iterable<PageArea> areas, Page page) {#PageGroupArea-java.lang.Iterable-com.groupdocs.parser.data.PageArea--com.groupdocs.parser.data.Page-}
```
public PageGroupArea(Iterable<PageArea> areas, Page page)
```


Initialise une nouvelle instance de la classe [PageGroupArea](../../com.groupdocs.parser.data/pagegrouparea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | zones | java.lang.Iterable<com.groupdocs.parser.data.PageArea> | La collection des zones de page à regrouper. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient la zone. |
|

### getAreas() {#getAreas--}
```
public Iterable<PageArea> getAreas()
```


Obtient la collection des zones de page groupées.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageArea> - Une collection d'objets [PageArea](../../com.groupdocs.parser.data/pagearea).

