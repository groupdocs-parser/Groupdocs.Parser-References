---
title: "ContainerItem"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt ein Containerelement dar, wie z.B. ein Zip-Archiv, eine E‑Mail‑Anlage, ein PDF‑Portfolio‑Element und so weiter."
type: docs
weight: 10
url: /de/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Stellt ein Containerelement dar, wie z. B. ein Zip‑Archiv‑Objekt, einen E‑Mail‑Anhang, ein PDF‑Portfolio‑Element und so weiter.

Eine Instanz der Klasse [ContainerItem](../../com.groupdocs.parser.data/containeritem) wird als Rückgabewert der Methode [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) verwendet. Siehe dort die Anwendungsbeispiele.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initialisiert eine neue Instanz von [ContainerItem](../../com.groupdocs.parser.data/containeritem) mit dem Namen und dem Verzeichnis des Elements. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initialisiert eine neue Instanz von [ContainerItem](../../com.groupdocs.parser.data/containeritem) mit dem vollständigen Pfad des Elements. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getName()](#getName--) | Ruft den Namen des Elements ab. |
|
|  | [getDirectory()](#getDirectory--) | Ruft das Verzeichnis des Elements ab. |
|
|  | [getFilePath()](#getFilePath--) | Ruft den vollständigen Pfad des Elements ab. |
|
|  | [getSize()](#getSize--) | Ruft die Größe des Elements ab. |
|
|  | [getMetadata()](#getMetadata--) | Ruft die Sammlung von Metadaten‑Elementen ab. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Ruft den Metadatenwert ab. |
|
|  | [openStream()](#openStream--) | Öffnet den Stream des Elementinhalts. |
|
|  | [openParser()](#openParser--) | Erstellt das [Parser](../../com.groupdocs.parser/parser)-Objekt für den Inhalt des Elements. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Erstellt das [Parser](../../com.groupdocs.parser/parser)-Objekt für den Inhalt des Elements mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Erstellt das [Parser](../../com.groupdocs.parser/parser)-Objekt für den Inhalt des Elements mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions) und [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Ermittelt den Dateityp des Container-Elements. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Initialisiert eine neue Instanz von [ContainerItem](../../com.groupdocs.parser.data/containeritem) mit dem Namen und dem Verzeichnis des Elements.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Name | java.lang.String | Der Name des Elements. |
|
|  | Verzeichnis | java.lang.String | Das Verzeichnis des Elements. |
|
|  | size | long | Die Größe des Elements. |
|
|  | Metadaten | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Die Sammlung von Metadaten-Elementen. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Initialisiert eine neue Instanz von [ContainerItem](../../com.groupdocs.parser.data/containeritem) mit dem vollständigen Pfad des Elements.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der vollständige Pfad des Elements. |
|
|  | size | long | Die Größe des Elements. |
|
|  | Metadaten | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Die Sammlung von Metadaten-Elementen. |
|

### getName() {#getName--}
```
public String getName()
```


Ruft den Namen des Elements ab.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den Dateinamen des Elements (ohne Verzeichnis) darstellt.

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Ruft das Verzeichnis des Elements ab.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der das Verzeichnis des Elements (ohne Dateinamen) darstellt.

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Ruft den vollständigen Pfad des Elements ab.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den vollständigen Pfad des Elements darstellt.

### getSize() {#getSize--}
```
public long getSize()
```


Ruft die Größe des Elements ab.


**Returns:**
long - Ein ganzzahliger Wert, der die Größe des Elements in Bytes darstellt.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Ruft die Sammlung von Metadaten‑Elementen ab.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Eine Sammlung von [MetadataItem](../../com.groupdocs.parser.data/metadataitem)-Objekten; leer, wenn Metadaten nicht gesetzt sind.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Ruft den Metadatenwert ab.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Name | java.lang.String | Der Name der Metadaten. |
|

**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den Wert des Metadaten-Elements darstellt;  null  wenn die Metadaten mit diesem Namen nicht gefunden werden.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Öffnet den Stream des Elementinhalts.


**Returns:**
java.io.InputStream - Ein Stream mit dem Inhalt des Elements.

### openParser() {#openParser--}
```
public Parser openParser()
```


Erstellt das [Parser](../../com.groupdocs.parser/parser)-Objekt für den Inhalt des Elements.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Erstellt das [Parser](../../com.groupdocs.parser/parser)-Objekt für den Inhalt des Elements mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen des Inhalts des Elements. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Erstellt das [Parser](../../com.groupdocs.parser/parser)-Objekt für den Inhalt des Elements mit [LoadOptions](../../com.groupdocs.parser.options/loadoptions) und [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Die Optionen zum Öffnen des Inhalts des Elements. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Die Parser-Einstellungen, die zum Anpassen der Datenerfassung verwendet werden. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Ermittelt den Dateityp des Container-Elements.


detectionMode
Parameter bietet die Möglichkeit, die Dateityp-Erkennung zu steuern:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Das folgende Beispiel zeigt, wie der Dateityp des Container-Elements ermittelt wird:

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Definiert einen Modus der Dateityp-Erkennung. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

