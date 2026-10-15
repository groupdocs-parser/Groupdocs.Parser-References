---
title: "LoadOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi instance baru dari kelas LoadOptionsgroupdocs.parser.options/loadoptions dengan Passwordgroupdocs.parser.options/loadoptions/password kosong, FileFormatgroupdocs.parser.options/loadoptions/fileformat sama dengan Unknown, dan pengkodean default."
type: docs
weight: 10
url: /id/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan [`Password`](../password) kosong, [`FileFormat`](../fileformat) sama dengan Unknown, dan pengkodean default.

```csharp
public LoadOptions()
```

### Lihat Juga

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan *timeout*.

```csharp
public LoadOptions(TimeSpan timeout)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| timeout | TimeSpan | TimeSpan yang mewakili jumlah milidetik yang harus ditunggu. |

### Lihat Juga

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan [`FileFormat`](../fileformat) sama dengan Unknown, dan pengkodean default.

```csharp
public LoadOptions(string password)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| password | String | Kata sandi untuk membuka file yang dilindungi kata sandi. |

### Lihat Juga

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan [`Password`](../password) kosong, dan pengkodean default.

```csharp
public LoadOptions(FileFormat fileFormat)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileFormat | FileFormat | Format file. |

### Lihat Juga

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan kata sandi dan pengkodean default.

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileFormat | FileFormat | Format file. |
| password | String | Kata sandi untuk membuka file yang dilindungi kata sandi. |

### Lihat Juga

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan pengkodean khusus.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileFormat | FileFormat | Format file. |
| password | String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
| encoding | Encoding | Pengkodean dokumen. |
| defaultAnsiEncoding | Encoding | Pengkodean ANSI default yang digunakan untuk deteksi pengkodean. |

### Lihat Juga

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) yang sepenuhnya disesuaikan.

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileFormat | FileFormat | Format file. |
| password | String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
| encoding | Encoding | Pengkodean dokumen. |
| defaultAnsiEncoding | Encoding | Pengkodean ANSI default yang digunakan untuk deteksi pengkodean. |
| timeout | TimeSpan | TimeSpan yang mewakili jumlah milidetik yang harus ditunggu. |

### Lihat Juga

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan [`Password`](../password) kosong, dan pengkodean default.

```csharp
public LoadOptions(FileType fileType)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileType | FileType | Tipe file. |

### Lihat Juga

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan kata sandi dan pengkodean default.

```csharp
public LoadOptions(FileType fileType, string password)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileType | FileType | Tipe file. |
| password | String | Kata sandi untuk membuka file yang dilindungi kata sandi. |

### Lihat Juga

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) dengan pengkodean khusus.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileType | FileType | Tipe file. |
| password | String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
| encoding | Encoding | Pengkodean dokumen. |
| defaultAnsiEncoding | Encoding | Pengkodean ANSI default yang digunakan untuk deteksi pengkodean. |

### Lihat Juga

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

Menginisialisasi instance baru dari kelas [`LoadOptions`](../../loadoptions) yang sepenuhnya disesuaikan.

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| fileType | FileType | Tipe file. |
| password | String | Kata sandi untuk membuka file yang dilindungi kata sandi. |
| encoding | Encoding | Pengkodean dokumen. |
| defaultAnsiEncoding | Encoding | Pengkodean ANSI default yang digunakan untuk deteksi pengkodean. |
| timeout | TimeSpan | TimeSpan yang mewakili jumlah milidetik yang harus ditunggu. |

### Lihat Juga

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
