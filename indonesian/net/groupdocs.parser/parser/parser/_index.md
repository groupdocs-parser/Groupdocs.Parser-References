---
title: Parser
second_title: GroupDocs.Parser untuk Referensi .NET API
description: Menginisialisasi instance baru dariParsergroupdocs.parser/parser kelas untuk mengekstrak data dari database.
type: docs
weight: 10
url: /id/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas untuk mengekstrak data dari database.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| connection | DbConnection | Koneksi basis data. |

### Perkataan

**Belajarlah lagi:**

* [Ekstrak data dari database](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Contoh

Contoh berikut menunjukkan cara mengekstrak data dari database Sqlite:

```csharp
// Buat objek DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Buat instance kelas Parser untuk mengekstrak tabel dari database
using (Parser parser = new Parser(connection))
{
    // Periksa apakah ekstraksi teks didukung
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Periksa apakah ekstraksi toc didukung
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Dapatkan daftar tabel
    IEnumerable<TocItem> toc = parser.GetToc();
    // Ulangi tabel
    foreach (TocItem i in toc)
    {
        // Cetak nama tabel
        Console.WriteLine(i.Text);
        // Ekstrak konten tabel sebagai teks
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat juga

* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas untuk mengekstrak data dari database.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| connection | DbConnection | Koneksi basis data. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Perkataan

**Belajarlah lagi:**

* [Ekstrak data dari database](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Penebangan](https://docs.groupdocs.com/display/parsernet/Logging)

### Contoh

Contoh berikut menunjukkan cara mengekstrak data dari database Sqlite:

```csharp
// Buat objek DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Buat instance kelas Parser untuk mengekstrak tabel dari database
using (Parser parser = new Parser(connection))
{
    // Periksa apakah ekstraksi teks didukung
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Periksa apakah ekstraksi toc didukung
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Dapatkan daftar tabel
    IEnumerable<TocItem> toc = parser.GetToc();
    // Ulangi tabel
    foreach (TocItem i in toc)
    {
        // Cetak nama tabel
        Console.WriteLine(i.Text);
        // Ekstrak konten tabel sebagai teks
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Lihat juga

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas untuk mengekstrak data dari server email jarak jauh.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| connection | EmailConnection | Koneksi email. |

### Perkataan

**Belajarlah lagi:**

* [Ekstrak email dari server jarak jauh melalui protokol POP, IMAP, atau Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Contoh

Contoh berikut menunjukkan cara mengekstrak email dari Exchange Server:

```csharp
// Buat objek koneksi untuk protokol Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Buat instance kelas Parser untuk mengekstrak email dari server jarak jauh
using (Parser parser = new Parser(connection))
{
    // Periksa apakah ekstraksi kontainer didukung
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Ekstrak pesan email dari server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Ulangi lampiran
    foreach (ContainerItem item in emails)
    {
        // Buat instance kelas Parser untuk pesan email
        using (Parser emailParser = item.OpenParser())
        {
            // Ekstrak teks email
            using (TextReader reader = emailParser.GetText())
            {
                // Cetak teks email
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Lihat juga

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas untuk mengekstrak data dari server email jarak jauh.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| connection | EmailConnection | Koneksi email. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Perkataan

**Belajarlah lagi:**

* [Ekstrak email dari server jarak jauh melalui protokol POP, IMAP, atau Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Penebangan](https://docs.groupdocs.com/display/parsernet/Logging)

### Contoh

Contoh berikut menunjukkan cara mengekstrak email dari Exchange Server:

```csharp
// Buat objek koneksi untuk protokol Exchange Web Services 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Buat instance kelas Parser untuk mengekstrak email dari server jarak jauh
using (Parser parser = new Parser(connection))
{
    // Periksa apakah ekstraksi kontainer didukung
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Ekstrak pesan email dari server
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Ulangi lampiran
    foreach (ContainerItem item in emails)
    {
        // Buat instance kelas Parser untuk pesan email
        using (Parser emailParser = item.OpenParser())
        {
            // Ekstrak teks email
            using (TextReader reader = emailParser.GetText())
            {
                // Cetak teks email
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Lihat juga

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas.

```csharp
public Parser(string filePath)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file. |

### Perkataan

**Belajarlah lagi:**

* [Muat dokumen dari disk lokal](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Contoh

Contoh berikut menunjukkan cara memuat dokumen dari disk lokal:

```csharp
// Buat instance kelas Parser dengan filePath
using (Parser parser = new Parser(filePath))
{
    // Ekstrak teks ke pembaca
    using (TextReader reader = parser.GetText())
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca adalah null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat juga

* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas dengan[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Pilihan untuk membuka file. |

### Perkataan

**Belajarlah lagi:**

* [Memuat format file tertentu](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Memuat dokumen yang dilindungi kata sandi](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Muat dokumen dari disk lokal](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Contoh

Kata sandi dokumen diteruskan oleh kelas LoadOptions:

```csharp
try
{
    // Buat instance kelas Parser dengan kata sandi:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Periksa apakah ekstraksi teks didukung
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Cetak teks dokumen
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Cetak pesan jika kata sandi salah atau kosong
    Console.WriteLine("Invalid password");
}
```

### Lihat juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas dengan[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Lihat juga

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas dengan[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) dan[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Pilihan untuk membuka file. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Perkataan

**Belajarlah lagi:**

* [Memuat format file tertentu](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Memuat dokumen yang dilindungi kata sandi](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Penebangan](https://docs.groupdocs.com/display/parsernet/Logging)
* [Muat dokumen dari disk lokal](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Contoh

Contoh berikut menunjukkan cara menerima informasi melalui[`ILogger`](../../../groupdocs.parser.options/ilogger) antarmuka:

```csharp
// mencoba
{
    // Buat instance kelas Logger
    Logger logger = new Logger();
    // Buat instance kelas Parser dengan pengaturan parser
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Periksa apakah ekstraksi teks didukung
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Cetak teks dokumen
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Abaikan pengecualian
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Cetak pesan kesalahan
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Cetak pesan acara
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Cetak pesan peringatan
        Console.WriteLine("Warning: " + message);
    }
}
```

### Lihat juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas.

```csharp
public Parser(Stream document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| document | Stream | Aliran masukan sumber. |

### Perkataan

**Belajarlah lagi:**

* [Muat dokumen dari aliran](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Contoh

Contoh berikut menunjukkan cara memuat dokumen dari aliran:

```csharp
// Buat instance kelas Parser dengan aliran
using (Parser parser = new Parser(stream))
{
    // Ekstrak teks ke pembaca
    using (TextReader reader = parser.GetText())
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca adalah null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat juga

* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas dengan[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| document | Stream | Aliran masukan sumber. |
| loadOptions | LoadOptions | Pilihan untuk membuka file. |

### Perkataan

**Belajarlah lagi:**

* [Memuat format file tertentu](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Memuat dokumen yang dilindungi kata sandi](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Muat dokumen dari aliran](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Contoh

Dalam beberapa kasus, perlu ditentukan[`FileFormat`](../../../groupdocs.parser.options/fileformat). Baik untuk kasus khusus (database, server email) dan untuk mendeteksi jenis file berdasarkan konten:

Kata sandi dokumen dilewatkan[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) kelas:

```csharp
// Buat instance kelas Parser untuk dokumen penurunan harga
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Periksa apakah ekstraksi teks didukung
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Cetak teks dokumen
        // Penurunan harga terdeteksi; teks tanpa simbol khusus dicetak
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Buat instance kelas Parser dengan kata sandi:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Periksa apakah ekstraksi teks didukung
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Cetak teks dokumen
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Cetak pesan jika kata sandi salah atau kosong
    Console.WriteLine("Invalid password");
}
```

### Lihat juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas dengan[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| document | Stream | Aliran masukan sumber. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Lihat juga

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Menginisialisasi instance baru dari[`Parser`](../../parser) kelas dengan[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) dan[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| document | Stream | Aliran masukan sumber. |
| loadOptions | LoadOptions | Pilihan untuk membuka file. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Perkataan

**Belajarlah lagi:**

* [Memuat format file tertentu](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Memuat dokumen yang dilindungi kata sandi](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Muat dokumen dari aliran](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Penebangan](https://docs.groupdocs.com/display/parsernet/Logging)

### Contoh

Contoh berikut menunjukkan cara menerima informasi melalui[`ILogger`](../../../groupdocs.parser.options/ilogger) antarmuka:

```csharp
// mencoba
{
    // Buat instance kelas Logger
    Logger logger = new Logger();
    // Buat instance kelas Parser dengan pengaturan parser
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Periksa apakah ekstraksi teks didukung
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Cetak teks dokumen
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Abaikan pengecualian
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Cetak pesan kesalahan
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Cetak pesan acara
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Cetak pesan peringatan
        Console.WriteLine("Warning: " + message);
    }
}
```

### Lihat juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ruang nama [GroupDocs.Parser](../../parser)
* perakitan [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
