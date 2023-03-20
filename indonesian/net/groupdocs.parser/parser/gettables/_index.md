---
title: GetTables
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Mengekstrak tabel dari dokumen.
type: docs
weight: 140
url: /id/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Mengekstrak tabel dari dokumen.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| options | PageTableAreaOptions | Opsi untuk ekstraksi tabel. |

### Nilai Pengembalian

Kumpulan dari[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objek; `batal` jika ekstraksi tabel tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak tabel dari seluruh dokumen:

```csharp
// Buat instance dari kelas Parser
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
    // Ulangi tabel
    foreach (PageTableArea t in tables)
    {
        // Ulangi baris
        for (int row = 0; row < t.RowCount; row++)
        {
            // Ulangi kolom
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

### Lihat juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Mengekstrak tabel dari halaman dokumen.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageTableAreaOptions | Opsi untuk ekstraksi tabel. |

### Nilai Pengembalian

Kumpulan dari[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) objek; `batal` jika ekstraksi tabel tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak tabel dari halaman dokumen:

```csharp
// Buat instance dari kelas Parser
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
        // Ekstrak tabel dari halaman dokumen
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Ulangi tabel
        foreach (PageTableArea t in tables)
        {
            // Ulangi baris
            for (int row = 0; row < t.RowCount; row++)
            {
                // Ulangi kolom
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

### Lihat juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
