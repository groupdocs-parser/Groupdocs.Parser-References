---
title: GetBarcodes
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Ekstrak barcode dari dokumen.
type: docs
weight: 50
url: /id/net/groupdocs.parser/parser/getbarcodes/
---
## GetBarcodes() {#getbarcodes}

Ekstrak barcode dari dokumen.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Nilai Pengembalian

Kumpulan dari[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objek; `batal` jika ekstraksi barcode tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak barcode dari dokumen:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak kode batang dari dokumen.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Ulangi kode batang
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Cetak indeks halaman
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Cetak nilai barcode
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Lihat juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_2}

Mengekstrak barcode dari halaman dokumen.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Pengembalian

Kumpulan dari[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objek; `batal` jika ekstraksi barcode tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak barcode dari halaman dokumen:

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak kode batang dari halaman dokumen kedua.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Ulangi kode batang
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Cetak indeks halaman
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Cetak nilai barcode
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Lihat juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetBarcodes(PageAreaOptions) {#getbarcodes_1}

Ekstrak kode batang dari dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi kode batang).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(PageAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| options | PageAreaOptions | Opsi untuk ekstraksi kode batang. |

### Nilai Pengembalian

Kumpulan dari[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objek; `batal` jika ekstraksi barcode tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak barcode dari pojok kanan atas.

```csharp
// Buat instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Buat opsi yang digunakan untuk ekstraksi kode batang
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Ekstrak kode batang dari sudut kanan atas.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Ulangi kode batang
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Cetak indeks halaman
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Cetak nilai barcode
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Lihat juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, PageAreaOptions) {#getbarcodes_3}

Mengekstrak kode batang dari halaman dokumen menggunakan opsi penyesuaian (untuk menyetel area persegi panjang yang berisi kode batang).

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, PageAreaOptions options)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PageAreaOptions | Opsi untuk ekstraksi kode batang. |

### Nilai Pengembalian

Kumpulan dari[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) objek; `batal` jika ekstraksi barcode tidak didukung.

### Lihat juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
