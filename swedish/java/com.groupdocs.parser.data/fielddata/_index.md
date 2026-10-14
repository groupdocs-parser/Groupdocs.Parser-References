---
title: "FieldData"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar fältdata såsom ett namn, ett sidindex, ett fältvärde osv."
type: docs
weight: 13
url: /sv/java/com.groupdocs.parser.data/fielddata/
---
**Inheritance:**
java.lang.Object
```
public class FieldData
```

Representerar fältdata såsom ett namn, ett sidindex, ett fältvärde osv. Beroende på fältet kan värdet vara text, en bild, en tabell osv.

Instanserna av klassen [FieldData](../../com.groupdocs.parser.data/fielddata) används i samlingen [DocumentData](../../com.groupdocs.parser.data/documentdata).

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getName()](#getName--) | Hämtar fältets namn. |
|
|  | [getPageIndex()](#getPageIndex--) | Hämtar sidindexet. |
|
|  | [getPageArea()](#getPageArea--) | Hämtar fältets värde. |
|
|  | [getLinkedField()](#getLinkedField--) | Hämtar det länkade fältet. |
|
|  | [getText()](#getText--) | Hämtar texten. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Hämtar ett värde som indikerar om ett  Name  konverterades till STORA BOKSTÄVER. |
|
### getName() {#getName--}
```
public String getName()
```


Hämtar fältets namn.


**Returns:**
java.lang.String - Ett strängvärde i versaler som representerar fältets namn.

### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Hämtar sidindexet.


**Returns:**
int - Ett nollbaserat index för sidan som innehåller fältet.

### getPageArea() {#getPageArea--}
```
public PageArea getPageArea()
```


Hämtar fältets värde.

Beroende på fältet kan PageArea-egenskapen innehålla någon av arvtagarna till klassen [PageArea](../../com.groupdocs.parser.data/pagearea).
Till exempel extraherar metoden [Parser.parseForm()](../../com.groupdocs.parser/parser#parseForm--) endast textfält.

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


Hämtar det länkade fältet.


**Returns:**
[FieldData](../../com.groupdocs.parser.data/fielddata) - An instance of [FieldData](../../com.groupdocs.parser.data/fielddata) class that represents the field which is linked to the field;  null  if it isn't set.

### getText() {#getText--}
```
public String getText()
```


Hämtar texten.


**Returns:**
java.lang.String - Ett strängvärde som representerar fältets textvärde; null om egenskapen [PageArea](../../com.groupdocs.parser.data/pagearea) inte är en [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Hämtar ett värde som indikerar om ett  Name  konverterades till STORA BOKSTÄVER.


**Returns:**
boolean - Ett booleskt värde som indikerar om ett  Name  konverterades till STORA BOKSTÄVER.

