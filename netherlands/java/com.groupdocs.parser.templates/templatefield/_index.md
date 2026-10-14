---
title: "TemplateField"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt het sjabloon tekstveld."
type: docs
weight: 12
url: /nl/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Biedt het sjabloon tekstveld.

Tekstvelden worden gedefinieerd op basis van hun positie op de pagina. Er zijn drie manieren om een tekstveld te definiëren:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse met de hoofdlettergevoelige naam. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse met de hoofdlettergevoelige naam. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getPosition()](#getPosition--) | Haalt de waarde op die beschrijft hoe het sjabloonveld op de documentpagina gevonden kan worden. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | De veldpositie. |
|
|  | naam | java.lang.String | De veldnaam. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse met de hoofdlettergevoelige naam.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | De veldpositie. |
|
|  | naam | java.lang.String | De veldnaam. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse met de hoofdlettergevoelige naam.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | De veldpositie. |
|
|  | naam | java.lang.String | De veldnaam. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | De veldpositie. |
|
|  | naam | java.lang.String | De veldnaam. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateField](../../com.groupdocs.parser.templates/templatefield) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | De veldpositie. |
|
|  | naam | java.lang.String | De veldnaam. |
|
|  | pageIndex | java.lang.Integer | Een geheel getal dat de index van de pagina aangeeft waarop het sjabloonitem zich bevindt; null als het sjabloonitem zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Haalt de waarde op die beschrijft hoe het sjabloonveld op de documentpagina gevonden kan worden.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

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
