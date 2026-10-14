---
title: "Licens"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar GroupDocs.Parser-licens."
type: docs
weight: 10
url: /sv/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Representerar GroupDocs.Parser-licens.

Detta exempel visar hur man ställer in licens.

````
 ```

// Initiera Licens-klass
License license = new License();
// Ange sökväg till .lic-fil
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [License()](#License--) | Initierar en ny instans av klassen [License](../../com.groupdocs.parser.licensing/license). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Licensierar komponenten. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licensierar komponenten. |
|
### License() {#License--}
```
public License()
```


Initierar en ny instans av klassen [License](../../com.groupdocs.parser.licensing/license).


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Licensierar komponenten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Absolut sökväg till licensfilen. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licensierar komponenten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | stream | java.io.InputStream | Licensström. |
|

