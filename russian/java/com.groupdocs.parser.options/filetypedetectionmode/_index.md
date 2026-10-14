---
title: "FileTypeDetectionMode"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Определяет режим обнаружения типа файла."
type: docs
weight: 44
url: /ru/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

Определяет режим обнаружения типа файла.

## Поля

| Поле | Описание |
| --- | --- |
|  | [Default](#Default) | Тип файла определяется по расширению файла; если расширение файла не распознано, тип файла определяется по содержимому файла. |
|
|  | [Extension](#Extension) | Тип файла определяется только по расширению файла. |
|
|  | [Content](#Content) | Тип файла определяется только по содержимому файла. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


Тип файла определяется по расширению файла; если расширение файла не распознано, тип файла определяется по содержимому файла.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


Тип файла определяется только по расширению файла.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


Тип файла определяется только по содержимому файла.


### values() {#values--}
```
public static FileTypeDetectionMode[] values()
```




**Returns:**
com.groupdocs.parser.options.FileTypeDetectionMode[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static FileTypeDetectionMode valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)
