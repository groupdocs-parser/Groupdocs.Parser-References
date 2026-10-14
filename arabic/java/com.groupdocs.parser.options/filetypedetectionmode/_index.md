---
title: "FileTypeDetectionMode"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يحدد وضع اكتشاف نوع الملف."
type: docs
weight: 44
url: /ar/java/com.groupdocs.parser.options/filetypedetectionmode/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum FileTypeDetectionMode extends Enum<FileTypeDetectionMode>
```

يحدد وضع اكتشاف نوع الملف.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Default](#Default) | يتم اكتشاف نوع الملف بناءً على امتداد الملف؛ إذا لم يتم التعرف على الامتداد، يتم اكتشاف نوع الملف بناءً على محتوى الملف. |
|
|  | [Extension](#Extension) | يتم اكتشاف نوع الملف فقط بناءً على امتداد الملف. |
|
|  | [Content](#Content) | يتم اكتشاف نوع الملف فقط بناءً على محتوى الملف. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Default {#Default}
```
public static final FileTypeDetectionMode Default
```


يتم اكتشاف نوع الملف بناءً على امتداد الملف؛ إذا لم يتم التعرف على الامتداد، يتم اكتشاف نوع الملف بناءً على محتوى الملف.


### Extension {#Extension}
```
public static final FileTypeDetectionMode Extension
```


يتم اكتشاف نوع الملف فقط بناءً على امتداد الملف.


### Content {#Content}
```
public static final FileTypeDetectionMode Content
```


يتم اكتشاف نوع الملف فقط بناءً على محتوى الملف.


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
| المعامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[FileTypeDetectionMode](../../com.groupdocs.parser.options/filetypedetectionmode)
