---
title: "GetHyperlinks"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak tautan hiper dari dokumen."
type: docs
weight: 120
url: /id/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

Mengekstrak tautan hiper dari dokumen.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### Nilai Kembali

Koleksi objek [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua hyperlink dari seluruh dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
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
    // Iterasi hyperlink
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

### Lihat Juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

Mengekstrak tautan hiper dari halaman dokumen.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Kembali

Koleksi objek [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak hyperlink dari halaman dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi hyperlink
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // Dapatkan informasi dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Iterasi melalui halaman
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Ekstrak hyperlink dari halaman dokumen
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // Iterasi hyperlink
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

### Lihat Juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

Mengekstrak tautan hiper dari dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan hiper).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| options | PageAreaOptions | Opsi untuk ekstraksi hyperlink. |

### Nilai Kembali

Koleksi objek [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak hyperlink dari area halaman dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
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
    // Iterasi hyperlink
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

### Lihat Juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

Mengekstrak tautan hiper dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi tautan hiper).

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageAreaOptions | Opsi untuk ekstraksi hyperlink. |

### Nilai Kembali

Koleksi objek [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea); `null` jika ekstraksi hyperlink tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak hyperlink dari area halaman dokumen menggunakan opsi penyesuaian:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi hyperlink
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // Dapatkan informasi dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // Buat opsi yang digunakan untuk ekstraksi hyperlink
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // Iterasi melalui halaman
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // Ekstrak hyperlink dari area halaman dokumen
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // Iterasi hyperlink
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

### Lihat Juga

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
