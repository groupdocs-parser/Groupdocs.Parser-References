---
title: "LoadOptions"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "初始化 LoadOptionsgroupdocs.parser.options/loadoptions 类的新实例，Passwordgroupdocs.parser.options/loadoptions/password 为空，FileFormatgroupdocs.parser.options/loadoptions/fileformat 等于 Unknown，并使用默认编码。"
type: docs
weight: 10
url: /zh/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，[`Password`](../password) 为空，[`FileFormat`](../fileformat) 等于 Unknown，并使用默认编码。

```csharp
public LoadOptions()
```

### 另请参见

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，使用 *timeout*。

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 超时 | TimeSpan | 表示等待毫秒数的 TimeSpan。 |

### 另请参见

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，[`FileFormat`](../fileformat) 等于 Unknown，并使用默认编码。

```csharp
public LoadOptions(string password)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 密码 | 字符串 | 用于打开受密码保护文件的密码。 |

### 另请参见

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，[`Password`](../password) 为空，并使用默认编码。

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileFormat | FileFormat | 文件的格式。 |

### 另请参见

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，使用密码并使用默认编码。

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileFormat | FileFormat | 文件的格式。 |
| 密码 | 字符串 | 用于打开受密码保护文件的密码。 |

### 另请参见

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，使用自定义编码。

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileFormat | FileFormat | 文件的格式。 |
| 密码 | 字符串 | 用于打开受密码保护文件的密码。 |
| encoding | Encoding | 文档的编码。 |
| defaultAnsiEncoding | Encoding | 用于编码检测的默认 ANSI 编码。 |

### 另请参见

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

初始化完全自定义的 [`LoadOptions`](../../loadoptions) 类的新实例。

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileFormat | FileFormat | 文件的格式。 |
| 密码 | 字符串 | 用于打开受密码保护文件的密码。 |
| encoding | Encoding | 文档的编码。 |
| defaultAnsiEncoding | Encoding | 用于编码检测的默认 ANSI 编码。 |
| 超时 | TimeSpan | 表示等待毫秒数的 TimeSpan。 |

### 另请参见

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，[`Password`](../password) 为空，并使用默认编码。

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileType | FileType | 文件的类型。 |

### 另请参见

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，使用密码并使用默认编码。

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileType | FileType | 文件的类型。 |
| 密码 | 字符串 | 用于打开受密码保护文件的密码。 |

### 另请参见

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

初始化 [`LoadOptions`](../../loadoptions) 类的新实例，使用自定义编码。

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileType | FileType | 文件的类型。 |
| 密码 | 字符串 | 用于打开受密码保护文件的密码。 |
| encoding | Encoding | 文档的编码。 |
| defaultAnsiEncoding | Encoding | 用于编码检测的默认 ANSI 编码。 |

### 另请参见

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

初始化完全自定义的 [`LoadOptions`](../../loadoptions) 类的新实例。

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| fileType | FileType | 文件的类型。 |
| 密码 | 字符串 | 用于打开受密码保护文件的密码。 |
| encoding | Encoding | 文档的编码。 |
| defaultAnsiEncoding | Encoding | 用于编码检测的默认 ANSI 编码。 |
| 超时 | TimeSpan | 表示等待毫秒数的 TimeSpan。 |

### 另请参见

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
