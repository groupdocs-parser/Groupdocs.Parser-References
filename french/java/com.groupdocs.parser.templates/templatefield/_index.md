---
title: "TemplateField"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit le champ de texte du modèle."
type: docs
weight: 12
url: /fr/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Fournit le champ de texte du modèle.

Les champs texte sont définis par leur position sur la page. Il existe trois façons de définir un champ texte :

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield) avec le nom EN MAJUSCULES. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield) avec le nom EN MAJUSCULES. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getPosition()](#getPosition--) | Obtient la valeur qui décrit comment trouver le champ du modèle sur la page du document. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La position du champ. |
|
|  | nom | java.lang.String | Le nom du champ. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield) avec le nom EN MAJUSCULES.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La position du champ. |
|
|  | nom | java.lang.String | Le nom du champ. |
|
|  | pageIndex | java.lang.Integer | Une valeur entière qui représente l'index de la page où l'élément du modèle est situé ;  null  si l'élément du modèle se trouve sur n'importe quelle page. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield) avec le nom EN MAJUSCULES.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La position du champ. |
|
|  | nom | java.lang.String | Le nom du champ. |
|
|  | pageIndex | java.lang.Integer | Une valeur entière qui représente l'index de la page où l'élément du modèle est situé ;  null  si l'élément du modèle se trouve sur n'importe quelle page. |
|
|  | pageWidth | java.lang.Double | La largeur de la page qui a été utilisée pour créer l'élément modèle. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La position du champ. |
|
|  | nom | java.lang.String | Le nom du champ. |
|
|  | pageIndex | java.lang.Integer | Une valeur entière qui représente l'index de la page où l'élément du modèle est situé ;  null  si l'élément du modèle se trouve sur n'importe quelle page. |
|
|  | useUpperCaseName | boolean | La valeur qui indique si un  name  est converti en MAJUSCULE. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialise une nouvelle instance de la classe [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | La position du champ. |
|
|  | nom | java.lang.String | Le nom du champ. |
|
|  | pageIndex | java.lang.Integer | Une valeur entière qui représente l'index de la page où l'élément du modèle est situé ;  null  si l'élément du modèle se trouve sur n'importe quelle page. |
|
|  | pageWidth | java.lang.Double | La largeur de la page qui a été utilisée pour créer l'élément modèle. |
|
|  | useUpperCaseName | boolean | La valeur qui indique si un  name  est converti en MAJUSCULE. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Obtient la valeur qui décrit comment trouver le champ du modèle sur la page du document.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Crée une copie de l'élément actuel avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
