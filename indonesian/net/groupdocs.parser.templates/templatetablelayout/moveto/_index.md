---
title: "MoveTo"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Membuat tata letak baru dengan pemisah ukuran yang sama dan posisi pada titik."
type: docs
weight: 50
url: /id/net/groupdocs.parser.templates/templatetablelayout/moveto/
---

## TemplateTableLayout.MoveTo method

Membuat tata letak baru dengan ukuran, pemisah, dan posisi yang sama dalam *point*.

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| point | Point | Posisi tata letak baru. |

### Nilai Kembali

Tata letak baru dengan ukuran, pemisah, dan posisi yang sama pada *point*.

### Contoh

Fungsionalitas ini memungkinkan untuk memindahkan Tata Letak Tabel.

Misalnya, sebuah dokumen memiliki tabel di setiap halaman (atau sekumpulan dokumen dengan tabel pada halaman). Tabel-tabel ini berbeda dalam posisi dan konten, tetapi memiliki kolom dan baris yang sama. Dalam kasus ini, pengguna dapat mendefinisikan objek [`TemplateTableLayout`](../../templatetablelayout) pada `(0, 0)` sekali dan kemudian memindahkannya ke lokasi tabel yang pasti.

Jika posisi tabel bergantung pada objek lain di halaman, pengguna dapat mendefinisikan objek [`TemplateTableLayout`](../../templatetablelayout) berdasarkan dokumen templat dan kemudian memindahkannya sesuai dengan objek jangkar. Misalnya, jika ini adalah tabel ringkasan dan diikuti oleh tabel detail (yang dapat berisi jumlah baris yang berbeda). Dalam kasus ini, pengguna dapat mendefinisikan objek [`TemplateTableLayout`](../../templatetablelayout) pada dokumen templat (dengan persegi panjang tabel detail yang diketahui) dan kemudian memindahkan objek [`TemplateTableLayout`](../../templatetablelayout) sesuai dengan perbedaan persegi panjang tabel detail antara templat dan dokumen nyata.

Metode `MoveTo` mengembalikan salinan objek saat ini. Pengguna dapat memberikan koordinat apa pun (bahkan negatif - maka tata letak akan dipindahkan ke kiri/atas).

```csharp
// Buat tata letak tabel
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// Cetak persegi panjang
Rectangle rect = layout.Rectangle;

// Mencetak: pos: (0, 0) ukuran: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// Pindahkan tata letak ke lokasi tabel yang pasti
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// Pastikan pemisah pertama dipindahkan:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // prints: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // prints: 250

Rectangle movedRect = movedLayout.Rectangle;

// Mencetak: pos: (315, 250) ukuran: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// Objek movedLayout adalah salinan dari objek layout, sehingga kita dapat menyesuaikan pemisah tanpa memengaruhi tata letak asli:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // prints: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // prints: 6
```

### Lihat Juga

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
