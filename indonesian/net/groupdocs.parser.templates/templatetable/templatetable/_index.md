---
title: "TemplateTable"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi sebuah instance baru dari kelas TemplateTablegroupdocs.parser.templates/templatetable dengan nama HURUF KAPITAL."
type: docs
weight: 10
url: /id/net/groupdocs.parser.templates/templatetable/templatetable/
---

## TemplateTable(TemplateTableLayout, string) {#constructor}

Menginisialisasi sebuah instance baru dari kelas [`TemplateTable`](../../templatetable) dengan nama HURUF KAPITAL.

```csharp
public TemplateTable(TemplateTableLayout layout, string name)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| layout | TemplateTableLayout | Tata letak tabel. |
| nama | String | Nama tabel. |

### Contoh

Tabel templat diatur oleh tata letak tabel jika tabel tidak dapat terdeteksi secara otomatis:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Buat templat dokumen
Template template = new Template(new TemplateItem[] { table });
```

### Lihat Juga

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`TemplateTable`](../../templatetable) dengan nama HURUF KAPITAL.

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| layout | TemplateTableLayout | Tata letak tabel. |
| nama | String | Nama tabel. |
| pageWidth | Nullable`1 | Lebar halaman yang digunakan untuk membuat item templat. |

### Contoh

Tabel templat diatur oleh tata letak tabel jika tabel tidak dapat terdeteksi secara otomatis:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null);

// Buat templat dokumen
Template template = new Template(new TemplateItem[] { table });
```

### Lihat Juga

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableLayout, string, double?, bool) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableLayout layout, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| layout | TemplateTableLayout | Tata letak tabel. |
| nama | String | Nama tabel. |
| pageWidth | Nullable`1 | Lebar halaman yang digunakan untuk membuat item templat. |
| useUpperCaseName | Boolean | Nilai yang menunjukkan apakah `name` diubah menjadi HURUF BESAR. |

### Contoh

Tabel templat diatur oleh tata letak tabel jika tabel tidak dapat terdeteksi secara otomatis:

```csharp
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 50, 95, 275 },
    new double[] { 325, 340, 365 });
 
TemplateTable table = new TemplateTable(layout, "Details", null, false);

// Buat templat dokumen
Template template = new Template(new TemplateItem[] { table });
```

### Lihat Juga

* class [TemplateTableLayout](../../templatetablelayout)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string) {#constructor_3}

Menginisialisasi sebuah instance baru dari kelas [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| parameters | TemplateTableParameters | Parameter untuk mendeteksi tabel dalam mode otomatis. |
| nama | String | Nama tabel. |

### Contoh

Jika tabel templat diatur oleh parameter detektor, tabel akan terdeteksi secara otomatis:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0);

// Buat templat dokumen
Template template = new Template(new TemplateItem[] { table });
```

### Lihat Juga

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?) {#constructor_4}

Menginisialisasi sebuah instance baru dari kelas [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| parameters | TemplateTableParameters | Parameter untuk mendeteksi tabel dalam mode otomatis. |
| nama | String | Nama tabel. |
| pageWidth | Nullable`1 | Lebar halaman yang digunakan untuk membuat item templat. |

### Contoh

Jika tabel templat diatur oleh parameter detektor, tabel akan terdeteksi secara otomatis:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Buat templat dokumen
Template template = new Template(new TemplateItem[] { table });
```

### Lihat Juga

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## TemplateTable(TemplateTableParameters, string, double?, bool) {#constructor_5}

Menginisialisasi sebuah instance baru dari kelas [`TemplateTable`](../../templatetable).

```csharp
public TemplateTable(TemplateTableParameters parameters, string name, double? pageWidth, 
    bool useUpperCaseName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| parameters | TemplateTableParameters | Parameter untuk mendeteksi tabel dalam mode otomatis. |
| nama | String | Nama tabel. |
| pageWidth | Nullable`1 | Lebar halaman yang digunakan untuk membuat item templat. |
| useUpperCaseName | Boolean | Nilai yang menunjukkan apakah `name` diubah menjadi HURUF BESAR. |

### Contoh

Jika tabel templat diatur oleh parameter detektor, tabel akan terdeteksi secara otomatis:

```csharp
TemplateTableParameters parameters = new TemplateTableParameters(
    new Rectangle(new Point(175, 350), new Size(400, 200)),
    new double[] { 185, 370, 425, 485, 545 });

TemplateTable table = new TemplateTable(parameters, "Details", 0, false);

// Buat templat dokumen
Template template = new Template(new TemplateItem[] { table });
```

### Lihat Juga

* class [TemplateTableParameters](../../templatetableparameters)
* class [TemplateTable](../../templatetable)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
