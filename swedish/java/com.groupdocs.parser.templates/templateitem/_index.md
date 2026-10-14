---
title: "TemplateItem"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller en abstrakt basklass för mallobjekt."
type: docs
weight: 14
url: /sv/java/com.groupdocs.parser.templates/templateitem/
---
**Inheritance:**
java.lang.Object
```
public abstract class TemplateItem
```

Tillhandahåller en abstrakt basklass för mallobjekt.

Arvingarna till klassen [TemplateItem](../../com.groupdocs.parser.templates/templateitem) används i samlingen [Template](../../com.groupdocs.parser.templates/template).

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [scale(double factor)](#scale-double-) | Skapar en kopia av det aktuella objektet med alla koordinater skalade med den angivna faktorn. |
|
|  | [getName()](#getName--) | Hämtar namnet på mallobjektet. |
|
|  | [getPageIndex()](#getPageIndex--) | Hämtar sidindexet för mallobjektet. |
|
|  | [getPageWidth()](#getPageWidth--) | Hämtar bredden på sidan som användes för att skapa mallobjektet. |
|
|  | [getUseUpperCaseName()](#getUseUpperCaseName--) | Hämtar ett värde som indikerar om ett  Name  konverterades till STORA BOKSTÄVER. |
|
### scale(double factor) {#scale-double-}
```
public abstract TemplateItem scale(double factor)
```


Skapar en kopia av det aktuella objektet med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | faktor | double | Skalfaktorn. |
|

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem) - A new [TemplateItem](../../com.groupdocs.parser.templates/templateitem) with scaled coordinates.

### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på mallobjektet.


**Returns:**
java.lang.String - Ett strängvärde i stora bokstäver som representerar ett namn på mallobjektet.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Hämtar sidindexet för mallobjektet.


**Returns:**
java.lang.Integer - Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida.

### getPageWidth() {#getPageWidth--}
```
public Double getPageWidth()
```


Hämtar bredden på sidan som användes för att skapa mallobjektet.


**Returns:**
java.lang.Double - Sidans bredd i pixlar;  null  om sidbredden är okänd.

### getUseUpperCaseName() {#getUseUpperCaseName--}
```
public boolean getUseUpperCaseName()
```


Hämtar ett värde som indikerar om ett  Name  konverterades till STORA BOKSTÄVER.


**Returns:**
boolean - Ett booleskt värde som indikerar om ett  Name  konverterades till STORA BOKSTÄVER.

