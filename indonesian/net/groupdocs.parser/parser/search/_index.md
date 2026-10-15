---
title: "Search"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mencari kata kunci dalam dokumen."
type: docs
weight: 250
url: /id/net/groupdocs.parser/parser/search/
---

## Search(string) {#search}

Mencari *keyword* dalam dokumen.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| kata kunci | String | Kata kunci yang akan dicari. |

### Nilai Kembali

Koleksi objek [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null` jika pencarian tidak didukung.

### Catatan

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Contoh

Contoh berikut menunjukkan cara menemukan kata kunci dalam dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Cari kata kunci:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Periksa apakah pencarian didukung
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterasi hasil pencarian
    foreach(SearchResult s in sr)
    {
        // Cetak indeks dan teks yang ditemukan:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Lihat Juga

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Mencari *keyword* dalam dokumen menggunakan opsi pencarian (ekspresi reguler, cocokkan huruf besar/kecil, dll).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| kata kunci | String | Kata kunci yang akan dicari. |
| options | SearchOptions | Opsi pencarian. |

### Nilai Kembali

Koleksi objek [`SearchResult`](../../../groupdocs.parser.data/searchresult); `null` jika pencarian tidak didukung.

### Catatan

**Learn more:**

* [Search text](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Search text in Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Search text in Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Search text in Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Search text in PDF documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Search text in Emails](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Search text in EPUB eBooks](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Search text in HTML documents](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Search text in Microsoft OneNote sections](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Contoh

Contoh berikut menunjukkan cara mencari dengan ekspresi reguler dalam dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Cari dengan ekspresi reguler dengan pencocokan huruf besar/kecil
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Periksa apakah pencarian didukung
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterasi hasil pencarian
    foreach(SearchResult s in sr)
    {
        // Cetak indeks dan teks yang ditemukan:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

Contoh berikut menunjukkan cara mencari teks pada halaman:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Cari kata kunci dengan nomor halaman
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Periksa apakah pencarian didukung
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Iterasi hasil pencarian
    foreach(SearchResult s in sr)
    {
        // Cetak indeks, nomor halaman, dan teks yang ditemukan:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Lihat Juga

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
