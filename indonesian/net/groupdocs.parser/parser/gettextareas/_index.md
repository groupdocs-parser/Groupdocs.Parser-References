---
title: "GetTextAreas"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak area teks dari dokumen."
type: docs
weight: 190
url: /id/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

Mengekstrak area teks dari dokumen.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Nilai Kembali

Koleksi dari [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `null` jika ekstraksi area teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Contoh

Contoh berikut menunjukkan cara mengekstrak semua area teks dari seluruh dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
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
 
    // Iterasi area teks halaman
    foreach(PageTextArea a in areas)
    {
        // Cetak indeks halaman, persegi panjang, dan nilai area teks:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Mengekstrak area teks dari dokumen menggunakan opsi kustomisasi (ekspresi reguler, cocokkan huruf besar/kecil, dll.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| options | PageTextAreaOptions | Opsi untuk ekstraksi area teks. |

### Nilai Kembali

Koleksi dari [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `null` jika ekstraksi area teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Contoh

Contoh berikut menunjukkan cara mengekstrak hanya area teks dengan digit dari pojok kiri atas:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Buat opsi yang digunakan untuk ekstraksi area teks
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Ekstrak area teks yang hanya berisi digit dari pojok kiri atas halaman:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Periksa apakah ekstraksi area teks didukung
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Iterasi area teks halaman
    foreach(PageTextArea a in areas)
    {
        // Cetak indeks halaman, persegi panjang, dan nilai area teks:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Mengekstrak area teks dari halaman dokumen.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Kembali

Koleksi dari [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `null` jika ekstraksi area teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Contoh

Untuk mengekstrak area teks dari halaman dokumen, metode berikut digunakan:

```csharp
// Buat sebuah instance dari kelas Parser
using(Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi area teks
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // Dapatkan informasi dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Iterasi melalui halaman
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Iterasi area teks halaman
        // Kami mengabaikan pengecekan null karena kami telah memeriksa dukungan fitur ekstraksi area teks sebelumnya
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Cetak persegi panjang dan nilai area teks:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Mengekstrak area teks dari halaman dokumen menggunakan opsi kustomisasi (ekspresi reguler, cocokkan huruf besar/kecil, dll.).

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageTextAreaOptions | Opsi untuk ekstraksi area teks. |

### Nilai Kembali

Koleksi dari [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) objek; `null` jika ekstraksi area teks tidak didukung.

### Catatan

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
