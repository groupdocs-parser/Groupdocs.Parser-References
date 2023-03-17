---
title: Parser
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mewakili kelas utama yang mengontrol fungsi teks gambar ekstraksi penampung dan parsing.
type: docs
weight: 640
url: /id/net/groupdocs.parser/parser/
---
## Parser class

Mewakili kelas utama yang mengontrol fungsi teks, gambar, ekstraksi penampung, dan parsing.

```csharp
public sealed class Parser : IDisposable
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas untuk mengekstrak data dari database. |
| [Parser](parser#constructor)(EmailConnection) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas untuk mengekstrak data dari server email jarak jauh. |
| [Parser](parser#constructor_4)(Stream) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas. |
| [Parser](parser#constructor_8)(string) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas untuk mengekstrak data dari database. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas untuk mengekstrak data dari server email jarak jauh. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas dengan[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas dengan[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas dengan[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_11)(string, ParserSettings) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas dengan[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas dengan[`LoadOptions`](../../groupdocs.parser.options/loadoptions) dan[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Menginisialisasi instance baru dari[`Parser`](../parser) kelas dengan[`LoadOptions`](../../groupdocs.parser.options/loadoptions) dan[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Properti

| Nama | Keterangan |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Mendapatkan fitur yang didukung. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau menyetel ulang sumber daya yang tidak dikelola. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Dapatkan pratinjau halaman. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Ekstrak barcode dari dokumen. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Mengekstrak barcode dari halaman dokumen. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Ekstrak kode batang dari dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi kode batang). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Mengekstrak kode batang dari halaman dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi kode batang). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Mengekstrak objek penampung dari dokumen untuk bekerja dengan format yang berisi lampiran, arsip ZIP, dll. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Mengembalikan informasi umum tentang dokumen. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Mengekstrak teks yang diformat dari dokumen. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Mengekstrak teks yang diformat dari halaman dokumen. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Mengekstrak sorotan dari dokumen. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Mengekstrak hyperlink dari dokumen. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Mengekstrak hyperlink dari halaman dokumen. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Mengekstrak hyperlink dari dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi hyperlink). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Mengekstrak hyperlink dari halaman dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi hyperlink). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Mengekstrak gambar dari dokumen. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Mengekstrak gambar dari halaman dokumen. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Mengekstrak gambar dari dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi gambar). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Mengekstrak gambar dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Mengekstrak metadata dari dokumen. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Mengekstrak teks terstruktur dari dokumen. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Mengekstrak tabel dari dokumen. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Mengekstrak tabel dari halaman dokumen. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Mengekstrak teks dari dokumen. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Mengekstrak teks dari halaman dokumen. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Mengekstrak halaman teks dari dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Mengekstrak teks dari halaman dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks cepat mentah). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Mengekstrak area teks dari dokumen. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Mengekstrak area teks dari halaman dokumen. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Mengekstrak area teks dari dokumen menggunakan opsi penyesuaian (ekspresi reguler, huruf besar-kecil, dll.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Mengekstrak area teks dari halaman dokumen menggunakan opsi penyesuaian (ekspresi reguler, huruf besar-kecil, dll.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Mengekstrak daftar isi dari dokumen. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Mem-parsing dokumen dengan template buatan pengguna. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Mengurai formulir dokumen. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Pencarian a*keyword* dalam dokumen. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Pencarian a*keyword*dalam dokumen menggunakan opsi pencarian (ekspresi reguler, kasus pencocokan, dll.). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Mengembalikan informasi umum tentang file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Mengembalikan informasi umum tentang file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Mengembalikan informasi umum tentang file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Mengembalikan informasi umum tentang file. |

### Lihat juga

* ruang nama [GroupDocs.Parser](../../groupdocs.parser)
* perakitan [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
