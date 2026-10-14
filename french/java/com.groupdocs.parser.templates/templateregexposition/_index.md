---
title: "TemplateRegexPosition"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit une position de champ de modèle qui utilise l'expression régulière."
type: docs
weight: 19
url: /fr/java/com.groupdocs.parser.templates/templateregexposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateRegexPosition extends TemplatePosition
```

Fournit une position de champ de modèle qui utilise l'expression régulière.

L'exemple suivant montre la situation si le document contient "Invoice Number INV-12345"
alors le champ de modèle peut être défini de la manière suivante:

````
// Create a regex template field with "InvoiceNumber" name
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+[A-Z0-9\\-]+"),
     "InvoiceNumber");
 
````

Dans ce cas, la chaîne entière est extraite comme valeur. Pour extraire uniquement une partie de la chaîne
le groupe d'expression régulière "value" est utilisé:

````
// Create a regex template field with "InvoiceNumber" name with "value" group
 TemplateField templateField = new TemplateField(
     new TemplateRegexPosition("Invoice Number\\s+(?[A-Z0-9\\-]+)"),
     "InvoiceNumber");
````

Dans ce cas, la chaîne "INV-3337" est extraite comme valeur.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TemplateRegexPosition(String expression)](#TemplateRegexPosition-java.lang.String-) | Initialise une nouvelle instance de la classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
|  | [TemplateRegexPosition(String expression, boolean matchCase)](#TemplateRegexPosition-java.lang.String-boolean-) | Initialise une nouvelle instance de la classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getExpression()](#getExpression--) | Obtient l'expression régulière. |
|
|  | [isMatchCase()](#isMatchCase--) | Obtient la valeur qui indique si la casse du texte n'est pas ignorée. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateRegexPosition(String expression) {#TemplateRegexPosition-java.lang.String-}
```
public TemplateRegexPosition(String expression)
```


Initialise une nouvelle instance de la classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | expression | java.lang.String | L'expression régulière. |
|

### TemplateRegexPosition(String expression, boolean matchCase) {#TemplateRegexPosition-java.lang.String-boolean-}
```
public TemplateRegexPosition(String expression, boolean matchCase)
```


Initialise une nouvelle instance de la classe [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | expression | java.lang.String | L'expression régulière. |
|
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Obtient l'expression régulière.


**Returns:**
java.lang.String - Une chaîne qui représente l'expression régulière.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Obtient la valeur qui indique si la casse du texte n'est pas ignorée.


**Returns:**
boolean -  true  si la casse du texte n'est pas ignorée ; sinon,  false .

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Crée une copie de la position actuelle avec toutes les coordonnées mises à l'échelle par le facteur donné.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| factor | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
