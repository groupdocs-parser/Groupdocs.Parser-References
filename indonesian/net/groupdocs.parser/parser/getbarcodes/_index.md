---
title: "GetBarcodes"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak kode batang dari dokumen."
type: docs
weight: 70
url: /id/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

Mengekstrak kode batang dari dokumen.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### Nilai Kembali

Koleksi objek [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` jika ekstraksi kode batang tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak kode batang dari dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak kode batang dari dokumen.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // Iterasi kode batang
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Cetak indeks halaman
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Cetak nilai kode batang
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Lihat Juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

Mengekstrak kode batang dari halaman dokumen.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Kembali

Koleksi objek [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` jika ekstraksi kode batang tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak kode batang dari halaman dokumen:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak kode batang dari halaman kedua dokumen.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // Iterasi kode batang
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // Cetak indeks halaman
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Cetak nilai kode batang
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Lihat Juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

Mengekstrak kode batang dari dokumen menggunakan opsi penyesuaian.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| options | BarcodeOptions | Opsi untuk ekstraksi kode batang. |

### Nilai Kembali

Koleksi objek [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` jika ekstraksi kode batang tidak didukung.

### Contoh

Contoh berikut menunjukkan cara mengekstrak kode batang dari sudut kanan atas.

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Buat opsi yang digunakan untuk ekstraksi kode batang
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // Ekstrak kode batang dari sudut kanan atas.
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // Iterasi kode batang
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // Cetak indeks halaman
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // Cetak nilai kode batang
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### Lihat Juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

Mengekstrak kode batang dari halaman dokumen menggunakan opsi penyesuaian.

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | BarcodeOptions | Opsi untuk ekstraksi kode batang. |

### Nilai Kembali

Koleksi objek [`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea); `null` jika ekstraksi kode batang tidak didukung.

### Lihat Juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
