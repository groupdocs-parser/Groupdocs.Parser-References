---
title: "License"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa la licencia de GroupDocs.Parser."
type: docs
weight: 10
url: /es/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

Representa la licencia de GroupDocs.Parser.

Este ejemplo muestra cómo configurar la licencia.

````
 ```

// Inicializar la clase License
License license = new License();
// Establecer la ruta al archivo .lic
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [License()](#License--) | Inicializa una nueva instancia de la clase [License](../../com.groupdocs.parser.licensing/license). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | Licencia el componente. |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Licencia el componente. |
|
### License() {#License--}
```
public License()
```


Inicializa una nueva instancia de la clase [License](../../com.groupdocs.parser.licensing/license).


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


Licencia el componente.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | Ruta absoluta al archivo de licencia. |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Licencia el componente.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.InputStream | Flujo de licencia. |
|

