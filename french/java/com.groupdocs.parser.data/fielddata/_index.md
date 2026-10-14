---
title: "FieldData"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les données de champ telles qu'un nom, un indice de page, une valeur de champ, etc."
type: docs
weight: 13
url: /fr/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Représente les données de champ telles qu'un nom, un indice de page, une valeur de champ, etc. Selon le champ, la valeur peut être un texte, une image, un tableau, etc.

Les instances de la classe [FieldData](../../com.groupdocs.parser.data/fielddata) sont utilisées dans la collection [DocumentData](../../com.groupdocs.parser.data/documentdata).

## Methods

| Method | Description |
| --- | --- |
|  | [getName()](#getName--) | Obtient le nom du champ. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtient l'indice de page. |
|
|  | [getPageArea()](#getPageArea--) | Obtient la valeur du champ. |
|
|  | [getLinkedField()](#getLinkedField--) | Obtient le champ lié. |
|
|  | [getText()](#getText--) | Obtient le texte. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Obtient une valeur qui indique si un  Name  a été converti en MAJUSCULES. |
|
### getName() {#getName--}
```
public String getName()
```


Obtient le nom du champ.


**Returns:**
java.lang.String - Une valeur de chaîne en majuscules qui représente le nom du champ.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtient l'indice de page.


**Returns:**
int - Un indice de page basé sur zéro qui contient le champ.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Obtient la valeur du champ.

Selon le champ, la propriété PageArea peut contenir n'importe lequel des héritiers de la classe [PageArea](../../com.groupdocs.parser.data/pagearea).
Par exemple, la méthode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extrait uniquement les champs de texte.

````
PageTextArea area = field.getPageArea() instanceof PageTextArea
         ? (PageTextArea) field.getPageArea()
         : null;
 System.out.println(area == null ? "Not a template field" : area.getText());
 
````



**Returns:**
[PageArea](../../com.groupdocs.parser.data/pagearea) - An instance of [PageArea](../../com.groupdocs.parser.data/pagearea) class that represents the value of the field.

### getLinkedField() {#getLinkedField--}
```
public FieldData getLinkedField()
```


Obtient le champ lié.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Obtient le texte.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente la valeur du texte du champ ; null si la propriété [PageArea](../../com.groupdocs.parser.data/pagearea) n'est pas [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Obtient une valeur qui indique si un  Name  a été converti en MAJUSCULES.


**Returns:**
boolean - Une valeur booléenne qui indique si un  Name  a été converti en MAJUSCULE.

