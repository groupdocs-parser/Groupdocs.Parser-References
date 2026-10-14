---
title: "ContainerItem"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Zip arşivi varlığı, e-posta eki, PDF Portföy öğesi vb. gibi bir konteyner öğesini temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Zip arşiv varlığı, e-posta eki, PDF Portföy öğesi vb. gibi bir konteyner öğesini temsil eder.

Bir [ContainerItem](../../com.groupdocs.parser.data/containeritem) sınıfının örneği, [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) metodunun dönüş değeri olarak kullanılır. Oradaki kullanım örneklerine bakın.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Yeni bir [ContainerItem](../../com.groupdocs.parser.data/containeritem) örneğini öğe adı ve diziniyle başlatır. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Yeni bir [ContainerItem](../../com.groupdocs.parser.data/containeritem) örneğini öğenin tam yolu ile başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getName()](#getName--) | Öğenin adını alır. |
|
|  | [getDirectory()](#getDirectory--) | Öğenin dizinini alır. |
|
|  | [getFilePath()](#getFilePath--) | Öğenin tam yolunu alır. |
|
|  | [getSize()](#getSize--) | Öğenin boyutunu alır. |
|
|  | [getMetadata()](#getMetadata--) | Meta veri öğelerinin koleksiyonunu alır. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Meta veri değerini alır. |
|
|  | [openStream()](#openStream--) | Öğe içeriğinin akışını açar. |
|
|  | [openParser()](#openParser--) | Öğe içeriği için [Parser](../../com.groupdocs.parser/parser) nesnesi oluşturur. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Öğe içeriği için [Parser](../../com.groupdocs.parser/parser) nesnesini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ile oluşturur. |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Öğe içeriği için [Parser](../../com.groupdocs.parser/parser) nesnesini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ve [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile oluşturur. |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Konteyner öğesinin dosya tipini algılar. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Yeni bir [ContainerItem](../../com.groupdocs.parser.data/containeritem) örneğini öğe adı ve diziniyle başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ad | java.lang.String | Öğenin adı. |
|
|  | dizin | java.lang.String | Öğenin dizini. |
|
|  | size | long | Öğenin boyutu. |
|
|  | meta veri | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Meta veri öğelerinin koleksiyonu. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Yeni bir [ContainerItem](../../com.groupdocs.parser.data/containeritem) örneğini öğenin tam yolu ile başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Öğenin tam yolu. |
|
|  | size | long | Öğenin boyutu. |
|
|  | meta veri | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Meta veri öğelerinin koleksiyonu. |
|

### getName() {#getName--}
```
public String getName()
```


Öğenin adını alır.


**Returns:**
java.lang.String - Öğenin dosya adını temsil eden bir dize değeri (dizin olmadan).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Öğenin dizinini alır.


**Returns:**
java.lang.String - Öğenin dizinini temsil eden bir dize değeri (dosya adı olmadan).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Öğenin tam yolunu alır.


**Returns:**
java.lang.String - Öğenin tam yolunu temsil eden bir dize değeri.

### getSize() {#getSize--}
```
public long getSize()
```


Öğenin boyutunu alır.


**Returns:**
long - Öğenin boyutunu bayt cinsinden temsil eden bir tamsayı değeri.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Meta veri öğelerinin koleksiyonunu alır.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - [MetadataItem](../../com.groupdocs.parser.data/metadataitem) nesnelerinden oluşan bir koleksiyon; meta veri ayarlanmamışsa boştur.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Meta veri değerini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | ad | java.lang.String | Meta verinin adı. |
|

**Returns:**
java.lang.String - Meta veri öğesinin değerini temsil eden bir dize değeri; bu adla meta veri bulunamazsa  null  olur.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Öğe içeriğinin akışını açar.


**Returns:**
java.io.InputStream - Öğenin içeriğini içeren bir akış.

### openParser() {#openParser--}
```
public Parser openParser()
```


Öğe içeriği için [Parser](../../com.groupdocs.parser/parser) nesnesi oluşturur.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Öğe içeriği için [Parser](../../com.groupdocs.parser/parser) nesnesini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ile oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Öğenin içeriğini açma seçenekleri. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Öğe içeriği için [Parser](../../com.groupdocs.parser/parser) nesnesini [LoadOptions](../../com.groupdocs.parser.options/loadoptions) ve [ParserSettings](../../com.groupdocs.parser.options/parsersettings) ile oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Öğenin içeriğini açma seçenekleri. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Veri çıkarımını özelleştirmek için kullanılan ayrıştırıcı ayarları. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Konteyner öğesinin dosya tipini algılar.


detectionMode
parametre, dosya türü algılamasını kontrol etme yeteneği sağlar:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Aşağıdaki örnek, kapsayıcı öğenin dosya türünün nasıl algılanacağını gösterir:

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Dosya türü algılamanın bir modunu tanımlar. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

