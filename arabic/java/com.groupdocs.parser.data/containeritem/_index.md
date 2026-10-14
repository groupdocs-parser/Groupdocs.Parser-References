---
title: "ContainerItem"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يمثل عنصر حاوية مثل كيان أرشيف Zip أو مرفق بريد إلكتروني أو عنصر PDF Portfolio وما إلى ذلك."
type: docs
weight: 10
url: /ar/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

يمثل عنصر حاوية مثل كيان أرشيف Zip، مرفق بريد إلكتروني، عنصر PDF Portfolio وما إلى ذلك.

يتم استخدام نسخة من الفئة [ContainerItem](../../com.groupdocs.parser.data/containeritem) كقيمة إرجاع لطريقة [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--) . راجع أمثلة الاستخدام هناك.

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | يُهيئ نسخة جديدة من [ContainerItem](../../com.groupdocs.parser.data/containeritem) باستخدام اسم العنصر والمسار. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | يُهيئ نسخة جديدة من [ContainerItem](../../com.groupdocs.parser.data/containeritem) باستخدام المسار الكامل للعنصر. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getName()](#getName--) | يحصل على اسم العنصر. |
|
|  | [getDirectory()](#getDirectory--) | يحصل على مسار العنصر. |
|
|  | [getFilePath()](#getFilePath--) | يحصل على المسار الكامل للعنصر. |
|
|  | [getSize()](#getSize--) | يحصل على حجم العنصر. |
|
|  | [getMetadata()](#getMetadata--) | يحصل على مجموعة عناصر البيانات الوصفية. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | يحصل على قيمة البيانات الوصفية. |
|
|  | [openStream()](#openStream--) | يفتح تدفق محتوى العنصر. |
|
|  | [openParser()](#openParser--) | ينشئ كائن [Parser](../../com.groupdocs.parser/parser) لمحتوى العنصر. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | ينشئ كائن [Parser](../../com.groupdocs.parser/parser) لمحتوى العنصر باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | ينشئ كائن [Parser](../../com.groupdocs.parser/parser) لمحتوى العنصر باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions) و[ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | يكتشف نوع ملف عنصر الحاوية. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


يُهيئ نسخة جديدة من [ContainerItem](../../com.groupdocs.parser.data/containeritem) باستخدام اسم العنصر والمسار.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الاسم | java.lang.String | اسم العنصر. |
|
|  | المسار | java.lang.String | مسار العنصر. |
|
|  | size | long | حجم العنصر. |
|
|  | البيانات الوصفية | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | مجموعة عناصر البيانات الوصفية. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


يُهيئ نسخة جديدة من [ContainerItem](../../com.groupdocs.parser.data/containeritem) باستخدام المسار الكامل للعنصر.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | المسار الكامل للعنصر. |
|
|  | size | long | حجم العنصر. |
|
|  | البيانات الوصفية | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem} | مجموعة عناصر البيانات الوصفية. |
|

### getName() {#getName--}
```
public String getName()
```


يحصل على اسم العنصر.


**Returns:**
java.lang.String - قيمة نصية تمثل اسم ملف العنصر (بدون مسار).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


يحصل على مسار العنصر.


**Returns:**
java.lang.String - قيمة نصية تمثل مسار العنصر (بدون اسم ملف).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


يحصل على المسار الكامل للعنصر.


**Returns:**
java.lang.String - قيمة نصية تمثل المسار الكامل للعنصر.

### getSize() {#getSize--}
```
public long getSize()
```


يحصل على حجم العنصر.


**Returns:**
long - قيمة عددية تمثل حجم العنصر بالبايت.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


يحصل على مجموعة عناصر البيانات الوصفية.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - مجموعة من كائنات [MetadataItem](../../com.groupdocs.parser.data/metadataitem)؛ تكون فارغة إذا لم يتم تعيين البيانات الوصفية.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


يحصل على قيمة البيانات الوصفية.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | الاسم | java.lang.String | اسم البيانات الوصفية. |
|

**Returns:**
java.lang.String - قيمة نصية تمثل قيمة عنصر البيانات الوصفية؛  null  إذا لم يتم العثور على البيانات الوصفية بهذا الاسم.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


يفتح تدفق محتوى العنصر.


**Returns:**
java.io.InputStream - تدفق يحتوي على محتوى العنصر.

### openParser() {#openParser--}
```
public Parser openParser()
```


ينشئ كائن [Parser](../../com.groupdocs.parser/parser) لمحتوى العنصر.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


ينشئ كائن [Parser](../../com.groupdocs.parser/parser) لمحتوى العنصر باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح محتوى العنصر. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


ينشئ كائن [Parser](../../com.groupdocs.parser/parser) لمحتوى العنصر باستخدام [LoadOptions](../../com.groupdocs.parser.options/loadoptions) و[ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | الخيارات لفتح محتوى العنصر. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | إعدادات المحلل التي تُستخدم لتخصيص استخراج البيانات. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


يكتشف نوع ملف عنصر الحاوية.


detectionMode
المعلمة توفر القدرة على التحكم في اكتشاف نوع الملف:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

المثال التالي يوضح كيفية اكتشاف نوع ملف العنصر الحاوي:

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
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | يحدد وضع اكتشاف نوع الملف. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

