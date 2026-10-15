---
title: "GetTables"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak tabel dari dokumen."
type: docs
weight: 170
url: /id/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

Mengekstrak tabel dari dokumen.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| options | PageTableAreaOptions | Opsi untuk ekstraksi tabel. |

### Nilai Kembali

Koleksi objek [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` jika ekstraksi tabel tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak tabel dari seluruh dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi tabel
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Buat tata letak tabel
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Buat opsi untuk ekstraksi tabel
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Ekstrak tabel dari dokumen
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Iterasi atas tabel
    foreach (PageTableArea t in tables)
    {
        // Iterasi baris
        for (int row = 0; row < t.RowCount; row++)
        {
            // Iterasi kolom
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Dapatkan sel tabel
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Cetak teks sel tabel
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### Lihat Juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

Mengekstrak tabel dari halaman dokumen.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageTableAreaOptions | Opsi untuk ekstraksi tabel. |

### Nilai Kembali

Koleksi objek [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` jika ekstraksi tabel tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak tabel dari halaman dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi tabel
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Buat tata letak tabel
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Buat opsi untuk ekstraksi tabel
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Dapatkan informasi dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Iterasi melalui halaman
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Ekstrak tabel dari halaman dokumen
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Iterasi atas tabel
        foreach (PageTableArea t in tables)
        {
            // Iterasi baris
            for (int row = 0; row < t.RowCount; row++)
            {
                // Iterasi kolom
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Dapatkan sel tabel
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Cetak teks sel tabel
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### Lihat Juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

Mengekstrak tabel dari dokumen.

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### Nilai Kembali

Koleksi objek [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` jika ekstraksi tabel tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak tabel dari seluruh dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi tabel
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Ekstrak tabel dari dokumen
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // Iterasi atas tabel
    foreach (PageTableArea t in tables)
    {
        // Iterasi baris
        for (int row = 0; row < t.RowCount; row++)
        {
            // Iterasi kolom
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Dapatkan sel tabel
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Cetak teks sel tabel
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### Lihat Juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

Mengekstrak tabel dari halaman dokumen.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Kembali

Koleksi objek [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea); `null` jika ekstraksi tabel tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak tabel dari halaman dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Periksa apakah dokumen mendukung ekstraksi tabel
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // Dapatkan informasi dokumen
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Periksa apakah dokumen memiliki halaman
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // Iterasi melalui halaman
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Cetak nomor halaman 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Ekstrak tabel dari halaman dokumen
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // Iterasi atas tabel
        foreach (PageTableArea t in tables)
        {
            // Iterasi baris
            for (int row = 0; row < t.RowCount; row++)
            {
                // Iterasi kolom
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Dapatkan sel tabel
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Cetak teks sel tabel
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### Lihat Juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
