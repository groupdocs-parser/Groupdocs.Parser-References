---
title: "Lizenz"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die GroupDocs.Parser‑Lizenz dar."
type: docs
weight: 10
url: /de/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Stellt die GroupDocs.Parser‑Lizenz dar.

Dieses Beispiel zeigt, wie man die Lizenz einrichtet.

````
 ```

// Lizenzklasse initialisieren
License license = new License();
// Pfad zur .lic-Datei festlegen
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [License()](#License--) | Initialisiert eine neue Instanz der [License](../../com.groupdocs.parser.licensing/license) Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Lizenziert die Komponente. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Lizenziert die Komponente. |
|
### License() {#License--}
```
public License()
```


Initialisiert eine neue Instanz der [License](../../com.groupdocs.parser.licensing/license) Klasse.


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Lizenziert die Komponente.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Absoluter Pfad zur Lizenzdatei. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Lizenziert die Komponente.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.InputStream | Lizenz-Stream. |
|

