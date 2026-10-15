---
title: "LoadOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan opsi yang digunakan untuk membuka berkas."
type: docs
weight: 420
url: /id/net/groupdocs.parser.options/loadoptions/
---

## LoadOptions class

Menyediakan opsi yang digunakan untuk membuka berkas.

```csharp
public sealed class LoadOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan [`Password`](./password) kosong, [`FileFormat`](./fileformat) bernilai Unknown, dan enkoding default. |
| [LoadOptions](loadoptions#constructor_1)(FileFormat) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan [`Password`](./password) kosong dan enkoding default. |
| [LoadOptions](loadoptions#constructor_5)(FileType) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan [`Password`](./password) kosong dan enkoding default. |
| [LoadOptions](loadoptions#constructor_9)(string) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan [`FileFormat`](./fileformat) bernilai Unknown dan enkoding default. |
| [LoadOptions](loadoptions#constructor_10)(TimeSpan) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan *timeout*. |
| [LoadOptions](loadoptions#constructor_2)(FileFormat, string) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan kata sandi dan enkoding default. |
| [LoadOptions](loadoptions#constructor_6)(FileType, string) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan kata sandi dan enkoding default. |
| [LoadOptions](loadoptions#constructor_3)(FileFormat, string, Encoding, Encoding) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan enkoding khusus. |
| [LoadOptions](loadoptions#constructor_7)(FileType, string, Encoding, Encoding) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) dengan enkoding khusus. |
| [LoadOptions](loadoptions#constructor_4)(FileFormat, string, Encoding, Encoding, TimeSpan) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) yang sepenuhnya disesuaikan. |
| [LoadOptions](loadoptions#constructor_8)(FileType, string, Encoding, Encoding, TimeSpan) | Menginisialisasi sebuah instance baru dari kelas [`LoadOptions`](../loadoptions) yang sepenuhnya disesuaikan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DefaultAnsiEncoding](../../groupdocs.parser.options/loadoptions/defaultansiencoding) { get; } | Mendapatkan enkoding ANSI default yang digunakan untuk deteksi enkoding. |
| [Encoding](../../groupdocs.parser.options/loadoptions/encoding) { get; } | Mendapatkan enkoding dokumen. |
| [FileFormat](../../groupdocs.parser.options/loadoptions/fileformat) { get; } | Mendapatkan format file. |
| [FileType](../../groupdocs.parser.options/loadoptions/filetype) { get; } | Mendapatkan tipe file. |
| [Password](../../groupdocs.parser.options/loadoptions/password) { get; } | Mendapatkan kata sandi. |
| [Timeout](../../groupdocs.parser.options/loadoptions/timeout) { get; } | Mendapatkan nilai yang mewakili jumlah milidetik untuk menunggu. |

### Catatan

Sebuah instance dari kelas ini digunakan sebagai parameter dalam konstruktor kelas [`Parser`](../../groupdocs.parser/parser):

* [`Parser`](../../groupdocs.parser/parser/parser)
* [`Parser`](../../groupdocs.parser/parser/parser)

Lihat contoh penggunaan di sana.

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)

### Lihat Juga

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
