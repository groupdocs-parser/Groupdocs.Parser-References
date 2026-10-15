---
title: "LoadOptions"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يُنشئ مثلاً جديدًا من الفئة LoadOptionsgroupdocs.parser.options/loadoptions مع Passwordgroupdocs.parser.options/loadoptions/password فارغ و FileFormatgroupdocs.parser.options/loadoptions/fileformat يساوي Unknown والترميزات الافتراضية."
type: docs
weight: 10
url: /ar/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع [`Password`](../password) فارغ، و[`FileFormat`](../fileformat) يساوي Unknown والترميزات الافتراضية.

```csharp
public LoadOptions()
```

### انظر أيضًا

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| timeout | TimeSpan | الـ TimeSpan الذي يمثل عدد الملليثانية للانتظار. |

### انظر أيضًا

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع [`FileFormat`](../fileformat) يساوي Unknown والترميزات الافتراضية.

```csharp
public LoadOptions(string password)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| password | سلسلة | كلمة المرور لفتح الملف المحمي بكلمة مرور. |

### انظر أيضًا

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع [`Password`](../password) فارغ والترميزات الافتراضية.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileFormat | FileFormat | تنسيق الملف. |

### انظر أيضًا

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع كلمة المرور والترميزات الافتراضية.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileFormat | FileFormat | تنسيق الملف. |
| password | سلسلة | كلمة المرور لفتح الملف المحمي بكلمة مرور. |

### انظر أيضًا

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع ترميزات مخصصة.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileFormat | FileFormat | تنسيق الملف. |
| password | سلسلة | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
| encoding | Encoding | ترميز المستند. |
| defaultAnsiEncoding | Encoding | ترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |

### انظر أيضًا

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) المخصصة بالكامل.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileFormat | FileFormat | تنسيق الملف. |
| password | سلسلة | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
| encoding | Encoding | ترميز المستند. |
| defaultAnsiEncoding | Encoding | ترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |
| timeout | TimeSpan | الـ TimeSpan الذي يمثل عدد الملليثانية للانتظار. |

### انظر أيضًا

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع [`Password`](../password) فارغ والترميزات الافتراضية.

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileType | FileType | نوع الملف. |

### انظر أيضًا

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع كلمة المرور والترميزات الافتراضية.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileType | FileType | نوع الملف. |
| password | سلسلة | كلمة المرور لفتح الملف المحمي بكلمة مرور. |

### انظر أيضًا

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) مع ترميزات مخصصة.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileType | FileType | نوع الملف. |
| password | سلسلة | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
| encoding | Encoding | ترميز المستند. |
| defaultAnsiEncoding | Encoding | ترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |

### انظر أيضًا

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

يُنشئ مثلاً جديدًا من الفئة [`LoadOptions`](../../loadoptions) المخصصة بالكامل.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| fileType | FileType | نوع الملف. |
| password | سلسلة | كلمة المرور لفتح الملف المحمي بكلمة مرور. |
| encoding | Encoding | ترميز المستند. |
| defaultAnsiEncoding | Encoding | ترميز ANSI الافتراضي الذي يُستخدم لاكتشاف الترميز. |
| timeout | TimeSpan | الـ TimeSpan الذي يمثل عدد الملليثانية للانتظار. |

### انظر أيضًا

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
