---
title: Search
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Pencarian akeyword dalam dokumen.
type: docs
weight: 200
url: /id/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

Pencarian a*keyword* dalam dokumen.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| keyword | String | Kata kunci untuk mencari. |

### Nilai Pengembalian

Kumpulan dari[`SearchResult`](../../../groupdocs.parser.data/searchresult) benda; `batal` jika pencarian tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Cari teks](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Cari teks dalam dokumen Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Cari teks di spreadsheet Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Cari teks dalam presentasi Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Cari teks dalam dokumen PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Cari teks di Email](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Cari teks di eBook EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Cari teks dalam dokumen HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Cari teks di bagian Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Contoh

Contoh berikut menunjukkan cara menemukan kata kunci dalam dokumen:

```csharp
// Buat instance dari kelas Parser
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
 
    // Ulangi hasil pencarian
    foreach(SearchResult s in sr)
    {
        // Cetak indeks dan temukan teks:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Lihat juga

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

Pencarian a*keyword*dalam dokumen menggunakan opsi pencarian (ekspresi reguler, kasus pencocokan, dll.).

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| keyword | String | Kata kunci untuk mencari. |
| options | SearchOptions | Opsi pencarian. |

### Nilai Pengembalian

Kumpulan dari[`SearchResult`](../../../groupdocs.parser.data/searchresult) objek; `batal` jika pencarian tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Cari teks](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Cari teks dalam dokumen Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Cari teks di spreadsheet Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Cari teks dalam presentasi Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [Cari teks dalam dokumen PDF](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [Cari teks di Email](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [Cari teks di eBook EPUB](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [Cari teks dalam dokumen HTML](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Cari teks di bagian Microsoft OneNote](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Contoh

Contoh berikut menunjukkan cara mencari dengan ekspresi reguler dalam dokumen:

Contoh berikut menunjukkan cara mencari teks di halaman:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Cari dengan ekspresi reguler dengan pencocokan huruf besar-kecil
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Periksa apakah pencarian didukung
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Ulangi hasil pencarian
    foreach(SearchResult s in sr)
    {
        // Cetak indeks dan temukan teks:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Buat instance dari kelas Parser
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
 
    // Ulangi hasil pencarian
    foreach(SearchResult s in sr)
    {
        // Cetak indeks, nomor halaman, dan teks yang ditemukan:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Lihat juga

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
