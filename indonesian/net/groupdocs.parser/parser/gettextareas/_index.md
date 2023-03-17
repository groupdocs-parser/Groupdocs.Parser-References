---
title: GetTextAreas
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mengekstrak area teks dari dokumen.
type: docs
weight: 160
url: /id/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Mengekstrak area teks dari dokumen.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Nilai Pengembalian

Kumpulan dari[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `batal` jika ekstraksi area teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak area teks](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua area teks dari seluruh dokumen:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Ekstrak area teks
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Periksa apakah ekstraksi area teks didukung
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Ulangi area teks halaman
    foreach(PageTextArea a in areas)
    {
        // Cetak indeks halaman, persegi panjang dan nilai area teks:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Lihat juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Mengekstrak area teks dari dokumen menggunakan opsi penyesuaian (ekspresi reguler, huruf besar-kecil, dll.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| options | PageTextAreaOptions | Opsi untuk ekstraksi area teks. |

### Nilai Pengembalian

Kumpulan dari[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `batal` jika ekstraksi area teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak area teks](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Contoh

Contoh berikut menunjukkan cara mengekstrak hanya area teks dengan angka dari pojok kiri atas:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Buat opsi yang digunakan untuk ekstraksi area teks
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Ekstrak area teks yang hanya berisi angka dari pojok kiri atas halaman:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Periksa apakah ekstraksi area teks didukung
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Ulangi area teks halaman
    foreach(PageTextArea a in areas)
    {
        // Cetak indeks halaman, persegi panjang dan nilai area teks:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Lihat juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Mengekstrak area teks dari halaman dokumen.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Pengembalian

Kumpulan dari[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `batal` jika ekstraksi area teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak area teks](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Contoh

Untuk mengekstrak area teks dari halaman dokumen, metode berikut digunakan:

```csharp
// Buat instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi area teks
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Dapatkan info dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Ulangi beberapa halaman
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Ulangi area teks halaman
        // Kami mengabaikan pemeriksaan nol karena kami telah memeriksa dukungan fitur ekstraksi area teks sebelumnya
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Cetak nilai persegi panjang dan area teks:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Lihat juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Mengekstrak area teks dari halaman dokumen menggunakan opsi penyesuaian (ekspresi reguler, huruf besar-kecil, dll.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageTextAreaOptions | Opsi untuk ekstraksi area teks. |

### Nilai Pengembalian

Kumpulan dari[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `batal` jika ekstraksi area teks tidak didukung.

### Perkataan

**Belajarlah lagi:**

* [Ekstrak area teks](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Lihat juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
