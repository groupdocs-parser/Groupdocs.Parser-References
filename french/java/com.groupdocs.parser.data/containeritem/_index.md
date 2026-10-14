---
title: "ContainerItem"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente un élément de conteneur tel qu'une entité d'archive Zip, une pièce jointe d'e-mail, un élément de portefeuille PDF, etc."
type: docs
weight: 10
url: /fr/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Représente un élément de conteneur tel qu'une entité d'archive Zip, une pièce jointe d'e-mail, un élément de portefeuille PDF, etc.

Une instance de la classe [ContainerItem](../../com.groupdocs.parser.data/containeritem) est utilisée comme valeur de retour de la méthode [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) . Voir les exemples d'utilisation là-bas.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initialise une nouvelle instance de [ContainerItem](../../com.groupdocs.parser.data/containeritem) avec le nom de l'élément et le répertoire. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Initialise une nouvelle instance de [ContainerItem](../../com.groupdocs.parser.data/containeritem) avec le chemin complet de l'élément. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getName()](#getName--) | Obtient le nom de l'élément. |
|
|  | [getDirectory()](#getDirectory--) | Obtient le répertoire de l'élément. |
|
|  | [getFilePath()](#getFilePath--) | Obtient le chemin complet de l'élément. |
|
|  | [getSize()](#getSize--) | Obtient la taille de l'élément. |
|
|  | [getMetadata()](#getMetadata--) | Obtient la collection d'éléments de métadonnées. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Obtient la valeur de métadonnée. |
|
|  | [openStream()](#openStream--) | Ouvre le flux du contenu de l'élément. |
|
|  | [openParser()](#openParser--) | Crée l'objet [Parser](../../com.groupdocs.parser/parser) pour le contenu de l'élément. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Crée l'objet [Parser](../../com.groupdocs.parser/parser) pour le contenu de l'élément avec [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Crée l'objet [Parser](../../com.groupdocs.parser/parser) pour le contenu de l'élément avec [LoadOptions](../../com.groupdocs.parser.options/loadoptions) et [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Détecte le type de fichier de l'élément de conteneur. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Initialise une nouvelle instance de [ContainerItem](../../com.groupdocs.parser.data/containeritem) avec le nom de l'élément et le répertoire.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | nom | java.lang.String | Le nom de l'élément. |
|
|  | répertoire | java.lang.String | Le répertoire de l'élément. |
|
|  | size | long | La taille de l'élément. |
|
|  | métadonnées | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La collection d'éléments de métadonnées. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Initialise une nouvelle instance de [ContainerItem](../../com.groupdocs.parser.data/containeritem) avec le chemin complet de l'élément.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin complet de l'élément. |
|
|  | size | long | La taille de l'élément. |
|
|  | métadonnées | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | La collection d'éléments de métadonnées. |
|

### getName() {#getName--}
```
public String getName()
```


Obtient le nom de l'élément.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le nom de fichier de l'élément (sans répertoire).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Obtient le répertoire de l'élément.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le répertoire de l'élément (sans nom de fichier).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Obtient le chemin complet de l'élément.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le chemin complet de l'élément.

### getSize() {#getSize--}
```
public long getSize()
```


Obtient la taille de l'élément.


**Returns:**
long - Une valeur entière qui représente la taille de l'élément en octets.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Obtient la collection d'éléments de métadonnées.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Une collection d'objets [MetadataItem](../../com.groupdocs.parser.data/metadataitem) ; vide si les métadonnées ne sont pas définies.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Obtient la valeur de métadonnée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | nom | java.lang.String | Le nom des métadonnées. |
|

**Returns:**
java.lang.String - Une valeur de chaîne qui représente la valeur de l'élément de métadonnées ;  null  si les métadonnées avec ce nom ne sont pas trouvées.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Ouvre le flux du contenu de l'élément.


**Returns:**
java.io.InputStream - Un flux contenant le contenu de l'élément.

### openParser() {#openParser--}
```
public Parser openParser()
```


Crée l'objet [Parser](../../com.groupdocs.parser/parser) pour le contenu de l'élément.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Crée l'objet [Parser](../../com.groupdocs.parser/parser) pour le contenu de l'élément avec [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Les options pour ouvrir le contenu de l'élément. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Crée l'objet [Parser](../../com.groupdocs.parser/parser) pour le contenu de l'élément avec [LoadOptions](../../com.groupdocs.parser.options/loadoptions) et [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Les options pour ouvrir le contenu de l'élément. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Les paramètres du parseur qui sont utilisés pour personnaliser l'extraction de données. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Détecte le type de fichier de l'élément de conteneur.


detectionMode
le paramètre offre la possibilité de contrôler la détection du type de fichier :

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

L'exemple suivant montre comment détecter le type de fichier d'un élément conteneur :

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
| Parameter | Type | Description |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Définit un mode de détection du type de fichier. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

