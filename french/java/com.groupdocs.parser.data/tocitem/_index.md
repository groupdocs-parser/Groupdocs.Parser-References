---
title: "TocItem"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente l'élément utilisé dans la fonctionnalité d'extraction de la table des matières."
type: docs
weight: 31
url: /fr/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Représente l'élément utilisé dans la fonctionnalité d'extraction de la table des matières.

Une instance de la classe [TocItem](../../com.groupdocs.parser.data/tocitem) est utilisée comme valeur de retour de la méthode [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) . Voir les exemples d'utilisation là‑bas.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Initialise une nouvelle instance de la classe TocItem. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getDepth()](#getDepth--) | Obtient le niveau de profondeur. |
|
|  | [getText()](#getText--) | Obtient le texte. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtient l'indice de page. |
|
|  | [extractText()](#extractText--) | Extrait un texte du document auquel l'objet TocItem fait référence. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Initialise une nouvelle instance de la classe TocItem.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | depth | int | Le niveau de profondeur de l'élément. |
|
|  | texte | java.lang.String | Le texte de l'élément. |
|
|  | pageIndex | java.lang.Integer | L'indice de la page référencée par l'élément |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Obtient le niveau de profondeur.


**Returns:**
int - Une valeur entière qui représente le niveau de profondeur de l'élément.

### getText() {#getText--}
```
public String getText()
```


Obtient le texte.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le texte de l'élément.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Obtient l'indice de page.


**Returns:**
java.lang.Integer - Une valeur entière qui représente l'indice de la page référencée par l'élément ;  null  si elle n'est pas définie.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Extrait un texte du document auquel l'objet TocItem fait référence.

L'exemple suivant montre comment extraire un texte à l'aide d'un élément de la table des matières :

````
// Create an instance of Parser class
 try (Parser parser = new Parser(Constants.SampleDocxWithToc)) {
     // Get table of contents
     Iterable tocItems = parser.getToc();

     // Check if toc extraction is supported
     if (tocItems == null) {
         System.out.println("Table of contents extraction isn't supported");
     }

     // Iterate over items
     for (TocItem tocItem : tocItems) {
         // Print the text of the chapter
         try (TextReader reader = tocItem.extractText()) {
             System.out.println("----");
             System.out.println(reader.readToEnd());
         }
     }
 }
 
````



**Returns:**
[TextReader](../../com.groupdocs.parser.data/textreader) - An instance of [TextReader](../../com.groupdocs.parser.data/textreader) class with the extracted text.

