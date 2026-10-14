---
title: "PageTableAreaOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'extraction des zones de tableau de page."
type: docs
weight: 31
url: /fr/java/com.groupdocs.parser.options/pagetableareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTableAreaOptions extends PageAreaOptions
```

Fournit les options utilisées pour l'extraction des zones de tableau de page.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageTableAreaOptions(TemplateTableLayout tableLayout)](#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-) | Initialise une nouvelle instance de la classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions). |
|
|  | [PageTableAreaOptions(Rectangle rectangle)](#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) avec un rectangle de recherche et aucune mise en page fixe. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getTableLayout()](#getTableLayout--) | Obtient la disposition du tableau qui définit le tableau sur une page. |
|
### PageTableAreaOptions(TemplateTableLayout tableLayout) {#PageTableAreaOptions-com.groupdocs.parser.templates.TemplateTableLayout-}
```
public PageTableAreaOptions(TemplateTableLayout tableLayout)
```


Initialise une nouvelle instance de la classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | tableLayout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposition du tableau qui définit le tableau sur une page. |
|

### PageTableAreaOptions(Rectangle rectangle) {#PageTableAreaOptions-com.groupdocs.parser.data.Rectangle-}
```
public PageTableAreaOptions(Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageTableAreaOptions](../../com.groupdocs.parser.options/pagetableareaoptions) avec un rectangle de recherche et aucune mise en page fixe.

Utile pour restreindre les tables détectées automatiquement à une région de la page. Reflète le C#

new PageTableAreaOptions(null) { Rectangle = ... }
modèle.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire sur la page où les tables doivent être détectées ; passez  null  pour rechercher sur toute la page. |
|

### getTableLayout() {#getTableLayout--}
```
public TemplateTableLayout getTableLayout()
```


Obtient la disposition du tableau qui définit le tableau sur une page.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instane of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class.

