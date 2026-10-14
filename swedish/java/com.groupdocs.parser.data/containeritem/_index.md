---
title: "ContainerItem"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett containerobjekt som Zip-arkiv, e-postbilaga, PDF-portföljobjekt osv."
type: docs
weight: 10
url: /sv/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Representerar ett containerobjekt som Zip-arkivpost, e-postbilaga, PDF‑portföljobjekt och så vidare.

En instans av [ContainerItem](../../com.groupdocs.parser.data/containeritem)-klassen används som returvärde för [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--)‑metoden. Se användningsexemplen där.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initierar en ny instans av [ContainerItem](../../com.groupdocs.parser.data/containeritem) med objektets namn och katalog. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initierar en ny instans av [ContainerItem](../../com.groupdocs.parser.data/containeritem) med objektets fullständiga sökväg. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getName()](#getName--) | Hämtar objektets namn. |
|
|  | [getDirectory()](#getDirectory--) | Hämtar objektets katalog. |
|
|  | [getFilePath()](#getFilePath--) | Hämtar objektets fullständiga sökväg. |
|
|  | [getSize()](#getSize--) | Hämtar objektets storlek. |
|
|  | [getMetadata()](#getMetadata--) | Hämtar samlingen av metadataobjekt. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Hämtar metadata‑värdet. |
|
|  | [openStream()](#openStream--) | Öppnar strömmen för objektets innehåll. |
|
|  | [openParser()](#openParser--) | Skapar [Parser](../../com.groupdocs.parser/parser)-objektet för objektets innehåll. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Skapar [Parser](../../com.groupdocs.parser/parser)-objektet för objektets innehåll med [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Skapar [Parser](../../com.groupdocs.parser/parser)-objektet för objektets innehåll med [LoadOptions](../../com.groupdocs.parser.options/loadoptions) och [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Detekterar en filtyp för containerobjektet. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Initierar en ny instans av [ContainerItem](../../com.groupdocs.parser.data/containeritem) med objektets namn och katalog.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | namn | java.lang.String | Namnet på objektet. |
|
|  | katalog | java.lang.String | Katalogen för objektet. |
|
|  | size | long | Storleken på objektet. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Samlingen av metadataobjekt. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Initierar en ny instans av [ContainerItem](../../com.groupdocs.parser.data/containeritem) med objektets fullständiga sökväg.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Den fullständiga sökvägen för objektet. |
|
|  | size | long | Storleken på objektet. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Samlingen av metadataobjekt. |
|

### getName() {#getName--}
```
public String getName()
```


Hämtar objektets namn.


**Returns:**
java.lang.String - Ett strängvärde som representerar filnamnet för objektet (utan en katalog).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Hämtar objektets katalog.


**Returns:**
java.lang.String - Ett strängvärde som representerar katalogen för objektet (utan ett filnamn).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Hämtar objektets fullständiga sökväg.


**Returns:**
java.lang.String - Ett strängvärde som representerar den fullständiga sökvägen för objektet.

### getSize() {#getSize--}
```
public long getSize()
```


Hämtar objektets storlek.


**Returns:**
long - Ett heltalsvärde som representerar storleken på objektet i byte.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Hämtar samlingen av metadataobjekt.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - En samling av [MetadataItem](../../com.groupdocs.parser.data/metadataitem) objekt; tom om metadata inte har satts.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Hämtar metadata‑värdet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | namn | java.lang.String | Namnet på metadata. |
|

**Returns:**
java.lang.String - Ett strängvärde som representerar värdet för metadataobjektet; null om metadata med detta namn inte hittas.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Öppnar strömmen för objektets innehåll.


**Returns:**
java.io.InputStream - En ström med objektets innehåll.

### openParser() {#openParser--}
```
public Parser openParser()
```


Skapar [Parser](../../com.groupdocs.parser/parser)-objektet för objektets innehåll.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Skapar [Parser](../../com.groupdocs.parser/parser)-objektet för objektets innehåll med [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna objektets innehåll. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Skapar [Parser](../../com.groupdocs.parser/parser)-objektet för objektets innehåll med [LoadOptions](../../com.groupdocs.parser.options/loadoptions) och [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Alternativen för att öppna objektets innehåll. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Parserinställningarna som används för att anpassa dataextraktion. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Detekterar en filtyp för containerobjektet.


detectionMode
parametern ger möjlighet att kontrollera filtypdetektering:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Följande exempel visar hur man detekterar filtypen för containerobjektet:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Definierar ett läge för filtypdetektering. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

