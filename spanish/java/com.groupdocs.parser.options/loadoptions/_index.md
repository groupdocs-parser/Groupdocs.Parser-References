---
title: "LoadOptions"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona las opciones que se utilizan para abrir un archivo."
type: docs
weight: 24
url: /es/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Proporciona las opciones que se utilizan para abrir un archivo.

Una instancia de esta clase se usa como parámetro en los constructores de la clase [Parser](../../com.groupdocs.parser/parser):

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

Vea los ejemplos de uso allí.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con tiempo de espera. |
|
|  | [LoadOptions()](#LoadOptions--) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vacío, FileFormat igual a FileFormat.Unknown y codificaciones predeterminadas. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con FileFormat igual a FileFormat.Unknown y codificaciones predeterminadas. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vacío y codificaciones predeterminadas. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codificaciones predeterminadas. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codificaciones personalizadas. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) totalmente personalizada. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vacío y codificaciones predeterminadas. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con contraseña y codificaciones predeterminadas. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codificaciones personalizadas. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) totalmente personalizada. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | Obtiene el formato del archivo. |
|
|  | [getFileType()](#getFileType--) | Obtiene el tipo de archivo. |
|
|  | [getPassword()](#getPassword--) | Obtiene la contraseña. |
|
|  | [getCharset()](#getCharset--) | Obtiene la codificación del documento. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | Obtiene la codificación ANSI predeterminada que se utiliza para la detección de codificaciones. |
|
|  | [getTimeout()](#getTimeout--) | Obtiene el valor que representa la cantidad de milisegundos a esperar. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con tiempo de espera.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | tiempo de espera | java.time.Duration | La Duration que representa la cantidad de milisegundos a esperar. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vacío, FileFormat igual a FileFormat.Unknown y codificaciones predeterminadas.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con FileFormat igual a FileFormat.Unknown y codificaciones predeterminadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | contraseña | java.lang.String | La contraseña para abrir el archivo protegido con contraseña. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vacío y codificaciones predeterminadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | El formato del archivo. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codificaciones predeterminadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | El formato del archivo. |
|
|  | contraseña | java.lang.String | La contraseña para abrir el archivo protegido con contraseña. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codificaciones personalizadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | El formato del archivo. |
|
|  | contraseña | java.lang.String | La contraseña para abrir el archivo protegido con contraseña. |
|
|  | conjunto de caracteres | java.nio.charset.Charset | La codificación del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codificación ANSI predeterminada que se utiliza para la detección de codificaciones. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) totalmente personalizada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | El formato del archivo. |
|
|  | contraseña | java.lang.String | La contraseña para abrir el archivo protegido con contraseña. |
|
|  | conjunto de caracteres | java.nio.charset.Charset | La codificación del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codificación ANSI predeterminada que se utiliza para la detección de codificaciones. |
|
|  | tiempo de espera | java.time.Duration | La Duration que representa la cantidad de milisegundos a esperar. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con Password vacío y codificaciones predeterminadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | El tipo de archivo. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con contraseña y codificaciones predeterminadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | El tipo de archivo. |
|
|  | contraseña | java.lang.String | La contraseña para abrir el archivo protegido con contraseña. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) con codificaciones personalizadas.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | El tipo de archivo. |
|
|  | contraseña | java.lang.String | La contraseña para abrir el archivo protegido con contraseña. |
|
|  | conjunto de caracteres | java.nio.charset.Charset | La codificación del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codificación ANSI predeterminada que se utiliza para la detección de codificaciones. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


Inicializa una nueva instancia de la clase [LoadOptions](../../com.groupdocs.parser.options/loadoptions) totalmente personalizada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | El tipo de archivo. |
|
|  | contraseña | java.lang.String | La contraseña para abrir el archivo protegido con contraseña. |
|
|  | conjunto de caracteres | java.nio.charset.Charset | La codificación del documento. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | La codificación ANSI predeterminada que se utiliza para la detección de codificaciones. |
|
|  | tiempo de espera | java.time.Duration | La Duration que representa la cantidad de milisegundos a esperar. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


Obtiene el formato del archivo.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


Obtiene el tipo de archivo.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


Obtiene la contraseña.


**Returns:**
java.lang.String - Un valor de cadena que representa una contraseña para abrir el archivo protegido con contraseña.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


Obtiene la codificación del documento.


**Returns:**
java.nio.charset.Charset - Una instancia de la clase  Charset  que representa la codificación del documento;  null  si no está establecida.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


Obtiene la codificación ANSI predeterminada que se utiliza para la detección de codificaciones.


**Returns:**
java.nio.charset.Charset - Una instancia de la clase  Charset  que representa la codificación del documento;  null  si no está establecida.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


Obtiene el valor que representa la cantidad de milisegundos a esperar.


**Returns:**
java.time.Duration - Una instancia de Duration que representa la cantidad de milisegundos a esperar.

