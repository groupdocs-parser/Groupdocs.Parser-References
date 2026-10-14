---
title: "DocumentData"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa los datos del documento."
type: docs
weight: 11
url: /es/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Representa los datos del documento. Consiste en objetos [FieldData](../../com.groupdocs.parser.data/fielddata) que contienen los datos de campo del documento. Una instancia de la clase [DocumentData](../../com.groupdocs.parser.data/documentdata) se utiliza como valor de retorno de los métodos [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) y [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) . Consulte los ejemplos de uso allí.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Obtiene la plantilla que generó estos datos del documento. |
|
|  | [getCount()](#getCount--) | Obtiene el número total de los datos de los campos. |
|
|  | [get(int index)](#get-int-) | Obtiene los datos del campo por un índice. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Devuelve la colección de datos de campo donde el nombre es igual a  fieldName . |
|
|  | [iterator()](#iterator--) | Devuelve un iterador sobre los elementos de esta lista en la secuencia adecuada. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Obtiene la plantilla que generó estos datos del documento.

Cuando los datos fueron producidos por una selección automática de colección de plantillas (ver
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
esta es la plantilla seleccionada.
null
cuando los datos no fueron producidos por una plantilla.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Obtiene el número total de los datos de los campos.


**Returns:**
int - Un valor entero que representa el número total de datos de los campos.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Obtiene los datos del campo por un índice.

Iteración a través de todos los campos:

````
// Print all extracted data
 for (int i = 0; i < data.getCount(); i++) {
     // Print field name
     System.out.print(data.get(i).getName() + ": ");
     // As we have defined only text fields in the template,
     // we cast PageArea property value to PageTextArea
     PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
             ? (PageTextArea) data.get(i).getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field PageArea property can contain any
de los herederos de la clase [PageArea](../../com.groupdocs.parser.data/pagearea). Por ejemplo, el método [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extrae solo campos de texto:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleFormsPdf)) {
     // Extract data from PDF document
     DocumentData data = parser.parseForm();
     // Check if form extraction is supported
     if (data == null) {
         System.out.println("Form extraction isn't supported.");
         return;
     }
     // Iterate over extracted data
     for (int i = 0; i < data.getCount(); i++) {
         System.out.print(data.get(i).getName() + ": ");
         PageTextArea area = data.get(i).getPageArea() instanceof PageTextArea
                 ? (PageTextArea) data.get(i).getPageArea()
                 : null;
         System.out.println(area == null ? "Not a template field" : area.getText());
     }
 }
 
````



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | El índice basado en cero del campo. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Devuelve la colección de datos de campo donde el nombre es igual a  fieldName .

Buscar campos por nombre de campo:

````
// Print prices
 System.out.println("Prices:");
 for (FieldData field : data.getFieldsByName("Price")) {
     PageTextArea area = field.getPageArea() instanceof PageTextArea
             ? (PageTextArea) field.getPageArea()
             : null;
     System.out.println(area == null ? "Not a template field" : area.getText());
 }
 
````

[FieldData](../../com.groupdocs.parser.data/fielddata) class represents field data. Depending on the field [PageArea](../../com.groupdocs.parser.data/pagearea) property can contain
cualquiera de los herederos de la clase [PageArea](../../com.groupdocs.parser.data/pagearea). Por ejemplo, el método [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extrae solo campos de texto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fieldName | java.lang.String | El nombre del campo. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - Una colección de objetos [FieldData](../../com.groupdocs.parser.data/fielddata); colección vacía si no se encuentran datos de campo.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Devuelve un iterador sobre los elementos de esta lista en la secuencia adecuada.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - un iterador sobre los elementos de esta lista en la secuencia adecuada.

