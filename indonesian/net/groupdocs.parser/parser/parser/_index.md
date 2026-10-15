---
title: "Pengurai"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi instance baru dari kelas Parsergroupdocs.parser/parser untuk mengekstrak data dari sebuah URI."
type: docs
weight: 10
url: /id/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari sebuah URI.

```csharp
public Parser(Uri uri)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| uri | Uri | Uri tempat permintaan dikirim. |

### Lihat Juga

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari sebuah URI dengan *loadOptions*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| uri | Uri | Uri tempat permintaan dikirim. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |

### Lihat Juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari sebuah URI dengan *parserSettings*.

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| uri | Uri | Uri tempat permintaan dikirim. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Lihat Juga

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari sebuah URI dengan *loadOptions* dan *parserSettings*.

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| uri | Uri | Uri tempat permintaan dikirim. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Lihat Juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari sebuah basis data.

```csharp
public Parser(DbConnection connection)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| koneksi | DbConnection | Koneksi basis data. |

### Catatan

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Contoh

Contoh berikut menunjukkan cara mengekstrak data dari basis data Sqlite:

```csharp
// Buat objek DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Buat instance dari kelas Parser untuk mengekstrak tabel dari basis data
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
    // Iterasi atas tabel
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

### Lihat Juga

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari sebuah basis data.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| koneksi | DbConnection | Koneksi basis data. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Catatan

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Contoh

Contoh berikut menunjukkan cara mengekstrak data dari basis data Sqlite:

```csharp
// Buat objek DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Buat instance dari kelas Parser untuk mengekstrak tabel dari basis data
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
    // Iterasi atas tabel
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

### Lihat Juga

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari server email remote.

```csharp
public Parser(EmailConnection connection)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| koneksi | EmailConnection | Koneksi email. |

### Catatan

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Contoh

Contoh berikut menunjukkan cara mengekstrak email dari Exchange Server:

```csharp
// Buat objek koneksi untuk protokol Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Buat instance dari kelas Parser untuk mengekstrak email dari server remote
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
 
    // Iterasi atas lampiran
    foreach (ContainerItem item in emails)
    {
        // Buat sebuah instance kelas Parser untuk pesan email
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

### Lihat Juga

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Menginisialisasi instance baru dari kelas [`Parser`](../../parser) untuk mengekstrak data dari server email remote.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| koneksi | EmailConnection | Koneksi email. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Catatan

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Contoh

Contoh berikut menunjukkan cara mengekstrak email dari Exchange Server:

```csharp
// Buat objek koneksi untuk protokol Exchange Web Services
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Buat instance dari kelas Parser untuk mengekstrak email dari server remote
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
 
    // Iterasi atas lampiran
    foreach (ContainerItem item in emails)
    {
        // Buat sebuah instance kelas Parser untuk pesan email
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

### Lihat Juga

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser).

```csharp
public Parser(string filePath)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |

### Catatan

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Contoh

Contoh berikut menunjukkan cara memuat dokumen dari disk lokal:

```csharp
// Buat sebuah instance kelas Parser dengan filePath
using (Parser parser = new Parser(filePath))
{
    // Ekstrak teks ke dalam pembaca
    using (TextReader reader = parser.GetText())
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca akan bernilai null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat Juga

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser) dengan [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |

### Catatan

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Contoh

Kata sandi dokumen diberikan oleh kelas LoadOptions:

```csharp
try
{
    // Buat sebuah instance kelas Parser dengan kata sandi:
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
    // Cetak pesan jika kata sandi tidak benar atau kosong
    Console.WriteLine("Invalid password");
}
```

### Lihat Juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser) dengan [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Lihat Juga

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser) dengan [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) dan [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Catatan

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Contoh

Contoh berikut menunjukkan cara menerima informasi melalui antarmuka [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Buat sebuah instance kelas Logger
    Logger logger = new Logger();
    // Buat sebuah instance kelas Parser dengan pengaturan parser
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
    ; // Ignore the exception
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

### Lihat Juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser).

```csharp
public Parser(Stream document)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |

### Catatan

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Contoh

Contoh berikut menunjukkan cara memuat dokumen dari aliran:

```csharp
// Buat sebuah instance kelas Parser dengan aliran
using (Parser parser = new Parser(stream))
{
    // Ekstrak teks ke dalam pembaca
    using (TextReader reader = parser.GetText())
    {
        // Cetak teks dari dokumen
        // Jika ekstraksi teks tidak didukung, pembaca akan bernilai null
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Lihat Juga

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser) dengan [`LoadOptions`](../../../groupdocs.parser.options/loadoptions).

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |

### Catatan

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Contoh

Dalam beberapa kasus diperlukan untuk mendefinisikan [`FileFormat`](../../../groupdocs.parser.options/fileformat). Baik untuk kasus khusus (basis data, server email) maupun untuk mendeteksi tipe file berdasarkan kontennya:

```csharp
// Buat sebuah instance dari kelas Parser untuk dokumen markdown
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
        // Markdown terdeteksi; teks tanpa simbol khusus dicetak
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

Kata sandi dokumen diteruskan oleh kelas [`LoadOptions`](../../../groupdocs.parser.options/loadoptions):

```csharp
try
{
    // Buat sebuah instance kelas Parser dengan kata sandi:
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
    // Cetak pesan jika kata sandi tidak benar atau kosong
    Console.WriteLine("Invalid password");
}
```

### Lihat Juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser) dengan [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Lihat Juga

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Menginisialisasi sebuah instance baru dari kelas [`Parser`](../../parser) dengan [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) dan [`ParserSettings`](../../../groupdocs.parser.options/parsersettings).

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| dokumen | Stream | Aliran input sumber. |
| loadOptions | LoadOptions | Opsi untuk membuka file. |
| parserSettings | ParserSettings | Pengaturan parser yang digunakan untuk menyesuaikan ekstraksi data. |

### Catatan

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Contoh

Contoh berikut menunjukkan cara menerima informasi melalui antarmuka [`ILogger`](../../../groupdocs.parser.options/ilogger):

```csharp
// try
{
    // Buat sebuah instance kelas Logger
    Logger logger = new Logger();
    // Buat sebuah instance kelas Parser dengan pengaturan parser
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
    ; // Ignore the exception
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

### Lihat Juga

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
