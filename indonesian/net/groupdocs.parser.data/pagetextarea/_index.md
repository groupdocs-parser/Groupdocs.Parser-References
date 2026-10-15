---
title: "PageTextArea"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mewakili area teks halaman yang digunakan untuk mewakili nilai teks dalam fungsi parsing dengan templat atau parsing formulir."
type: docs
weight: 860
url: /id/net/groupdocs.parser.data/pagetextarea/
---

## PageTextArea class

Mewakili area teks halaman yang digunakan untuk mewakili nilai teks dalam fungsi parsing dengan templat atau parsing formulir.

```csharp
public sealed class PageTextArea : PageArea
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageTextArea](pagetextarea#constructor)(IEnumerable&lt;PageTextArea&gt;, Page) | Menginisialisasi sebuah instance baru dari [`PageTextArea`](../pagetextarea) kelas. |
| [PageTextArea](pagetextarea#constructor_1)(string, Page, Rectangle) | Menginisialisasi sebuah instance baru dari [`PageTextArea`](../pagetextarea) kelas. |
| [PageTextArea](pagetextarea#constructor_2)(string, double?, TextStyle, Page, Rectangle) | Menginisialisasi sebuah instance baru dari [`PageTextArea`](../pagetextarea) kelas. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Areas](../../groupdocs.parser.data/pagetextarea/areas) { get; } | Mendapatkan koleksi area halaman teks anak. |
| [BaseLine](../../groupdocs.parser.data/pagetextarea/baseline) { get; } | Mendapatkan garis dasar. |
| [Page](../../groupdocs.parser.data/pagearea/page) { get; } | Mendapatkan informasi halaman dokumen seperti indeks halaman dan ukuran halaman. |
| [Rectangle](../../groupdocs.parser.data/pagearea/rectangle) { get; } | Mendapatkan area persegi panjang. |
| [Text](../../groupdocs.parser.data/pagetextarea/text) { get; } | Mendapatkan teks. |
| [TextStyle](../../groupdocs.parser.data/pagetextarea/textstyle) { get; } | Mendapatkan gaya teks seperti ukuran font, nama font, dan seterusnya. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [ToString](../../groupdocs.parser.data/pagetextarea/tostring)() | Mengonversi nilai instance ini menjadi String. |

### Catatan

Sebuah instance dari [`PageTextArea`](../pagetextarea) kelas digunakan sebagai nilai kembali dari metode berikut:

* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)
* [`GetTextAreas`](../../groupdocs.parser/parser/gettextareas)

Juga sebuah instance dari [`PageTextArea`](../pagetextarea) kelas digunakan sebagai nilai properti [`PageArea`](../fielddata/pagearea).

Lihat contoh penggunaan di sana.

Area teks dapat berupa tunggal atau komposit. Pada kasus pertama, ia berisi teks yang dibatasi oleh area persegi panjang. Pada kasus kedua, ia berisi area teks lain; properti teks dan tabel dihitung oleh area teks anak.

### Lihat Juga

* class [PageArea](../pagearea)
* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
