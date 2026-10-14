---
title: "PageBarcodeArea"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une zone de code-barres de page utilisée pour représenter une valeur de code-barres dans la fonctionnalité d'analyse par modèle."
type: docs
weight: 18
url: /fr/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

Représente une zone de code-barres de page utilisée pour représenter une valeur de code-barres dans la fonctionnalité d'analyse par modèle.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getValue()](#getValue--) | Obtient la valeur du code-barres. |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | Obtient le nom du type de code-barres. |
|
|  | [getConfidence()](#getConfidence--) | Obtient le niveau de confiance du code-barres analysé. |
|
|  | [getAngle()](#getAngle--) | Obtient l'angle du code-barres. |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | La valeur du code-barres. |
|
|  | codeTypeName | java.lang.String | Le nom du type du code-barres. |
|
|  | confiance | int | Le niveau de confiance du code-barres analysé. |
|
|  | angle | double | L'angle du code-barres. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient la zone du code-barres. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient la zone du code-barres. |
|

### getValue() {#getValue--}
```
public String getValue()
```


Obtient la valeur du code-barres.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente une valeur de la zone de page du code-barres.

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


Obtient le nom du type de code-barres.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le nom de type du code-barres.

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


Obtient le niveau de confiance du code-barres analysé.


**Returns:**
int - Une valeur entière qui représente la confiance du code-barres analysé (0-100).

### getAngle() {#getAngle--}
```
public double getAngle()
```


Obtient l'angle du code-barres.


**Returns:**
double - Une valeur décimale qui représente l'angle du code-barres (0-360).

