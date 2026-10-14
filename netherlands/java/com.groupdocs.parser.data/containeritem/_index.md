---
title: "ContainerItem"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een containeritem voor, zoals een Zip-archief, e-mailbijlage, PDF‑Portfolio-item enzovoort."
type: docs
weight: 10
url: /nl/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Stelt een containeritem voor, zoals een Zip-archief‑entiteit, e‑mailbijlage, PDF‑portfoliopost en dergelijke.

Een instantie van de klasse [ContainerItem](../../com.groupdocs.parser.data/containeritem) wordt gebruikt als retourwaarde van de methode [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--). Zie daar de gebruiksvoorbeelden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initialiseert een nieuwe instantie van [ContainerItem](../../com.groupdocs.parser.data/containeritem) met de naam en map van het item. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initialiseert een nieuwe instantie van [ContainerItem](../../com.groupdocs.parser.data/containeritem) met het volledige pad van het item. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getName()](#getName--) | Haalt de naam van het item op. |
|
|  | [getDirectory()](#getDirectory--) | Haalt de map van het item op. |
|
|  | [getFilePath()](#getFilePath--) | Haalt het volledige pad van het item op. |
|
|  | [getSize()](#getSize--) | Haalt de grootte van het item op. |
|
|  | [getMetadata()](#getMetadata--) | Haalt de verzameling metadata‑items op. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Haalt de metadata‑waarde op. |
|
|  | [openStream()](#openStream--) | Opent de stream van de iteminhoud. |
|
|  | [openParser()](#openParser--) | Maakt het [Parser](../../com.groupdocs.parser/parser)-object voor de iteminhoud. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Maakt het [Parser](../../com.groupdocs.parser/parser)-object voor de iteminhoud met [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Maakt het [Parser](../../com.groupdocs.parser/parser)-object voor de iteminhoud met [LoadOptions](../../com.groupdocs.parser.options/loadoptions) en [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Detecteert een bestandstype van het containeritem. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Initialiseert een nieuwe instantie van [ContainerItem](../../com.groupdocs.parser.data/containeritem) met de naam en map van het item.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | naam | java.lang.String | De naam van het item. |
|
|  | map | java.lang.String | De map van het item. |
|
|  | size | long | De grootte van het item. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | De verzameling metadata‑items. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Initialiseert een nieuwe instantie van [ContainerItem](../../com.groupdocs.parser.data/containeritem) met het volledige pad van het item.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het volledige pad van het item. |
|
|  | size | long | De grootte van het item. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | De verzameling metadata‑items. |
|

### getName() {#getName--}
```
public String getName()
```


Haalt de naam van het item op.


**Returns:**
java.lang.String - Een stringwaarde die de bestandsnaam van het item weergeeft (zonder een map).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Haalt de map van het item op.


**Returns:**
java.lang.String - Een stringwaarde die de map van het item weergeeft (zonder een bestandsnaam).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Haalt het volledige pad van het item op.


**Returns:**
java.lang.String - Een stringwaarde die het volledige pad van het item weergeeft.

### getSize() {#getSize--}
```
public long getSize()
```


Haalt de grootte van het item op.


**Returns:**
long - Een gehele getalwaarde die de grootte van het item in bytes weergeeft.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Haalt de verzameling metadata‑items op.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Een verzameling van [MetadataItem](../../com.groupdocs.parser.data/metadataitem) objecten; leeg als metadata niet is ingesteld.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Haalt de metadata‑waarde op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | naam | java.lang.String | De naam van de metadata. |
|

**Returns:**
java.lang.String - Een tekenreekswaarde die de waarde van het metadata-item weergeeft;  null  als de metadata met deze naam niet wordt gevonden.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Opent de stream van de iteminhoud.


**Returns:**
java.io.InputStream - Een stroom met de inhoud van het item.

### openParser() {#openParser--}
```
public Parser openParser()
```


Maakt het [Parser](../../com.groupdocs.parser/parser)-object voor de iteminhoud.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Maakt het [Parser](../../com.groupdocs.parser/parser)-object voor de iteminhoud met [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om de inhoud van het item te openen. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Maakt het [Parser](../../com.groupdocs.parser/parser)-object voor de iteminhoud met [LoadOptions](../../com.groupdocs.parser.options/loadoptions) en [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | De opties om de inhoud van het item te openen. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | De parserinstellingen die worden gebruikt om gegevensextractie aan te passen. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Detecteert een bestandstype van het containeritem.


detectionMode
parameter biedt de mogelijkheid om de bestandstype-detectie te regelen:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Het volgende voorbeeld toont hoe het bestandstype van een container-item te detecteren:

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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Definieert een modus van de bestandstype-detectie. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

