---
title: "ContainerItem"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un elemento contenitore come entità di archivio Zip, allegato email, elemento PDF Portfolio e così via."
type: docs
weight: 10
url: /it/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Rappresenta un elemento contenitore come entità di archivio Zip, allegato email, elemento PDF Portfolio e così via.

Un'istanza della classe [ContainerItem](../../com.groupdocs.parser.data/containeritem) è usata come valore di ritorno del metodo [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--). Vedi gli esempi d'uso lì.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Inizializza una nuova istanza di [ContainerItem](../../com.groupdocs.parser.data/containeritem) con il nome e la directory dell'elemento. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Inizializza una nuova istanza di [ContainerItem](../../com.groupdocs.parser.data/containeritem) con il percorso completo dell'elemento. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getName()](#getName--) | Restituisce il nome dell'elemento. |
|
|  | [getDirectory()](#getDirectory--) | Restituisce la directory dell'elemento. |
|
|  | [getFilePath()](#getFilePath--) | Restituisce il percorso completo dell'elemento. |
|
|  | [getSize()](#getSize--) | Restituisce la dimensione dell'elemento. |
|
|  | [getMetadata()](#getMetadata--) | Restituisce la collezione di elementi di metadati. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Restituisce il valore del metadato. |
|
|  | [openStream()](#openStream--) | Apre lo stream del contenuto dell'elemento. |
|
|  | [openParser()](#openParser--) | Crea l'oggetto [Parser](../../com.groupdocs.parser/parser) per il contenuto dell'elemento. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Crea l'oggetto [Parser](../../com.groupdocs.parser/parser) per il contenuto dell'elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Crea l'oggetto [Parser](../../com.groupdocs.parser/parser) per il contenuto dell'elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) e [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Rileva il tipo di file dell'elemento contenitore. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Inizializza una nuova istanza di [ContainerItem](../../com.groupdocs.parser.data/containeritem) con il nome e la directory dell'elemento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | name | java.lang.String | Il nome dell'elemento. |
|
|  | directory | java.lang.String | La directory dell'elemento. |
|
|  | size | long | La dimensione dell'elemento. |
|
|  | metadati | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La collezione di elementi di metadati. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Inizializza una nuova istanza di [ContainerItem](../../com.groupdocs.parser.data/containeritem) con il percorso completo dell'elemento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso completo dell'elemento. |
|
|  | size | long | La dimensione dell'elemento. |
|
|  | metadati | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La collezione di elementi di metadati. |
|

### getName() {#getName--}
```
public String getName()
```


Restituisce il nome dell'elemento.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il nome file dell'elemento (senza una directory).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Restituisce la directory dell'elemento.


**Returns:**
java.lang.String - Un valore stringa che rappresenta la directory dell'elemento (senza un nome file).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Restituisce il percorso completo dell'elemento.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il percorso completo dell'elemento.

### getSize() {#getSize--}
```
public long getSize()
```


Restituisce la dimensione dell'elemento.


**Returns:**
long - Un valore intero che rappresenta la dimensione dell'elemento in byte.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Restituisce la collezione di elementi di metadati.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Una collezione di oggetti [MetadataItem](../../com.groupdocs.parser.data/metadataitem); vuota se i metadati non sono impostati.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Restituisce il valore del metadato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | name | java.lang.String | Il nome del metadato. |
|

**Returns:**
java.lang.String - Un valore stringa che rappresenta il valore dell'elemento di metadati;  null  se il metadato con questo nome non viene trovato.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Apre lo stream del contenuto dell'elemento.


**Returns:**
java.io.InputStream - Un flusso con il contenuto dell'elemento.

### openParser() {#openParser--}
```
public Parser openParser()
```


Crea l'oggetto [Parser](../../com.groupdocs.parser/parser) per il contenuto dell'elemento.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Crea l'oggetto [Parser](../../com.groupdocs.parser/parser) per il contenuto dell'elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il contenuto dell'elemento. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Crea l'oggetto [Parser](../../com.groupdocs.parser/parser) per il contenuto dell'elemento con [LoadOptions](../../com.groupdocs.parser.options/loadoptions) e [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Le opzioni per aprire il contenuto dell'elemento. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Le impostazioni del parser utilizzate per personalizzare l'estrazione dei dati. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Rileva il tipo di file dell'elemento contenitore.


detectionMode
parameter fornisce la possibilità di controllare il rilevamento del tipo di file:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Il seguente esempio mostra come rilevare il tipo di file dell'elemento contenitore:

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Definisce una modalità di rilevamento del tipo di file. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

