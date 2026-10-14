---
title: "DocumentData"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αντιπροσωπεύει τα δεδομένα του εγγράφου."
type: docs
weight: 11
url: /el/java/com.groupdocs.parser.data/documentdata/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class DocumentData implements Iterable<FieldData>
```

Αναπαριστά τα δεδομένα του εγγράφου. Αποτελείται από αντικείμενα [FieldData](../../com.groupdocs.parser.data/fielddata) που περιέχουν δεδομένα πεδίου από το έγγραφο. Μια παρουσία της κλάσης [DocumentData](../../com.groupdocs.parser.data/documentdata) χρησιμοποιείται ως τιμή επιστροφής των μεθόδων [Parser.parseByTemplate(Template)](../../com.groupdocs.parser/parser#parseByTemplate-Template-) και [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) . Δείτε τα παραδείγματα χρήσης εκεί.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getTemplate()](#getTemplate--) | Λαμβάνει το πρότυπο που παρήγαγε αυτά τα δεδομένα εγγράφου. |
|
|  | [getCount()](#getCount--) | Λαμβάνει τον συνολικό αριθμό των δεδομένων πεδίων. |
|
|  | [get(int index)](#get-int-) | Λαμβάνει τα δεδομένα πεδίου με βάση έναν δείκτη. |
|
|  | [getFieldsByName(String fieldName)](#getFieldsByName-java.lang.String-) | Επιστρέφει τη συλλογή των δεδομένων πεδίου όπου το όνομα είναι ίσο με  fieldName . |
|
|  | [iterator()](#iterator--) | Επιστρέφει έναν επαναλήπτη πάνω στα στοιχεία αυτής της λίστας με τη σωστή σειρά. |
|
### getTemplate() {#getTemplate--}
```
public Template getTemplate()
```


Λαμβάνει το πρότυπο που παρήγαγε αυτά τα δεδομένα εγγράφου.

Όταν τα δεδομένα δημιουργήθηκαν από αυτόματη επιλογή συλλογής προτύπων (δείτε
[Parser.parseByTemplate(com.groupdocs.parser.templates.TemplateCollection, com.groupdocs.parser.options.ParseByTemplateOptions)](../../com.groupdocs.parser/parser#parseByTemplate-com.groupdocs.parser.templates.TemplateCollection--com.groupdocs.parser.options.ParseByTemplateOptions-)),
αυτό είναι το επιλεγμένο πρότυπο.
null
όταν τα δεδομένα δεν δημιουργήθηκαν από πρότυπο.


**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - The source [Template](../../com.groupdocs.parser.templates/template), or  null .

### getCount() {#getCount--}
```
public int getCount()
```


Λαμβάνει τον συνολικό αριθμό των δεδομένων πεδίων.


**Returns:**
int - Μια ακέραια τιμή που αντιπροσωπεύει το συνολικό αριθμό των δεδομένων πεδίων.

### get(int index) {#get-int-}
```
public FieldData get(int index)
```


Λαμβάνει τα δεδομένα πεδίου με βάση έναν δείκτη.

Επανάληψη μέσω όλων των πεδίων:

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
των κληρονόμων της κλάσης [PageArea](../../com.groupdocs.parser.data/pagearea). Για παράδειγμα, η μέθοδος [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) εξάγει μόνο πεδία κειμένου:

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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δείκτης | int | Ο μηδενικός δείκτης του πεδίου. |
|

**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class.

### getFieldsByName(String fieldName) {#getFieldsByName-java.lang.String-}
```
public List<FieldData> getFieldsByName(String fieldName)
```


Επιστρέφει τη συλλογή των δεδομένων πεδίου όπου το όνομα είναι ίσο με  fieldName .

Βρείτε πεδία με όνομα πεδίου:

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
οποιοσδήποτε από τους κληρονόμους της κλάσης [PageArea](../../com.groupdocs.parser.data/pagearea). Για παράδειγμα, η μέθοδος [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) εξάγει μόνο πεδία κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fieldName | java.lang.String | Το όνομα του πεδίου. |
|

**Returns:**
java.util.List<com.groupdocs.parser.data.FieldData> - Μια συλλογή αντικειμένων [FieldData](../../com.groupdocs.parser.data/fielddata); κενή συλλογή εάν δεν βρεθούν δεδομένα πεδίου.

### iterator() {#iterator--}
```
public Iterator<FieldData> iterator()
```


Επιστρέφει έναν επαναλήπτη πάνω στα στοιχεία αυτής της λίστας με τη σωστή σειρά.


**Returns:**
java.util.Iterator<com.groupdocs.parser.data.FieldData> - ένας επαναλήπτης των στοιχείων σε αυτή τη λίστα με τη σωστή σειρά.

