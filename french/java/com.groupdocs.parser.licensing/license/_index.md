---
title: "License"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente la licence GroupDocs.Parser."
type: docs
weight: 10
url: /fr/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Représente la licence GroupDocs.Parser.

Cet exemple montre comment configurer la licence.

````
 ```

// Initialise la classe License
License license = new License();
// Définir le chemin du fichier .lic
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Constructors

| Constructor | Description |
| --- | --- |
|  | [License()](#License--) | Initialise une nouvelle instance de la classe [License](../../com.groupdocs.parser.licensing/license). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Licence le composant. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licence le composant. |
|
### License() {#License--}
```
public License()
```


Initialise une nouvelle instance de la classe [License](../../com.groupdocs.parser.licensing/license).


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Licence le composant.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Chemin absolu du fichier de licence. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licence le composant.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | stream | java.io.InputStream | Flux de licence. |
|

