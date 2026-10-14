---
title: "TemplateTableParameters"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit des paramètres pour les algorithmes de détection de tables."
type: docs
weight: 22
url: /fr/java/com.groupdocs.parser.templates/templatetableparameters/
---
**Inheritance:**
java.lang.Object
```
public class TemplateTableParameters
```

Fournit des paramètres pour les algorithmes de détection de tables.

Il existe deux algorithmes pour détecter un tableau :

* Allows to detect a table in the rectangular area with set columns. This algorithm is useful for simple tables (without merged columns) and provides more accurate detection.
* Allows to detect a table in any place on the page. This is a more complex algorithm. It can detect tables in any place on the page. Additional parameters help to detect a table more correctly.

Dans certains cas, lorsque les algorithmes ne peuvent pas détecter un tableau ou le font de manière imprécise, la classe [TemplateTableLayout](../../com.groupdocs.parser.templates/templatetablelayout) est utilisée.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--) | Initialise une nouvelle instance de la classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
|  | [TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)](#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-) | Initialise une nouvelle instance de la classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtient la zone rectangulaire qui contient le tableau. |
|
|  | [getVerticalSeparators()](#getVerticalSeparators--) | Obtient les séparateurs de colonnes du tableau. |
|
|  | [hasMergedCells()](#hasMergedCells--) | Obtient la valeur qui indique si le tableau possède des cellules fusionnées. |
|
|  | [getMinRowCount()](#getMinRowCount--) | Obtient le nombre minimum de lignes du tableau. |
|
|  | [getMinColumnCount()](#getMinColumnCount--) | Obtient le nombre minimum de colonnes du tableau. |
|
|  | [getMinVerticalSpace()](#getMinVerticalSpace--) | Obtient l'espace minimum entre les colonnes du tableau. |
|
|  | [scale(double factor)](#scale-double-) | Crée une copie de ces paramètres avec toutes les coordonnées mises à l'échelle par le facteur donné. |
|
### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators)
```


Initialise une nouvelle instance de la classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient le tableau. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Les séparateurs de colonnes du tableau. |
|

### TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace) {#TemplateTableParameters-com.groupdocs.parser.data.Rectangle-java.lang.Iterable-java.lang.Double--java.lang.Boolean-java.lang.Integer-java.lang.Integer-java.lang.Integer-}
```
public TemplateTableParameters(Rectangle rectangle, Iterable<Double> verticalSeparators, Boolean mergedCells, Integer minRowCount, Integer minColumnCount, Integer minVerticalSpace)
```


Initialise une nouvelle instance de la classe [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient le tableau. |
|
|  | verticalSeparators | java.lang.Iterable<java.lang.Double> | Les séparateurs de colonnes du tableau. |
|
|  | mergedCells | java.lang.Boolean | La valeur qui indique si le tableau possède des cellules fusionnées. |
|
|  | minRowCount | java.lang.Integer | Le nombre minimum de lignes du tableau. |
|
|  | minColumnCount | java.lang.Integer | Le nombre minimum de colonnes du tableau. |
|
|  | minVerticalSpace | java.lang.Integer | L'espace minimum entre les colonnes du tableau. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtient la zone rectangulaire qui contient le tableau.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the table;  null  if it isn't set.

### getVerticalSeparators() {#getVerticalSeparators--}
```
public List<Double> getVerticalSeparators()
```


Obtient les séparateurs de colonnes du tableau.


**Returns:**
java.util.List<java.lang.Double> - Une collection de valeurs double qui représentent les coordonnées x des séparateurs de colonnes du tableau ;  null  si elle n'est pas définie.

### hasMergedCells() {#hasMergedCells--}
```
public Boolean hasMergedCells()
```


Obtient la valeur qui indique si le tableau possède des cellules fusionnées.


**Returns:**
java.lang.Boolean -  true  si le tableau possède des cellules fusionnées ; sinon,  false .  null  si elle n'est pas définie.

### getMinRowCount() {#getMinRowCount--}
```
public Integer getMinRowCount()
```


Obtient le nombre minimum de lignes du tableau.


**Returns:**
java.lang.Integer - Une valeur entière qui représente le nombre minimum de lignes du tableau ;  null  si elle n'est pas définie.

### getMinColumnCount() {#getMinColumnCount--}
```
public Integer getMinColumnCount()
```


Obtient le nombre minimum de colonnes du tableau.


**Returns:**
java.lang.Integer - Une valeur entière qui représente le nombre minimum de colonnes du tableau ;  null  si elle n'est pas définie.

### getMinVerticalSpace() {#getMinVerticalSpace--}
```
public Integer getMinVerticalSpace()
```


Obtient l'espace minimum entre les colonnes du tableau.


**Returns:**
java.lang.Integer - Une valeur entière qui représente l'espace minimum entre les colonnes du tableau ;  null  si elle n'est pas définie.

### scale(double factor) {#scale-double-}
```
public TemplateTableParameters scale(double factor)
```


Crée une copie de ces paramètres avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | factor | double | Le facteur d'échelle. |
|

**Returns:**
[TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) - A new [TemplateTableParameters](../../com.groupdocs.parser.templates/templatetableparameters) with scaled coordinates.

