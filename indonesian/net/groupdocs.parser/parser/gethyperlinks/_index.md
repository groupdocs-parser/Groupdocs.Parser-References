---
title: GetHyperlinks
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mengekstrak hyperlink dari dokumen.
type: docs
weight: 100
url: /id/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

Mengekstrak hyperlink dari dokumen.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Nilai Pengembalian

Kumpulan dari[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objek; `batal` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua hyperlink dari seluruh dokumen:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi hyperlink
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Ekstrak hyperlink dari dokumen
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // Iterasi melalui hyperlink
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Cetak teks hyperlink
        Console.WriteLine(h.Text);
        // Cetak URL hyperlink
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Lihat juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Mengekstrak hyperlink dari halaman dokumen.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Pengembalian

Kumpulan dari[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objek; `batal` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak hyperlink dari halaman dokumen:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi hyperlink
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Dapatkan info dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Ulangi beberapa halaman
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Ekstrak hyperlink dari halaman dokumen
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Iterasi melalui hyperlink
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Cetak teks hyperlink
            Console.WriteLine(h.Text);
            // Cetak URL hyperlink
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### Lihat juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Mengekstrak hyperlink dari dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi hyperlink).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| options | PageAreaOptions | Opsi untuk ekstraksi hyperlink. |

### Nilai Pengembalian

Kumpulan dari[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objek; `batal` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak hyperlink dari area halaman dokumen:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi hyperlink
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Buat opsi yang digunakan untuk ekstraksi hyperlink
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Ekstrak hyperlink dari area halaman dokumen
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // Iterasi melalui hyperlink
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // Cetak teks hyperlink
        Console.WriteLine(h.Text);
        // Cetak URL hyperlink
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### Lihat juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Mengekstrak hyperlink dari halaman dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi hyperlink).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageAreaOptions | Opsi untuk ekstraksi hyperlink. |

### Nilai Pengembalian

Kumpulan dari[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) objek; `batal` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak hyperlink dari area halaman dokumen menggunakan opsi penyesuaian:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi hyperlink
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Dapatkan info dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Buat opsi yang digunakan untuk ekstraksi hyperlink
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Ulangi beberapa halaman
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Ekstrak hyperlink dari area halaman dokumen
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Iterasi melalui hyperlink
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // Cetak teks hyperlink
            Console.WriteLine(h.Text);
            // Cetak URL hyperlink
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### Lihat juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
