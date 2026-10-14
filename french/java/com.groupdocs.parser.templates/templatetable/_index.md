---
title: "TemplateTable"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit la table de modèle."
type: docs
weight: 20
url: /fr/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Fournit la table de modèle.

Il existe deux manières de définir une table :

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) avec le nom en MAJUSCULE. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) avec le nom en MAJUSCULE. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) avec le nom en MAJUSCULE. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getLayout()](#getLayout--) | Obtient la disposition de la table. |
|
|  | [getParameters()](#getParameters--) | Obtient les paramètres pour détecter la table en mode automatique. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) avec le nom en MAJUSCULE.

La table modèle est définie par la disposition de la table si la table ne peut pas être détectée automatiquement :

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposition de la table. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) avec le nom en MAJUSCULE.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposition de la table. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|
|  | pageWidth | java.lang.Double | La largeur de la page qui a été utilisée pour créer l'élément modèle. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposition de la table. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|
|  | useUpperCaseName | boolean | La valeur qui indique si un  name  est converti en MAJUSCULE. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | La disposition de la table. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|
|  | pageWidth | java.lang.Double | La largeur de la page qui a été utilisée pour créer l'élément modèle. |
|
|  | useUpperCaseName | boolean | La valeur qui indique si un  name  est converti en MAJUSCULE. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable) avec le nom en MAJUSCULE.

Si une table modèle est définie par les paramètres du détecteur, la table est détectée automatiquement :

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Les paramètres pour détecter la table en mode automatique. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Les paramètres pour détecter la table en mode automatique. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|
|  | pageWidth | java.lang.Double | La largeur de la page qui a été utilisée pour créer l'élément modèle. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Les paramètres pour détecter la table en mode automatique. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|
|  | useUpperCaseName | boolean | La valeur qui indique si un  name  est converti en MAJUSCULE. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialise une nouvelle instance de la classe [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Les paramètres pour détecter la table en mode automatique. |
|
|  | nom | java.lang.String | Le nom de la table. |
|
|  | pageIndex | java.lang.Integer | L'index de la page où se trouve la table modèle ;  null  si la table modèle se trouve sur n'importe quelle page. |
|
|  | pageWidth | java.lang.Double | La largeur de la page qui a été utilisée pour créer l'élément modèle. |
|
|  | useUpperCaseName | boolean | La valeur qui indique si un  name  est converti en MAJUSCULE. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Obtient la disposition de la table.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Obtient les paramètres pour détecter la table en mode automatique.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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
