---
title: "TemplateTable"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Vorlagentabelle bereit."
type: docs
weight: 20
url: /de/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Stellt die Vorlagentabelle bereit.

Es gibt zwei Möglichkeiten, eine Tabelle zu definieren:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) mit dem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) mit dem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) mit dem GROSSBUCHSTABEN-Namen. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getLayout()](#getLayout--) | Gibt das Tabellenlayout zurück. |
|
|  | [getParameters()](#getParameters--) | Gibt die Parameter zurück, um die Tabelle im automatischen Modus zu erkennen. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) mit dem GROSSBUCHSTABEN-Namen.

Die Tabellenvorlage wird über das Tabellenlayout festgelegt, wenn die Tabelle nicht automatisch erkannt werden kann:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Das Tabellenlayout. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) mit dem GROSSBUCHSTABEN-Namen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Das Tabellenlayout. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Das Tabellenlayout. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Das Tabellenlayout. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable) mit dem GROSSBUCHSTABEN-Namen.

Wenn eine Vorlagentabelle durch Detektorparameter festgelegt wird, wird die Tabelle automatisch erkannt:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Die Parameter, um die Tabelle im automatischen Modus zu erkennen. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Die Parameter, um die Tabelle im automatischen Modus zu erkennen. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Die Parameter, um die Tabelle im automatischen Modus zu erkennen. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initialisiert eine neue Instanz der Klasse [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Die Parameter, um die Tabelle im automatischen Modus zu erkennen. |
|
|  | Name | java.lang.String | Der Tabellenname. |
|
|  | pageIndex | java.lang.Integer | Der Index der Seite, auf der die Vorlagentabelle positioniert ist;  null  wenn die Vorlagentabelle auf einer beliebigen Seite liegt. |
|
|  | pageWidth | java.lang.Double | Die Breite der Seite, die zur Erstellung des Vorlagen-Elements verwendet wurde. |
|
|  | useUpperCaseName | boolean | Der Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN umgewandelt wird. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Gibt das Tabellenlayout zurück.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Gibt die Parameter zurück, um die Tabelle im automatischen Modus zu erkennen.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Erstellt eine Kopie des aktuellen Elements, wobei alle Koordinaten um den angegebenen Faktor skaliert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Faktor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
