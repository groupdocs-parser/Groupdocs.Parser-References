---
title: "TemplateTable"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller malltabellen."
type: docs
weight: 20
url: /sv/java/com.groupdocs.parser.templates/templatetable/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateTable extends TemplateItem
```

Tillhandahåller malltabellen.

Det finns två sätt att definiera en tabell:

* Using [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class. In this case the table is defined by its position on the page: rectangular area, columns and rows separators.
* Using [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class. In this case the table is detected automatically by algorithms with set parameters. See [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) class for more information.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable) med det STORA BOKSTÄVER-namnet. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable) med det STORA BOKSTÄVER-namnet. |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable) med det STORA BOKSTÄVER-namnet. |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
|  | [TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getLayout()](#getLayout--) | Hämtar tabellens layout. |
|
|  | [getParameters()](#getParameters--) | Hämtar parametrarna för att upptäcka tabellen i automatiskt läge. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable) med det STORA BOKSTÄVER-namnet.

Malltabellen sätts av tabellayout om tabellen inte kan upptäckas automatiskt:

````
TemplateTableLayout layout = new TemplateTableLayout(
     java.util.Arrays.asList(new Double[] { 50.0, 95.0, 275.0 }),
     java.util.Arrays.asList(new Double[] { 325.0, 340.0, 365.0 }));
 TemplateTable table = new TemplateTable(layout, "Details", null);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
````



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tabellayouten. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable) med det STORA BOKSTÄVER-namnet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tabellayouten. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tabellayouten. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableLayout-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableLayout layout, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | layout | [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) | Tabellayouten. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable) med det STORA BOKSTÄVER-namnet.

Om en malltabell sätts av detektorns parametrar, upptäcks tabellen automatiskt:

````
TemplateTableParameters parameters = new TemplateTableParameters(
     new Rectangle(new Point(175, 350), new Size(400, 200)),
     java.util.Arrays.asList(new Double[] { 185.0, 370.0, 425.0, 485.0, 545.0 }));
 TemplateTable table = new TemplateTable(parameters, "Details", 0);
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(new TemplateItem[] { table }));
 
````



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parametrarna för att upptäcka tabellen i automatiskt läge. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parametrarna för att upptäcka tabellen i automatiskt läge. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parametrarna för att upptäcka tabellen i automatiskt läge. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateTable-com.groupdocs.parser.templates.TemplateTableParameters-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateTable(TemplateTableParameters parameters, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateTable](../../com.groupdocs.parser.templates/templatetable).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | parameters | [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) | Parametrarna för att upptäcka tabellen i automatiskt läge. |
|
|  | namn | java.lang.String | Tabellens namn. |
|
|  | pageIndex | java.lang.Integer | Indexet för sidan där malltabellen är placerad;  null  om malltabellen är placerad på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### getLayout() {#getLayout--}
```
public TemplateTableLayout getLayout()
```


Hämtar tabellens layout.


**Returns:**
[TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) - An instance of [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) class that represents the table layout;  null  if it isn't set.

### getParameters() {#getParameters--}
```
public TemplateTableParameters getParameters()
```


Hämtar parametrarna för att upptäcka tabellen i automatiskt läge.


**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - An instance of  TemplateTableParameters  class that represents the parameters to detect the table in the automatic mode;  null  if it isn't set.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Skapar en kopia av det aktuella objektet med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
