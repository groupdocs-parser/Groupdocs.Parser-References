---
title: LoadOptions
second_title: GroupDocs.Parser for .NET API Reference
description: Initializes a new instance of the LoadOptionsgroupdocs.parser.options/loadoptions class with empty Passwordgroupdocs.parser.options/loadoptions/password FileFormatgroupdocs.parser.options/loadoptions/fileformat equal to Unknown and default encodings.
type: docs
weight: 10
url: /net/groupdocs.parser.options/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with empty [`Password`](../password), [`FileFormat`](../fileformat) equal to Unknown and default encodings.

```csharp
public LoadOptions()
```

### See Also

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | Description |
| --- | --- | --- |
| timeout | TimeSpan | The TimeSpan that represents the number of milliseconds to wait. |

### See Also

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with [`FileFormat`](../fileformat) equal to Unknown and default encodings.

```csharp
public LoadOptions(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | The password to open the password-protected file. |

### See Also

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with empty [`Password`](../password) and default encodings.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | The format of the file. |

### See Also

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with the password and default encodings.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | The format of the file. |
| password | String | The password to open the password-protected file. |

### See Also

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with custom encodings.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | The format of the file. |
| password | String | The password to open the password-protected file. |
| encoding | Encoding | The encoding of the document. |
| defaultAnsiEncoding | Encoding | The default ANSI encoding which is used for encoding detection. |

### See Also

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) fully customized class.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileFormat | FileFormat | The format of the file. |
| password | String | The password to open the password-protected file. |
| encoding | Encoding | The encoding of the document. |
| defaultAnsiEncoding | Encoding | The default ANSI encoding which is used for encoding detection. |
| timeout | TimeSpan | The TimeSpan that represents the number of milliseconds to wait. |

### See Also

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with empty [`Password`](../password) and default encodings.

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileType | FileType | The type of the file. |

### See Also

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with the password and default encodings.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileType | FileType | The type of the file. |
| password | String | The password to open the password-protected file. |

### See Also

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) class with custom encodings.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileType | FileType | The type of the file. |
| password | String | The password to open the password-protected file. |
| encoding | Encoding | The encoding of the document. |
| defaultAnsiEncoding | Encoding | The default ANSI encoding which is used for encoding detection. |

### See Also

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Initializes a new instance of the [`LoadOptions`](../../loadoptions) fully customized class.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileType | FileType | The type of the file. |
| password | String | The password to open the password-protected file. |
| encoding | Encoding | The encoding of the document. |
| defaultAnsiEncoding | Encoding | The default ANSI encoding which is used for encoding detection. |
| timeout | TimeSpan | The TimeSpan that represents the number of milliseconds to wait. |

### See Also

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
