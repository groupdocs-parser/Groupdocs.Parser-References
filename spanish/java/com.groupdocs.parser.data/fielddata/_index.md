---
title: "FieldData"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa datos de campo como un nombre, un índice de página, un valor de campo, etc."
type: docs
weight: 13
url: /es/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Representa datos de campo como un nombre, un índice de página, un valor de campo, etc. Dependiendo del campo, el valor puede ser un texto, una imagen, una tabla, etc.

Las instancias de la clase [FieldData](../../com.groupdocs.parser.data/fielddata) se utilizan en la colección [DocumentData](../../com.groupdocs.parser.data/documentdata).

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getName()](#getName--) | Obtiene el nombre del campo. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtiene el índice de página. |
|
|  | [getPageArea()](#getPageArea--) | Obtiene el valor del campo. |
|
|  | [getLinkedField()](#getLinkedField--) | Obtiene el campo vinculado. |
|
|  | [getText()](#getText--) | Obtiene el texto. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Obtiene un valor que indica si un  Name  fue convertido a MAYÚSCULAS. |
|
### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del campo.


**Returns:**
java.lang.String - Un valor de cadena en mayúsculas que representa el nombre del campo.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Obtiene el índice de página.


**Returns:**
int - Un índice basado en cero de la página que contiene el campo.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Obtiene el valor del campo.

Dependiendo del campo, la propiedad PageArea puede contener cualquiera de los herederos de la clase [PageArea](../../com.groupdocs.parser.data/pagearea).
Por ejemplo, el método [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extrae solo campos de texto.

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


Obtiene el campo vinculado.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Obtiene el texto.


**Returns:**
java.lang.String - Un valor de cadena que representa el valor del texto del campo; null si la propiedad [PageArea](../../com.groupdocs.parser.data/pagearea) no es [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Obtiene un valor que indica si un  Name  fue convertido a MAYÚSCULAS.


**Returns:**
boolean - Un valor booleano que indica si un  Name  fue convertido a MAYÚSCULAS.

