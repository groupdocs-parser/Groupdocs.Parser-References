---
title: "BarcodeOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'extraction de codes-barres."
type: docs
weight: 10
url: /fr/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Fournit les options utilisées pour l'extraction de codes-barres.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Initialise une nouvelle instance de la classe BarcodeOptions avec les valeurs par défaut. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe BarcodeOptions avec la zone rectangulaire. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Initialise une nouvelle instance de la classe BarcodeOptions avec les paramètres de qualité et les types de code. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Initialise une nouvelle instance de la classe BarcodeOptions. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Obtient la valeur qui indique si les codes-barres incorrects sont autorisés. |
|
|  | [getDimension()](#getDimension--) | Obtient la taille minimale de l'élément minimal du code-barres. |
|
|  | [getImageQuality()](#getImageQuality--) | Obtient la qualité d'une image source. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Obtient la qualité d'un code-barres source. |
|
|  | [getRectangle()](#getRectangle--) | Obtient la zone rectangulaire qui contient les zones de page. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Obtient les types de codes-barres à lire. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Définit la valeur qui indique si les codes-barres incorrects sont autorisés. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Définit la taille minimale de l'élément minimal du code-barres. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Définit la qualité d'une image source. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Définit la qualité d'un code-barres source. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Définit la zone rectangulaire qui contient les codes-barres. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Définit les types de codes-barres à lire. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Initialise une nouvelle instance de la classe BarcodeOptions avec les valeurs par défaut.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Initialise une nouvelle instance de la classe BarcodeOptions avec la zone rectangulaire.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les codes-barres. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Initialise une nouvelle instance de la classe BarcodeOptions avec les paramètres de qualité et les types de code.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualité d'une image source. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualité d'un code-barres source. |
|
|  | codeTypes | java.lang.String[] | Les types de codes-barres à lire. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Initialise une nouvelle instance de la classe BarcodeOptions.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les codes-barres. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualité d'une image source. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | La qualité d'un code-barres source. |
|
|  | dimension | java.lang.Float | La taille minimale de l'élément minimal du code-barres. |
|
|  | allowIncorrectBarcodes | boolean | La valeur qui indique si les codes-barres incorrects sont autorisés. |
|
|  | codeTypes | java.lang.String[] | Les types de codes-barres à lire. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Obtient la valeur qui indique si les codes-barres incorrects sont autorisés.


**Returns:**
booléen -  true  si les codes-barres incorrects sont autorisés ; sinon,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Obtient la taille minimale de l'élément minimal du code-barres.


**Returns:**
java.lang.Float - La valeur flottante qui représente l'élément minimal du code-barres ;  null  si le mode automatique est utilisé.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Obtient la qualité d'une image source.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Obtient la qualité d'un code-barres source.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtient la zone rectangulaire qui contient les zones de page.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Obtient les types de codes-barres à lire.


**Returns:**
java.util.List<java.lang.String> - La collection en lecture seule qui contient des types de codes-barres à lire ; collection vide si elle n'est pas définie.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Définit la valeur qui indique si les codes-barres incorrects sont autorisés.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  si les codes-barres incorrects sont autorisés. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Définit la taille minimale de l'élément minimal du code-barres.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | dimension | java.lang.Float | L'élément minimal du code-barres ;  null  pour le mode automatique. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Définit la qualité d'une image source.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Le mode de qualité de l'image. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Définit la qualité d'un code-barres source.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Le mode de qualité du code-barres. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Définit la zone rectangulaire qui contient les codes-barres.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire ;  null  pour analyser toute la page. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Définit les types de codes-barres à lire.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Les types de codes-barres; null ou vide pour tous les types. |
|

