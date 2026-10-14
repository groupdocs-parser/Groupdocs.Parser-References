---
title: "DocumentData"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente les données du document."
type: docs
weight: 11
url: /fr/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Représente les données du document. Il se compose d'objets [FieldData](../../com.groupdocs.parser.data/fielddata) qui contiennent les données de champ du document. Une instance de la classe [DocumentData](../../com.groupdocs.parser.data/documentdata) est utilisée comme valeur de retour des méthodes [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) et [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--). Voir les exemples d'utilisation à cet endroit.

## Methods

| Method | Description |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Obtient le modèle qui a produit ces données de document. |
|
|  | [getCount()](#getCount--) | Obtient le nombre total des données de champs. |
|
|  | [get(int index)](#get-int-) | Obtient les données du champ par un indice. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Renvoie la collection de données de champ dont le nom est égal à  fieldName . |
|
|  | [iterator()](#iterator--) | Renvoie un itérateur sur les éléments de cette liste dans l'ordre correct. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Obtient le modèle qui a produit ces données de document.

Lorsque les données ont été produites par une sélection automatique de modèle-collection (voir
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
c’est le modèle sélectionné.
null
lorsque les données n'ont pas été produites par un modèle.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Obtient le nombre total des données de champs.


**Returns:**
int - Une valeur entière qui représente le nombre total des données de champs.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Obtient les données du champ par un indice.

Itération via tous les champs :

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
des héritiers de la classe [PageArea](../../com.groupdocs.parser.data/pagearea). Par exemple, la méthode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extrait uniquement les champs de texte :

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
| Parameter | Type | Description |
| --- | --- | --- |
|  | indice | int | L'indice zéro‑basé du champ. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Renvoie la collection de données de champ dont le nom est égal à  fieldName .

Trouver les champs par nom de champ :

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
tout héritier de la classe [PageArea](../../com.groupdocs.parser.data/pagearea). Par exemple, la méthode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) extrait uniquement les champs de texte.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | fieldName | java.lang.String | Le nom du champ. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - Une collection d'objets [FieldData](../../com.groupdocs.parser.data/fielddata) ; collection vide si aucune donnée de champ n'est trouvée.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Renvoie un itérateur sur les éléments de cette liste dans l'ordre correct.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - un itérateur sur les éléments de cette liste dans l'ordre correct.

