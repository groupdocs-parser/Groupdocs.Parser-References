---
title: "PageImageArea"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mewakili area gambar halaman yang digunakan untuk mewakili gambar pada halaman dalam fungsi parsing dengan templat atau lampiran gambar jika gambar diekstrak dari email atau arsip Zip."
type: docs
weight: 830
url: /id/net/groupdocs.parser.data/pageimagearea/
---

## PageImageArea class

Mewakili area gambar halaman yang digunakan untuk mewakili gambar pada halaman dalam fungsi parsing dengan templat atau lampiran gambar jika gambar diekstrak dari email atau arsip Zip.

```csharp
public sealed class PageImageArea : PageArea
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageImageArea](pageimagearea#constructor)(Stream, FileType, double) | Menginisialisasi instance baru dari kelas [`PageImageArea`](../pageimagearea). |
| [PageImageArea](pageimagearea#constructor_1)(Stream, FileType, double, Page, Rectangle) | Menginisialisasi instance baru dari kelas [`PageImageArea`](../pageimagearea). |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [FileType](../../groupdocs.parser.data/pageimagearea/filetype) { get; } | Mendapatkan format gambar. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Mendapatkan informasi halaman dokumen seperti indeks halaman dan ukuran halaman. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Mendapatkan area persegi panjang. |
| [Rotation](../../groupdocs.parser.data/pageimagearea/rotation) { get; } | Mendapatkan sudut rotasi gambar. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream)() | Mengembalikan aliran gambar. |
| [GetImageStream](../../groupdocs.parser.data/pageimagearea/getimagestream#getimagestream_1)(ImageOptions) | Mengembalikan aliran gambar dalam format yang berbeda. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save)(string) | Menyimpan gambar ke file. |
| [Save](../../groupdocs.parser.data/pageimagearea/save#save_1)(string, ImageOptions) | Menyimpan gambar ke file dalam format yang berbeda. |

### Catatan

Sebuah instance dari [`PageImageArea`](../pageimagearea) kelas digunakan sebagai nilai kembali dari metode berikut:

* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)
* [`GetImages`](../../groupdocs.parser/parser/getimages)

Lihat contoh penggunaan di sana.

### Lihat Juga

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
