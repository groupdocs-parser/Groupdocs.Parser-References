---
title: "Pengurai"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mewakili kelas utama yang mengontrol ekstraksi kontainer gambar teks dan fungsionalitas penguraian."
type: docs
weight: 30
url: /id/net/groupdocs.parser/parser/
---

## Parser class

Mewakili kelas utama yang mengendalikan fungsi ekstraksi dan parsing teks, gambar, serta kontainer.

```csharp
public sealed class Parser : IDisposable
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari basis data. |
| [Parser](parser#constructor)(EmailConnection) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari server email jarak jauh. |
| [Parser](parser#constructor_4)(Stream) | Menginisialisasi instance baru dari kelas [`Parser`](../parser). |
| [Parser](parser#constructor_8)(string) | Menginisialisasi instance baru dari kelas [`Parser`](../parser). |
| [Parser](parser#constructor_12)(Uri) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari sebuah URI. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari basis data. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari server email jarak jauh. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) dengan [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_7)(Stream, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) dengan [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_9)(string, LoadOptions) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) dengan [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [Parser](parser#constructor_11)(string, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) dengan [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_13)(Uri, LoadOptions) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari sebuah URI dengan *loadOptions*. |
| [Parser](parser#constructor_15)(Uri, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari sebuah URI dengan *parserSettings*. |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) dengan [`LoadOptions`](../../groupdocs.parser.options/loadoptions) dan [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_10)(string, LoadOptions, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) dengan [`LoadOptions`](../../groupdocs.parser.options/loadoptions) dan [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [Parser](parser#constructor_14)(Uri, LoadOptions, ParserSettings) | Menginisialisasi instance baru dari kelas [`Parser`](../parser) untuk mengekstrak data dari sebuah URI dengan *loadOptions* dan *parserSettings*. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Mendapatkan fitur yang didukung. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Melakukan tugas yang ditentukan aplikasi terkait dengan membebaskan, melepaskan, atau mereset sumber daya yang tidak dikelola. |
| [GenerateAdjustmentFields](../../groupdocs.parser/parser/generateadjustmentfields)(AdjustmentFieldsOptions) | Menghasilkan bidang untuk penyesuaian otomatis posisi dan skala templat. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Dapatkan pratinjau halaman. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations)() | Mengekstrak anotasi dari dokumen. Perhatikan bahwa hanya format PDF yang saat ini didukung. |
| [GetAnnotations](../../groupdocs.parser/parser/getannotations#getannotations_1)(int) | Mengekstrak anotasi dari halaman dokumen. Perhatikan bahwa hanya format PDF yang saat ini didukung. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Mengekstrak kode batang dari dokumen. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(BarcodeOptions) | Mengekstrak kode batang dari dokumen menggunakan opsi penyesuaian. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int) | Mengekstrak kode batang dari halaman dokumen. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_4)(int, BarcodeOptions) | Mengekstrak kode batang dari halaman dokumen menggunakan opsi penyesuaian. |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Mengekstrak objek kontainer dari dokumen untuk bekerja dengan format yang berisi lampiran, arsip ZIP, dll. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Mengembalikan informasi umum tentang dokumen. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Mengekstrak teks terformat dari dokumen. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Mengekstrak teks terformat dari halaman dokumen. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Mengekstrak sorotan dari dokumen. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Mengekstrak tautan hiper dari dokumen. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Mengekstrak tautan hiper dari halaman dokumen. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Mengekstrak tautan hiper dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan hiper). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Mengekstrak tautan hiper dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan hiper). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Mengekstrak gambar dari dokumen. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Mengekstrak gambar dari halaman dokumen. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | Mengekstrak gambar dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Mengekstrak gambar dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Mengekstrak metadata dari dokumen. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview)(int) | Menghasilkan pratinjau halaman dokumen. |
| [GetPagePreview](../../groupdocs.parser/parser/getpagepreview#getpagepreview_1)(int, PagePreviewOptions) | Menghasilkan pratinjau halaman dokumen menggunakan opsi penyesuaian. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Mengekstrak teks terstruktur dari dokumen. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)() | Mengekstrak tabel dari dokumen. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_2)(int) | Mengekstrak tabel dari halaman dokumen. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(PageTableAreaOptions) | Mengekstrak tabel dari dokumen. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_3)(int, PageTableAreaOptions) | Mengekstrak tabel dari halaman dokumen. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Mengekstrak teks dari dokumen. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Mengekstrak teks dari halaman dokumen. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Mengekstrak halaman teks dari dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks mentah cepat). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Mengekstrak teks dari halaman dokumen menggunakan opsi teks (untuk mengaktifkan mode ekstraksi teks mentah cepat). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Mengekstrak area teks dari dokumen. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Mengekstrak area teks dari halaman dokumen. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Mengekstrak area teks dari dokumen menggunakan opsi kustomisasi (ekspresi reguler, cocokkan huruf besar/kecil, dll.). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Mengekstrak area teks dari halaman dokumen menggunakan opsi kustomisasi (ekspresi reguler, cocokkan huruf besar/kecil, dll.). |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Mengekstrak daftar isi dari dokumen. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells)(int) | Mengekstrak sel lembar kerja. |
| [GetWorksheetCells](../../groupdocs.parser/parser/getworksheetcells#getworksheetcells_1)(int, WorksheetOptions) | Mengekstrak sel lembar kerja menggunakan opsi kustomisasi. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo_1)() | Mengekstrak informasi tentang semua lembar kerja dalam spreadsheet. |
| [GetWorksheetInfo](../../groupdocs.parser/parser/getworksheetinfo#getworksheetinfo)(int) | Mengekstrak informasi tentang lembar kerja. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate)(Template) | Menganalisis dokumen dengan templat yang dibuat pengguna. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_1)(Template, ParseByTemplateOptions) | Menganalisis dokumen dengan templat yang dibuat pengguna menggunakan opsi kustomisasi. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate#parsebytemplate_2)(TemplateCollection, ParseByTemplateOptions) | Memilih templat paling cocok dari koleksi yang disediakan dan kemudian menganalisis dokumen dengan templat yang dipilih. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Menganalisis formulir dokumen. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | Mencari *keyword* dalam dokumen. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | Mencari *keyword* dalam dokumen menggunakan opsi pencarian (ekspresi reguler, cocokkan huruf besar/kecil, dll). |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Mengembalikan informasi umum tentang file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Mengembalikan informasi umum tentang file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Mengembalikan informasi umum tentang file. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Mengembalikan informasi umum tentang file. |

### Lihat Juga

* namespace [GroupDocs.Parser](../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
