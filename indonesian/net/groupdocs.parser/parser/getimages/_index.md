---
title: GetImages
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mengekstrak gambar dari dokumen.
type: docs
weight: 110
url: /id/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

Mengekstrak gambar dari dokumen.

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### Nilai Pengembalian

Kumpulan dari[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objek; `batal` jika ekstraksi gambar tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak gambar dari dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Ekstrak gambar ke file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Ekstrak gambar dari dokumen Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Ekstrak gambar dari spreadsheet Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Ekstrak gambar dari presentasi Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Ekstrak gambar dari Email](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Ekstrak gambar dari dokumen PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua gambar dari seluruh dokumen:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak gambar
    IEnumerable<PageImageArea> images = parser.GetImages();
    // Periksa apakah ekstraksi gambar didukung
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // Ulangi gambar
    foreach (PageImageArea image in images)
    {
        // Cetak indeks halaman, persegi panjang, dan tipe gambar:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Lihat juga

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

Mengekstrak gambar dari dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi gambar).

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| options | PageAreaOptions | Pilihan untuk ekstraksi gambar. |

### Nilai Pengembalian

Kumpulan dari[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objek; `batal` jika ekstraksi gambar tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak gambar dari dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Ekstrak gambar ke file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Ekstrak gambar dari area halaman dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Ekstrak gambar dari dokumen Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Ekstrak gambar dari spreadsheet Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Ekstrak gambar dari presentasi Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Ekstrak gambar dari Email](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Ekstrak gambar dari dokumen PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Contoh

Contoh berikut menunjukkan cara mengekstrak hanya gambar dari pojok kiri atas:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Buat opsi yang digunakan untuk ekstraksi gambar
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // Ekstrak gambar dari sudut kiri atas halaman:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // Periksa apakah ekstraksi gambar didukung
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // Ulangi gambar
    foreach (PageImageArea image in images)
    {
        // Cetak indeks halaman, persegi panjang, dan tipe gambar:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### Lihat juga

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

Mengekstrak gambar dari halaman dokumen.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Pengembalian

Kumpulan dari[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objek; `batal` jika ekstraksi gambar tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak gambar dari dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Ekstrak gambar ke file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Ekstrak gambar dari halaman dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Ekstrak gambar dari dokumen Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Ekstrak gambar dari spreadsheet Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Ekstrak gambar dari presentasi Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Ekstrak gambar dari Email](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Ekstrak gambar dari dokumen PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Contoh

Untuk mengekstrak gambar dari halaman dokumen, metode berikut digunakan:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi gambar
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Ulangi gambar
        // Kami mengabaikan pemeriksaan nol karena kami telah memeriksa dukungan fitur ekstraksi gambar sebelumnya
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // Cetak persegi panjang dan tipe gambar
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### Lihat juga

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

Mengekstrak gambar dari halaman dokumen menggunakan opsi penyesuaian (untuk mengatur area persegi panjang yang berisi gambar).

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageAreaOptions | Pilihan untuk ekstraksi gambar. |

### Nilai Pengembalian

Kumpulan dari[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) objek; `batal` jika ekstraksi gambar tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak gambar dari dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Ekstrak gambar ke file](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Ekstrak gambar dari halaman dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Ekstrak gambar dari area halaman dokumen](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Ekstrak gambar dari dokumen Microsoft Office Word](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Ekstrak gambar dari spreadsheet Microsoft Office Excel](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Ekstrak gambar dari presentasi Microsoft Office PowerPoint](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Ekstrak gambar dari Email](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Ekstrak gambar dari dokumen PDF](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Lihat juga

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
