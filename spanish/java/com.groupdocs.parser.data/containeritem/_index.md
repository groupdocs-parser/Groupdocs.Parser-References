---
title: "ContainerItem"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un elemento de contenedor como entidad de archivo Zip, adjunto de correo electrónico, elemento de PDF Portfolio, etc."
type: docs
weight: 10
url: /es/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Representa un elemento contenedor como una entidad de archivo Zip, un adjunto de correo electrónico, un elemento de PDF Portfolio, etc.

Una instancia de la clase [ContainerItem](../../com.groupdocs.parser.data/containeritem) se usa como valor de retorno del método [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--). Consulte los ejemplos de uso allí.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Inicializa una nueva instancia de [ContainerItem](../../com.groupdocs.parser.data/containeritem) con el nombre y el directorio del elemento. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Inicializa una nueva instancia de [ContainerItem](../../com.groupdocs.parser.data/containeritem) con la ruta completa del elemento. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getName()](#getName--) | Obtiene el nombre del elemento. |
|
|  | [getDirectory()](#getDirectory--) | Obtiene el directorio del elemento. |
|
|  | [getFilePath()](#getFilePath--) | Obtiene la ruta completa del elemento. |
|
|  | [getSize()](#getSize--) | Obtiene el tamaño del elemento. |
|
|  | [getMetadata()](#getMetadata--) | Obtiene la colección de elementos de metadatos. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Obtiene el valor del metadato. |
|
|  | [openStream()](#openStream--) | Abre el flujo del contenido del elemento. |
|
|  | [openParser()](#openParser--) | Crea el objeto [Parser](../../com.groupdocs.parser/parser) para el contenido del elemento. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Crea el objeto [Parser](../../com.groupdocs.parser/parser) para el contenido del elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Crea el objeto [Parser](../../com.groupdocs.parser/parser) para el contenido del elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) y [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Detecta el tipo de archivo del elemento del contenedor. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Inicializa una nueva instancia de [ContainerItem](../../com.groupdocs.parser.data/containeritem) con el nombre y el directorio del elemento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | nombre | java.lang.String | El nombre del elemento. |
|
|  | directorio | java.lang.String | El directorio del elemento. |
|
|  | size | long | El tamaño del elemento. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La colección de elementos de metadatos. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Inicializa una nueva instancia de [ContainerItem](../../com.groupdocs.parser.data/containeritem) con la ruta completa del elemento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta completa del elemento. |
|
|  | size | long | El tamaño del elemento. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La colección de elementos de metadatos. |
|

### getName() {#getName--}
```
public String getName()
```


Obtiene el nombre del elemento.


**Returns:**
java.lang.String - Un valor de cadena que representa el nombre de archivo del elemento (sin un directorio).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Obtiene el directorio del elemento.


**Returns:**
java.lang.String - Un valor de cadena que representa el directorio del elemento (sin un nombre de archivo).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Obtiene la ruta completa del elemento.


**Returns:**
java.lang.String - Un valor de cadena que representa la ruta completa del elemento.

### getSize() {#getSize--}
```
public long getSize()
```


Obtiene el tamaño del elemento.


**Returns:**
long - Un valor entero que representa el tamaño del elemento en bytes.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Obtiene la colección de elementos de metadatos.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Una colección de objetos [MetadataItem](../../com.groupdocs.parser.data/metadataitem); vacía si los metadatos no están establecidos.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Obtiene el valor del metadato.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | nombre | java.lang.String | El nombre de los metadatos. |
|

**Returns:**
java.lang.String - Un valor de cadena que representa el valor del elemento de metadatos;  null  si no se encuentra el metadato con este nombre.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Abre el flujo del contenido del elemento.


**Returns:**
java.io.InputStream - Un flujo con el contenido del elemento.

### openParser() {#openParser--}
```
public Parser openParser()
```


Crea el objeto [Parser](../../com.groupdocs.parser/parser) para el contenido del elemento.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Crea el objeto [Parser](../../com.groupdocs.parser/parser) para el contenido del elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Las opciones para abrir el contenido del elemento. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Crea el objeto [Parser](../../com.groupdocs.parser/parser) para el contenido del elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) y [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Las opciones para abrir el contenido del elemento. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | La configuración del analizador que se utiliza para personalizar la extracción de datos. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Detecta el tipo de archivo del elemento del contenedor.


detectionMode
El parámetro proporciona la capacidad de controlar la detección del tipo de archivo:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

El siguiente ejemplo muestra cómo detectar el tipo de archivo del elemento contenedor:

````
// Create an instance of Parser class
 try (Parser parser = new Parser(filePath)) {
     // Extract attachments from the container
     Iterable attachments = parser.getContainer();
     // Check if container extraction is supported
     if (attachments == null) {
         System.out.println("Container extraction isn't supported");
     }
     // Iterate over attachments
     for (ContainerItem item : attachments) {
         // Detect the file type
         FileType fileType = item.detectFileType(FileTypeDetectionMode.Default);
         // Print the name and file type
         System.out.println(String.format("%s: %s", item.getName(), fileType));
     }
 }
 
````



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Define un modo de detección del tipo de archivo. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

