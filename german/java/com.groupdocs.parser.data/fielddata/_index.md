---
title: "FieldData"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt Felddaten dar, wie z. B. einen Namen, einen Seitenindex, einen Feldwert und so weiter."
type: docs
weight: 13
url: /de/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Stellt Felddaten dar, wie z. B. einen Namen, einen Seitenindex, einen Feldwert und so weiter. Abhängig vom Feld kann der Wert ein Text, ein Bild, eine Tabelle usw. sein.

Die Instanzen der Klasse [FieldData](../../com.groupdocs.parser.data/fielddata) werden in der Sammlung [DocumentData](../../com.groupdocs.parser.data/documentdata) verwendet.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getName()](#getName--) | Liefert den Feldnamen. |
|
|  | [getPageIndex()](#getPageIndex--) | Liefert den Seitenindex. |
|
|  | [getPageArea()](#getPageArea--) | Liefert den Wert des Feldes. |
|
|  | [getLinkedField()](#getLinkedField--) | Liefert das verknüpfte Feld. |
|
|  | [getText()](#getText--) | Liefert den Text. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Gibt einen Wert zurück, der angibt, ob ein  Name  in GROSSBUCHSTABEN konvertiert wurde. |
|
### getName() {#getName--}
```
public String getName()
```


Liefert den Feldnamen.


**Returns:**
java.lang.String - Ein String-Wert in Großbuchstaben, der den Namen des Feldes darstellt.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Liefert den Seitenindex.


**Returns:**
int - Ein nullbasierter Index der Seite, die das Feld enthält.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Liefert den Wert des Feldes.

Abhängig vom Feld kann die PageArea-Eigenschaft jede der Unterklassen der Klasse [PageArea](../../com.groupdocs.parser.data/pagearea) enthalten.
Zum Beispiel extrahiert die Methode [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) nur Textfelder.

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


Liefert das verknüpfte Feld.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Liefert den Text.


**Returns:**
java.lang.String - Ein String‑Wert, der den Wert des Feldtextes darstellt; null, wenn die Eigenschaft [PageArea](../../com.groupdocs.parser.data/pagearea) nicht [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) ist.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Gibt einen Wert zurück, der angibt, ob ein  Name  in GROSSBUCHSTABEN konvertiert wurde.


**Returns:**
boolean - Ein boolescher Wert, der angibt, ob ein  Name  in GROSSBUCHSTABEN konvertiert wurde.

