---
title: "TemplateBarcode"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt het sjabloon barcode-veld."
type: docs
weight: 11
url: /nl/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Biedt het sjabloon barcode-veld.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas met de HOOFDLETTERS-naam. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse met de HOOFDLETTERS-naam. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op dat het sjabloonbarcodeveld bevat. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het sjabloonbarcodeveld bevat. |
|
|  | naam | java.lang.String | De naam van het barcodeveld. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) clas met de HOOFDLETTERS-naam.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het sjabloonbarcodeveld bevat. |
|
|  | naam | java.lang.String | De naam van het barcodeveld. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse met de HOOFDLETTERS-naam.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het sjabloonbarcodeveld bevat. |
|
|  | naam | java.lang.String | De naam van het barcodeveld. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het sjabloonbarcodeveld bevat. |
|
|  | naam | java.lang.String | De naam van het barcodeveld. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het sjabloonbarcodeveld bevat. |
|
|  | naam | java.lang.String | De naam van het barcodeveld. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op dat het sjabloonbarcodeveld bevat.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Maakt een kopie van het huidige item waarbij alle coördinaten worden geschaald met de opgegeven factor.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
