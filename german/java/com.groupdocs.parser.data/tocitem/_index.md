---
title: "TocItem"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt das Element dar, das in der Funktionalität zur Extraktion des Inhaltsverzeichnisses verwendet wird."
type: docs
weight: 31
url: /de/java/com.groupdocs.parser.data/tocitem/
---
**Inheritance:**
java.lang.Object
```
public class TocItem
```

Stellt das Element dar, das in der Funktionalität zur Extraktion des Inhaltsverzeichnisses verwendet wird.

Eine Instanz der [TocItem](../../com.groupdocs.parser.data/tocitem)-Klasse wird als Rückgabewert der Methode [Parser.getToc()](../../com.groupdocs.parser/parser#getToc--) verwendet. Siehe dort die Anwendungsbeispiele.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TocItem(int depth, String text, Integer pageIndex)](#TocItem-int-java.lang.String-java.lang.Integer-) | Initialisiert eine neue Instanz der TocItem-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDepth()](#getDepth--) | Liefert die Tiefenstufe. |
|
|  | [getText()](#getText--) | Liefert den Text. |
|
|  | [getPageIndex()](#getPageIndex--) | Liefert den Seitenindex. |
|
|  | [extractText()](#extractText--) | Extrahiert einen Text aus dem Dokument, auf das das TocItem-Objekt verweist. |
|
### TocItem(int depth, String text, Integer pageIndex) {#TocItem-int-java.lang.String-java.lang.Integer-}
```
public TocItem(int depth, String text, Integer pageIndex)
```


Initialisiert eine neue Instanz der TocItem-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Tiefe | int | Die Tiefenstufe des Elements. |
|
|  | Text | java.lang.String | Der Text des Elements. |
|
|  | pageIndex | java.lang.Integer | Der Index der von dem Element referenzierten Seite |
|

### getDepth() {#getDepth--}
```
public int getDepth()
```


Liefert die Tiefenstufe.


**Returns:**
int - Ein ganzzahliger Wert, der die Tiefenstufe des Elements darstellt.

### getText() {#getText--}
```
public String getText()
```


Liefert den Text.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den Text des Elements darstellt.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Liefert den Seitenindex.


**Returns:**
java.lang.Integer - Ein ganzzahliger Wert, der den Index der von dem Element referenzierten Seite darstellt;  null  wenn er nicht gesetzt ist.

### extractText() {#extractText--}
```
public TextReader extractText()
```


Extrahiert einen Text aus dem Dokument, auf das das TocItem-Objekt verweist.

Das folgende Beispiel zeigt, wie man einen Text anhand eines Elements des Inhaltsverzeichnisses extrahiert:

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

