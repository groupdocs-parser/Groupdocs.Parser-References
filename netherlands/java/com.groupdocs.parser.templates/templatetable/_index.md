---
title: "TemplateTable"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de sjabloontabel."
type: docs
weight: 20
url: /nl/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Biedt de sjabloontabel.

Er zijn twee manieren om een tabel te definiëren:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Initialiseert een nieuw exemplaar van de klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) met de HOOFDLETTERS-naam. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialiseert een nieuw exemplaar van de klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) met de HOOFDLETTERS-naam. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Initialiseert een nieuw exemplaar van de klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) met de HOOFDLETTERS-naam. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getLayout()](#getLayout--) | Haalt de tabelindeling op. |
|
|  | [getParameters()](#getParameters--) | Haalt de parameters op om de tabel in de automatische modus te detecteren. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Initialiseert een nieuw exemplaar van de klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) met de HOOFDLETTERS-naam.

De tabel wordt ingesteld via tabelindeling als de tabel niet automatisch kan worden gedetecteerd:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | De tabelindeling. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Initialiseert een nieuw exemplaar van de klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) met de HOOFDLETTERS-naam.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | De tabelindeling. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | De tabelindeling. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | De tabelindeling. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Initialiseert een nieuw exemplaar van de klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) met de HOOFDLETTERS-naam.

Als een sjabloontabel wordt ingesteld via detectorparameters, wordt de tabel automatisch gedetecteerd:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | De parameters om de tabel in de automatische modus te detecteren. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | De parameters om de tabel in de automatische modus te detecteren. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | De parameters om de tabel in de automatische modus te detecteren. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialiseert een nieuw exemplaar van de [TemplateTable](../../com.groupdocs.parser.templates/templatetable) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | De parameters om de tabel in de automatische modus te detecteren. |
|
|  | naam | java.lang.String | De tabelnaam. |
|
|  | pageIndex | java.lang.Integer | De index van de pagina waarop de sjabloontabel zich bevindt;  null  als de sjabloontabel zich op een willekeurige pagina bevindt. |
|
|  | pageWidth | java.lang.Double | De breedte van de pagina die werd gebruikt om het sjabloonitem te maken. |
|
|  | useUpperCaseName | boolean | De waarde die aangeeft of een  name  wordt geconverteerd naar HOOFDLETTERS. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Haalt de tabelindeling op.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Haalt de parameters op om de tabel in de automatische modus te detecteren.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

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
