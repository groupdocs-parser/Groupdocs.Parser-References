---
title: "Template"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Παρέχει το πρότυπο σελίδας εγγράφου."
type: docs
weight: 10
url: /el/java/com.groupdocs.parser.templates/template/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Template implements Iterable<TemplateItem>
```

Παρέχει το πρότυπο σελίδας εγγράφου. Αποτελείται από αντικείμενα [TemplateItem](../../com.groupdocs.parser.templates/templateitem) που αντιπροσωπεύουν τα στοιχεία του προτύπου, όπως πεδία κειμένου και ορισμούς πινάκων.

**Learn more:**

* [Working with templates](../https://docs.groupdocs.com/display/parserjava/Working+with+templates)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Template(Iterable<? extends TemplateItem> items)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Template](../../com.groupdocs.parser.templates/template) . |
|
|  | [Template(Iterable<? extends TemplateItem> items, TemplateOptions options)](#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Template](../../com.groupdocs.parser.templates/template) . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCount()](#getCount--) | Λαμβάνει τον συνολικό αριθμό των στοιχείων προτύπου. |
|
|  | [get(int index)](#get-int-) | Λαμβάνει το στοιχείο προτύπου με δείκτη. |
|
|  | [getOptions()](#getOptions--) | Λαμβάνει τις επιλογές του προτύπου. |
|
| [iterator()](#iterator--) |  |
|  | [load(String filePath)](#load-java.lang.String-) | Φορτώνει ένα πρότυπο από αρχείο. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Φορτώνει ένα πρότυπο από ροή. |
|
|  | [save(String filePath)](#save-java.lang.String-) | Αποθηκεύει ένα πρότυπο σε αρχείο. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Αποθηκεύει ένα πρότυπο σε ροή. |
|
### Template(Iterable<? extends TemplateItem> items) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--}
```
public Template(Iterable<? extends TemplateItem> items)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Template](../../com.groupdocs.parser.templates/template) .

Χρήση:

````
// Create an array of template fields
 TemplateItem[] fields = new TemplateItem[]
 {
     new TemplateField(new TemplateRegexPosition("From"), "From", 0),
     new TemplateField(
         new TemplateLinkedPosition("From", new Size(100, 10), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromCompany",
         0),
     new TemplateField(
         new TemplateLinkedPosition("FromCompany", new Size(100, 30), new TemplateLinkedPositionEdges(false, false, false, true)),
         "FromAddress",
         0)
 };
 // Create a document template
 Template template = new Template(java.util.Arrays.asList(fields));
 
````



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Η συλλογή των αντικειμένων [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|

### Template(Iterable<? extends TemplateItem> items, TemplateOptions options) {#Template-java.lang.Iterable---extends-com.groupdocs.parser.templates.TemplateItem--com.groupdocs.parser.templates.TemplateOptions-}
```
public Template(Iterable<? extends TemplateItem> items, TemplateOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Template](../../com.groupdocs.parser.templates/template) .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | items | java.lang.Iterable<? extends com.groupdocs.parser.templates.TemplateItem> | Η συλλογή των αντικειμένων [TemplateItem](../../com.groupdocs.parser.templates/templateitem). |
|
|  | options | [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) | Οι επιλογές του προτύπου. |
|

### getCount() {#getCount--}
```
public int getCount()
```


Λαμβάνει τον συνολικό αριθμό των στοιχείων προτύπου.


**Returns:**
int - Ένας ακέραιος που αντιπροσωπεύει τον συνολικό αριθμό των στοιχείων προτύπου.

### get(int index) {#get-int-}
```
public TemplateItem get(int index)
```


Λαμβάνει το στοιχείο προτύπου με δείκτη.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δείκτης | int | Ο δείκτης μηδενικής βάσης του στοιχείου προτύπου. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - An instance of [TemplateItem](../../com.groupdocs.parser.templates/templateitem) class.

### getOptions() {#getOptions--}
```
public TemplateOptions getOptions()
```


Λαμβάνει τις επιλογές του προτύπου.


**Returns:**
[TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) - An instance of [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) class.

### iterator() {#iterator--}
```
public Iterator<TemplateItem> iterator()
```




**Returns:**
java.util.Iterator<com.groupdocs.parser.templates.TemplateItem>
### load(String filePath) {#load-java.lang.String-}
```
public static Template load(String filePath)
```


Φορτώνει ένα πρότυπο από αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Template load(InputStream stream)
```


Φορτώνει ένα πρότυπο από ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | stream | java.io.InputStream | Η ροή εισόδου. |
|

**Returns:**
[Template](../../com.groupdocs.parser.templates/template) - An instance of [Template](../../com.groupdocs.parser.templates/template) class with loaded template.

### save(String filePath) {#save-java.lang.String-}
```
public void save(String filePath)
```


Αποθηκεύει ένα πρότυπο σε αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή προς το αρχείο. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Αποθηκεύει ένα πρότυπο σε ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | stream | java.io.OutputStream | Η ροή εξόδου. |
|

