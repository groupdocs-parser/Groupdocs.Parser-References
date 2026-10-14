---
title: "Licentie"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Vertegenwoordigt de GroupDocs.Parser-licentie."
type: docs
weight: 10
url: /nl/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Vertegenwoordigt de GroupDocs.Parser-licentie.

Dit voorbeeld laat zien hoe je een licentie instelt.

````
 ```

// Initialiseert Licentieklasse
License license = new License();
// Stel pad naar .lic-bestand in
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [License()](#License--) | Initialiseert een nieuw exemplaar van de [License](../../com.groupdocs.parser.licensing/license) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Licentieert de component. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licentieert de component. |
|
### License() {#License--}
```
public License()
```


Initialiseert een nieuw exemplaar van de [License](../../com.groupdocs.parser.licensing/license) klasse.


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Licentieert de component.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Absoluut pad naar licentiebestand. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licentieert de component.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.InputStream | Licentiestroom. |
|

