---
title: "GetFileInfo"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengembalikan informasi umum tentang file."
type: docs
weight: 260
url: /id/net/groupdocs.parser/parser/getfileinfo/
---

## GetFileInfo(string) {#getfileinfo_2}

Mengembalikan informasi umum tentang file.

```csharp
public static FileInfo GetFileInfo(string filePath)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |

### Nilai Kembali

Sebuah instance dari kelas [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Contoh

Kode berikut menunjukkan cara memeriksa apakah sebuah file dilindungi kata sandi:

```csharp
// Dapatkan info file
Options.FileInfo info = Parser.GetFileInfo(filePath);
// Periksa properti IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### Lihat Juga

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(string, LoadOptions) {#getfileinfo_3}

Mengembalikan informasi umum tentang file.

```csharp
public static FileInfo GetFileInfo(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |

### Nilai Kembali

Sebuah instance dari kelas [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Contoh

Kode berikut menunjukkan cara memeriksa tipe file dari dokumen yang dilindungi kata sandi:

```csharp
// Dapatkan info file
Options.FileInfo info = Parser.GetFileInfo(filePath, new LoadOptions("password"));
// Periksa properti IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Cetak tipe file
Console.WriteLine(info.FileType.ToString());
```

### Lihat Juga

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream) {#getfileinfo}

Mengembalikan informasi umum tentang file.

```csharp
public static FileInfo GetFileInfo(Stream document)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |

### Nilai Kembali

Sebuah instance dari kelas [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Contoh

Kode berikut menunjukkan cara memeriksa apakah sebuah file dilindungi kata sandi:

```csharp
// Dapatkan info file
Options.FileInfo info = Parser.GetFileInfo(document);
// Periksa properti IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### Lihat Juga

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream, LoadOptions) {#getfileinfo_1}

Mengembalikan informasi umum tentang file.

```csharp
public static FileInfo GetFileInfo(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |

### Nilai Kembali

Sebuah instance dari kelas [`FileInfo`](../../../groupdocs.parser.options/fileinfo).

### Contoh

Kode berikut menunjukkan cara memeriksa tipe file dari dokumen yang dilindungi kata sandi:

```csharp
// Dapatkan info file
Options.FileInfo info = Parser.GetFileInfo(document);
// Periksa properti IsEncrypted
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// Cetak tipe file
Console.WriteLine(info.FileType.ToString());
```

### Lihat Juga

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
