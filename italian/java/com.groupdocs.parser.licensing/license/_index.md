---
title: "Licenza"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta la licenza di GroupDocs.Parser."
type: docs
weight: 10
url: /it/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Rappresenta la licenza di GroupDocs.Parser.

Questo esempio dimostra come configurare la licenza.

````
 ```

// Inizializza la classe License
License license = new License();
// Imposta il percorso al file .lic
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [License()](#License--) | Inizializza una nuova istanza della classe [License](../../com.groupdocs.parser.licensing/license). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Licenza il componente. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licenza il componente. |
|
### License() {#License--}
```
public License()
```


Inizializza una nuova istanza della classe [License](../../com.groupdocs.parser.licensing/license).


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Licenza il componente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Percorso assoluto al file di licenza. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licenza il componente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.InputStream | Stream di licenza. |
|

