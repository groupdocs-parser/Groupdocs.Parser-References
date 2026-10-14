---
title: "ContainerItem"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет элемент контейнера, такой как объект Zip‑архива, вложение электронной почты, элемент PDF‑портфолио и т.д."
type: docs
weight: 10
url: /ru/java/com.groupdocs.parser.data/containeritem/
---
**Inheritance:**
java.lang.Object
```
public abstract class ContainerItem
```

Представляет элемент контейнера, такой как объект Zip-архива, вложение электронной почты, элемент PDF‑портфеля и т.д.

Экземпляр класса [ContainerItem](../../com.groupdocs.parser.data/containeritem) используется в качестве возвращаемого значения метода [Parser.getContainer()](../../com.groupdocs.parser/parser#getContainer--). См. примеры использования там.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Инициализирует новый экземпляр [ContainerItem](../../com.groupdocs.parser.data/containeritem) с именем элемента и каталогом. |
|
|  | [ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)](#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--) | Инициализирует новый экземпляр [ContainerItem](../../com.groupdocs.parser.data/containeritem) с полным путём элемента. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getName()](#getName--) | Возвращает имя элемента. |
|
|  | [getDirectory()](#getDirectory--) | Возвращает каталог элемента. |
|
|  | [getFilePath()](#getFilePath--) | Возвращает полный путь элемента. |
|
|  | [getSize()](#getSize--) | Возвращает размер элемента. |
|
|  | [getMetadata()](#getMetadata--) | Возвращает коллекцию элементов метаданных. |
|
|  | [getMetadataValue(String name)](#getMetadataValue-java.lang.String-) | Возвращает значение метаданных. |
|
|  | [openStream()](#openStream--) | Открывает поток содержимого элемента. |
|
|  | [openParser()](#openParser--) | Создаёт объект [Parser](../../com.groupdocs.parser/parser) для содержимого элемента. |
|
|  | [openParser(LoadOptions loadOptions)](#openParser-com.groupdocs.parser.options.LoadOptions-) | Создаёт объект [Parser](../../com.groupdocs.parser/parser) для содержимого элемента с использованием [LoadOptions](../../com.groupdocs.parser.options/loadoptions). |
|
|  | [openParser(LoadOptions loadOptions, ParserSettings parserSettings)](#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-) | Создаёт объект [Parser](../../com.groupdocs.parser/parser) для содержимого элемента с использованием [LoadOptions](../../com.groupdocs.parser.options/loadoptions) и [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
|  | [detectFileType(FileTypeDetectionMode detectionMode)](#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-) | Определяет тип файла элемента контейнера. |
|
### ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String name, String directory, long size, Iterable<MetadataItem> metadata)
```


Инициализирует новый экземпляр [ContainerItem](../../com.groupdocs.parser.data/containeritem) с именем элемента и каталогом.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | имя | java.lang.String | Имя элемента. |
|
|  | каталог | java.lang.String | Каталог элемента. |
|
|  | size | long | Размер элемента. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Коллекция элементов метаданных. |
|

### ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata) {#ContainerItem-java.lang.String-long-java.lang.Iterable-com.groupdocs.parser.data.MetadataItem--}
```
public ContainerItem(String filePath, long size, Iterable<MetadataItem> metadata)
```


Инициализирует новый экземпляр [ContainerItem](../../com.groupdocs.parser.data/containeritem) с полным путём элемента.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Полный путь элемента. |
|
|  | size | long | Размер элемента. |
|
|  | metadata | java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> | Коллекция элементов метаданных. |
|

### getName() {#getName--}
```
public String getName()
```


Возвращает имя элемента.


**Returns:**
java.lang.String - строковое значение, представляющее имя файла элемента (без каталога).

### getDirectory() {#getDirectory--}
```
public String getDirectory()
```


Возвращает каталог элемента.


**Returns:**
java.lang.String - строковое значение, представляющее каталог элемента (без имени файла).

### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Возвращает полный путь элемента.


**Returns:**
java.lang.String - строковое значение, представляющее полный путь элемента.

### getSize() {#getSize--}
```
public long getSize()
```


Возвращает размер элемента.


**Returns:**
long - целочисленное значение, представляющее размер элемента в байтах.

### getMetadata() {#getMetadata--}
```
public Iterable<MetadataItem> getMetadata()
```


Возвращает коллекцию элементов метаданных.


**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.MetadataItem> - Коллекция объектов [MetadataItem](../../com.groupdocs.parser.data/metadataitem); пустая, если метаданные не заданы.

### getMetadataValue(String name) {#getMetadataValue-java.lang.String-}
```
public String getMetadataValue(String name)
```


Возвращает значение метаданных.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | имя | java.lang.String | Имя метаданных. |
|

**Returns:**
java.lang.String - Строковое значение, представляющее значение элемента метаданных;  null  если метаданные с этим именем не найдены.

### openStream() {#openStream--}
```
public abstract InputStream openStream()
```


Открывает поток содержимого элемента.


**Returns:**
java.io.InputStream - Поток с содержимым элемента.

### openParser() {#openParser--}
```
public Parser openParser()
```


Создаёт объект [Parser](../../com.groupdocs.parser/parser) для содержимого элемента.


**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions) {#openParser-com.groupdocs.parser.options.LoadOptions-}
```
public Parser openParser(LoadOptions loadOptions)
```


Создаёт объект [Parser](../../com.groupdocs.parser/parser) для содержимого элемента с использованием [LoadOptions](../../com.groupdocs.parser.options/loadoptions).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия содержимого элемента. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### openParser(LoadOptions loadOptions, ParserSettings parserSettings) {#openParser-com.groupdocs.parser.options.LoadOptions-com.groupdocs.parser.options.ParserSettings-}
```
public abstract Parser openParser(LoadOptions loadOptions, ParserSettings parserSettings)
```


Создаёт объект [Parser](../../com.groupdocs.parser/parser) для содержимого элемента с использованием [LoadOptions](../../com.groupdocs.parser.options/loadoptions) и [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | loadOptions | [LoadOptions](../../com.groupdocs.parser.options/loadoptions) | Параметры для открытия содержимого элемента. |
|
|  | parserSettings | [ParserSettings](../../com.groupdocs.parser.options/parsersettings) | Настройки парсера, используемые для настройки извлечения данных. |
|

**Returns:**
[Parser](../../com.groupdocs.parser/parser) - An instance of [Parser](../../com.groupdocs.parser/parser) class of the item content.

### detectFileType(FileTypeDetectionMode detectionMode) {#detectFileType-com.groupdocs.parser.options.FileTypeDetectionMode-}
```
public abstract FileType detectFileType(FileTypeDetectionMode detectionMode)
```


Определяет тип файла элемента контейнера.


detectionMode
параметр предоставляет возможность управлять определением типа файла:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

Следующий пример показывает, как определить тип файла контейнерного элемента:

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
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | detectionMode | [FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode) | Определяет режим обнаружения типа файла. |
|

**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - An instance of [FileType](../../com.groupdocs.parser.options/filetype) class; [FileType.Unknown](../../com.groupdocs.parser.options/filetype#Unknown) if a file type isn't detected.

