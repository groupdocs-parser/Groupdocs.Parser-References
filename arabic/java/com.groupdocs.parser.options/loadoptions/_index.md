---
title: "LoadOptions"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الخيارات المستخدمة لفتح ملف."
type: docs
weight: 24
url: /ar/java/com.groupdocs.parser.options/loadoptions/
---
**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

يوفر الخيارات المستخدمة لفتح ملف.

يُستخدم مثيل من هذه الفئة كمعامل في مُنشئات الفئة [Parser](../../com.groupdocs.parser/parser) :

* [Parser.Parser(java.io.InputStream, LoadOptions)](../../com.groupdocs.parser/parser#Parser-java.io.InputStream--LoadOptions-)
* [Parser.Parser(String, LoadOptions)](../../com.groupdocs.parser/parser#Parser-String--LoadOptions-)

انظر أمثلة الاستخدام هناك.

**Learn more:**

* [Loading specific file formats](../https://docs.groupdocs.com/display/parserjava/Loading+specific+file+formats)
* [Password-protected documents](../https://docs.groupdocs.com/display/parserjava/Password-protected+documents)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [LoadOptions(Duration timeout)](#LoadOptions-java.time.Duration-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع مهلة. |
|
|  | [LoadOptions()](#LoadOptions--) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور فارغة، FileFormat يساوي FileFormat.Unknown والترميزات الافتراضية. |
|
|  | [LoadOptions(String password)](#LoadOptions-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع FileFormat يساوي FileFormat.Unknown والترميزات الافتراضية. |
|
|  | [LoadOptions(FileFormat fileFormat)](#LoadOptions-com.groupdocs.parser.options.FileFormat-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور فارغة والترميزات الافتراضية. |
|
|  | [LoadOptions(FileFormat fileFormat, String password)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع الترميزات الافتراضية. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع الترميزات المخصصة. |
|
|  | [LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) المخصصة بالكامل. |
|
|  | [LoadOptions(FileType fileType)](#LoadOptions-com.groupdocs.parser.options.FileType-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور فارغة والترميزات الافتراضية. |
|
|  | [LoadOptions(FileType fileType, String password)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-) | يُنشئ مثيلاً جديدًا من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور والترميزات الافتراضية. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع الترميزات المخصصة. |
|
|  | [LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)](#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-) | ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) المخصصة بالكامل. |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getFileFormat()](#getFileFormat--) | يحصل على تنسيق الملف. |
|
|  | [getFileType()](#getFileType--) | يحصل على نوع الملف. |
|
|  | [getPassword()](#getPassword--) | يحصل على كلمة المرور. |
|
|  | [getCharset()](#getCharset--) | يحصل على ترميز المستند. |
|
|  | [getDefaultAnsiCharset()](#getDefaultAnsiCharset--) | يحصل على الترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |
|
|  | [getTimeout()](#getTimeout--) | يحصل على القيمة التي تمثل عدد المللي ثانية للانتظار. |
|
### LoadOptions(Duration timeout) {#LoadOptions-java.time.Duration-}
```
public LoadOptions(Duration timeout)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع مهلة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | مهلة | java.time.Duration | المدة التي تمثل عدد المللي ثانية للانتظار. |
|

### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور فارغة، FileFormat يساوي FileFormat.Unknown والترميزات الافتراضية.


### LoadOptions(String password) {#LoadOptions-java.lang.String-}
```
public LoadOptions(String password)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع FileFormat يساوي FileFormat.Unknown والترميزات الافتراضية.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | كلمة المرور | java.lang.String | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
|

### LoadOptions(FileFormat fileFormat) {#LoadOptions-com.groupdocs.parser.options.FileFormat-}
```
public LoadOptions(FileFormat fileFormat)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور فارغة والترميزات الافتراضية.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | تنسيق الملف. |
|

### LoadOptions(FileFormat fileFormat, String password) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-}
```
public LoadOptions(FileFormat fileFormat, String password)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع الترميزات الافتراضية.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | تنسيق الملف. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع الترميزات المخصصة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | تنسيق الملف. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
|
|  | مجموعة الأحرف | java.nio.charset.Charset | ترميز المستند. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | الترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |
|

### LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileFormat-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileFormat fileFormat, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) المخصصة بالكامل.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileFormat | [FileFormat](../../com.groupdocs.parser.options/fileformat) | تنسيق الملف. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
|
|  | مجموعة الأحرف | java.nio.charset.Charset | ترميز المستند. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | الترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |
|
|  | مهلة | java.time.Duration | المدة التي تمثل عدد المللي ثانية للانتظار. |
|

### LoadOptions(FileType fileType) {#LoadOptions-com.groupdocs.parser.options.FileType-}
```
public LoadOptions(FileType fileType)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور فارغة والترميزات الافتراضية.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | نوع الملف. |
|

### LoadOptions(FileType fileType, String password) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-}
```
public LoadOptions(FileType fileType, String password)
```


يُنشئ مثيلاً جديدًا من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع كلمة مرور والترميزات الافتراضية.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | نوع الملف. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) مع الترميزات المخصصة.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | نوع الملف. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
|
|  | مجموعة الأحرف | java.nio.charset.Charset | ترميز المستند. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | الترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |
|

### LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout) {#LoadOptions-com.groupdocs.parser.options.FileType-java.lang.String-java.nio.charset.Charset-java.nio.charset.Charset-java.time.Duration-}
```
public LoadOptions(FileType fileType, String password, Charset charset, Charset defaultAnsiCharset, Duration timeout)
```


ينشئ مثيلاً جديداً من الفئة [LoadOptions](../../com.groupdocs.parser.options/loadoptions) المخصصة بالكامل.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | fileType | [FileType](../../com.groupdocs.parser.options/filetype) | نوع الملف. |
|
|  | كلمة المرور | java.lang.String | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
|
|  | مجموعة الأحرف | java.nio.charset.Charset | ترميز المستند. |
|
|  | defaultAnsiCharset | java.nio.charset.Charset | الترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |
|
|  | مهلة | java.time.Duration | المدة التي تمثل عدد المللي ثانية للانتظار. |
|

### getFileFormat() {#getFileFormat--}
```
public FileFormat getFileFormat()
```


يحصل على تنسيق الملف.


**Returns:**
[FileFormat](../../com.groupdocs.parser.options/fileformat) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file format.

### getFileType() {#getFileType--}
```
public FileType getFileType()
```


يحصل على نوع الملف.


**Returns:**
[FileType](../../com.groupdocs.parser.options/filetype) - [FileFormat](../../com.groupdocs.parser.options/fileformat) enumeration that contains a file type.

### getPassword() {#getPassword--}
```
public String getPassword()
```


يحصل على كلمة المرور.


**Returns:**
java.lang.String - قيمة نصية تمثل كلمة مرور لفتح الملف المحمي بكلمة مرور.

### getCharset() {#getCharset--}
```
public Charset getCharset()
```


يحصل على ترميز المستند.


**Returns:**
java.nio.charset.Charset - مثيل من فئة  Charset  يمثل ترميز المستند؛  null  إذا لم يتم تعيينه.

### getDefaultAnsiCharset() {#getDefaultAnsiCharset--}
```
public Charset getDefaultAnsiCharset()
```


يحصل على الترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز.


**Returns:**
java.nio.charset.Charset - مثيل من فئة  Charset  يمثل ترميز المستند؛  null  إذا لم يتم تعيينه.

### getTimeout() {#getTimeout--}
```
public Duration getTimeout()
```


يحصل على القيمة التي تمثل عدد المللي ثانية للانتظار.


**Returns:**
java.time.Duration - مثيل من Duration يمثل عدد المللي ثانية للانتظار.

