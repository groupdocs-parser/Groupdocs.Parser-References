---
title: Parser
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Yeni bir örneğini başlatır.Parsergroupdocs.parser/parser bir veritabanından veri ayıklamak için sınıf.
type: docs
weight: 10
url: /tr/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Yeni bir örneğini başlatır.[`Parser`](../../parser) bir veritabanından veri ayıklamak için sınıf.

```csharp
public Parser(DbConnection connection)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| connection | DbConnection | Veritabanı bağlantısı. |

### Notlar

**Daha fazla bilgi edin:**

* [Veritabanlarından veri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Örnekler

Aşağıdaki örnek, Sqlite veritabanından verilerin nasıl çıkarılacağını gösterir:

```csharp
// DbConnection nesnesi oluştur
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Veritabanından tabloları çıkarmak için bir Parser sınıfı örneği oluşturun
using (Parser parser = new Parser(connection))
{
    // Metin çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Toc çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // tabloların listesini al
    IEnumerable<TocItem> toc = parser.GetToc();
    // Tablolar üzerinde yineleme
    foreach (TocItem i in toc)
    {
        // Tablo adını yazdır
        Console.WriteLine(i.Text);
        // Bir tablo içeriğini metin olarak çıkar
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ayrıca bakınız

* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Yeni bir örneğini başlatır.[`Parser`](../../parser) bir veritabanından veri ayıklamak için sınıf.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| connection | DbConnection | Veritabanı bağlantısı. |
| parserSettings | ParserSettings | Veri ayıklamayı özelleştirmek için kullanılan ayrıştırıcı ayarları. |

### Notlar

**Daha fazla bilgi edin:**

* [Veritabanlarından veri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Kerestecilik](https://docs.groupdocs.com/display/parsernet/Logging)

### Örnekler

Aşağıdaki örnek, Sqlite veritabanından verilerin nasıl çıkarılacağını gösterir:

```csharp
// DbConnection nesnesi oluştur
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Veritabanından tabloları çıkarmak için bir Parser sınıfı örneği oluşturun
using (Parser parser = new Parser(connection))
{
    // Metin çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Toc çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // tabloların listesini al
    IEnumerable<TocItem> toc = parser.GetToc();
    // Tablolar üzerinde yineleme
    foreach (TocItem i in toc)
    {
        // Tablo adını yazdır
        Console.WriteLine(i.Text);
        // Bir tablo içeriğini metin olarak çıkar
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ayrıca bakınız

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Yeni bir örneğini başlatır.[`Parser`](../../parser) uzak bir e-posta sunucusundan veri ayıklamak için sınıf.

```csharp
public Parser(EmailConnection connection)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| connection | EmailConnection | E-posta bağlantısı. |

### Notlar

**Daha fazla bilgi edin:**

* [POP, IMAP veya Exchange Web Hizmetleri protokolleri aracılığıyla uzak sunucudan e-postaları ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Örnekler

Aşağıdaki örnek, Exchange Server'dan e-postaların nasıl çıkarılacağını gösterir:

```csharp
// Exchange Web Hizmetleri protokolü için bağlantı nesnesini oluşturun 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Uzak sunucudan e-postaları ayıklamak için bir Parser sınıfı örneği oluşturun
using (Parser parser = new Parser(connection))
{
    // Konteyner çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// E-posta mesajlarını sunucudan çıkarın
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Ekler üzerinde yinele
    foreach (ContainerItem item in emails)
    {
        // E-posta mesajı için bir Parser sınıfı örneği oluşturun
        using (Parser emailParser = item.OpenParser())
        {
            // E-posta metnini ayıklayın
            using (TextReader reader = emailParser.GetText())
            {
                // E-posta metnini yazdır
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Ayrıca bakınız

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Yeni bir örneğini başlatır.[`Parser`](../../parser) uzak bir e-posta sunucusundan veri ayıklamak için sınıf.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| connection | EmailConnection | E-posta bağlantısı. |
| parserSettings | ParserSettings | Veri ayıklamayı özelleştirmek için kullanılan ayrıştırıcı ayarları. |

### Notlar

**Daha fazla bilgi edin:**

* [POP, IMAP veya Exchange Web Hizmetleri protokolleri aracılığıyla uzak sunucudan e-postaları ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Kerestecilik](https://docs.groupdocs.com/display/parsernet/Logging)

### Örnekler

Aşağıdaki örnek, Exchange Server'dan e-postaların nasıl çıkarılacağını gösterir:

```csharp
// Exchange Web Hizmetleri protokolü için bağlantı nesnesini oluşturun 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Uzak sunucudan e-postaları ayıklamak için bir Parser sınıfı örneği oluşturun
using (Parser parser = new Parser(connection))
{
    // Konteyner çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// E-posta mesajlarını sunucudan çıkarın
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Ekler üzerinde yinele
    foreach (ContainerItem item in emails)
    {
        // E-posta mesajı için bir Parser sınıfı örneği oluşturun
        using (Parser emailParser = item.OpenParser())
        {
            // E-posta metnini ayıklayın
            using (TextReader reader = emailParser.GetText())
            {
                // E-posta metnini yazdır
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Ayrıca bakınız

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_7}

Yeni bir örneğini başlatır.[`Parser`](../../parser) sınıf.

```csharp
public Parser(string filePath)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosyanın yolu. |

### Notlar

**Daha fazla bilgi edin:**

* [Belgeyi yerel diskten yükle](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Örnekler

Aşağıdaki örnek, belgenin yerel diskten nasıl yükleneceğini gösterir:

```csharp
// filePath ile Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Bir metni okuyucuya çıkarın
    using (TextReader reader = parser.GetText())
    {
        // Belgeden bir metin yazdır
        // Metin çıkarma desteklenmiyorsa, bir okuyucu boştur
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Ayrıca bakınız

* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_8}

Yeni bir örneğini başlatır.[`Parser`](../../parser) ile sınıf[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosyanın yolu. |
| loadOptions | LoadOptions | Dosyayı açma seçenekleri. |

### Notlar

**Daha fazla bilgi edin:**

* [Belirli dosya formatlarını yükleme](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Parola korumalı belgeleri yükleme](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Belgeyi yerel diskten yükle](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Örnekler

Belge parolası, LoadOptions sınıfı tarafından iletilir:

```csharp
try
{
    // Parser sınıfının bir örneğini şu parolayla oluşturun:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Metin çıkarmanın desteklenip desteklenmediğini kontrol edin
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Belge metnini yazdır
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Parola yanlış veya boşsa mesajı yazdır
    Console.WriteLine("Invalid password");
}
```

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_9}

Yeni bir örneğini başlatır.[`Parser`](../../parser) ile sınıf[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) ve[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| filePath | String | Dosyanın yolu. |
| loadOptions | LoadOptions | Dosyayı açma seçenekleri. |
| parserSettings | ParserSettings | Veri ayıklamayı özelleştirmek için kullanılan ayrıştırıcı ayarları. |

### Notlar

**Daha fazla bilgi edin:**

* [Belirli dosya formatlarını yükleme](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Parola korumalı belgeleri yükleme](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Kerestecilik](https://docs.groupdocs.com/display/parsernet/Logging)
* [Belgeyi yerel diskten yükle](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Örnekler

Aşağıdaki örnek, bilgilerin nasıl alınacağını gösterir.[`ILogger`](../../../groupdocs.parser.options/ilogger) arayüz:

```csharp
// denemek
{
    // Logger sınıfının bir örneğini oluşturun
    Logger logger = new Logger();
    // Ayrıştırıcı ayarlarıyla Parser sınıfının bir örneğini oluşturun
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Metin çıkarmanın desteklenip desteklenmediğini kontrol edin
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Belge metnini yazdır
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // istisnayı yoksay
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Hata mesajını yazdır
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Olay mesajını yazdır
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Uyarı mesajını yazdır
        Console.WriteLine("Warning: " + message);
    }
}
```

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Yeni bir örneğini başlatır.[`Parser`](../../parser) sınıf.

```csharp
public Parser(Stream document)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| document | Stream | Kaynak giriş akışı. |

### Notlar

**Daha fazla bilgi edin:**

* [Akıştan belge yükle](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Örnekler

Aşağıdaki örnek, belgenin akıştan nasıl yükleneceğini gösterir:

```csharp
// Akış ile Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(stream))
{
    // Bir metni okuyucuya çıkarın
    using (TextReader reader = parser.GetText())
    {
        // Belgeden bir metin yazdır
        // Metin çıkarma desteklenmiyorsa, bir okuyucu boştur
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Ayrıca bakınız

* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Yeni bir örneğini başlatır.[`Parser`](../../parser) ile sınıf[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| document | Stream | Kaynak giriş akışı. |
| loadOptions | LoadOptions | Dosyayı açma seçenekleri. |

### Notlar

**Daha fazla bilgi edin:**

* [Belirli dosya formatlarını yükleme](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Parola korumalı belgeleri yükleme](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Akıştan belge yükle](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Örnekler

Bazı durumlarda tanımlamak gerekir[`FileFormat`](../../../groupdocs.parser.options/fileformat). Hem özel durumlar için (veritabanları, e-posta sunucusu) hem de içeriğe göre dosya türlerini algılamak için:

Belge şifresi tarafından iletilir[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) sınıf:

```csharp
// İşaretleme belgesi için bir Parser sınıfı örneği oluşturun
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Metin çıkarmanın desteklenip desteklenmediğini kontrol edin
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Belge metnini yazdır
        // İşaretleme algılandı; özel simgeler içermeyen metin yazdırılır
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Parser sınıfının bir örneğini şu parolayla oluşturun:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Metin çıkarmanın desteklenip desteklenmediğini kontrol edin
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Belge metnini yazdır
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Parola yanlış veya boşsa mesajı yazdır
    Console.WriteLine("Invalid password");
}
```

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Yeni bir örneğini başlatır.[`Parser`](../../parser) ile sınıf[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) ve[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| document | Stream | Kaynak giriş akışı. |
| loadOptions | LoadOptions | Dosyayı açma seçenekleri. |
| parserSettings | ParserSettings | Veri ayıklamayı özelleştirmek için kullanılan ayrıştırıcı ayarları. |

### Notlar

**Daha fazla bilgi edin:**

* [Belirli dosya formatlarını yükleme](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Parola korumalı belgeleri yükleme](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Akıştan belge yükle](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Kerestecilik](https://docs.groupdocs.com/display/parsernet/Logging)

### Örnekler

Aşağıdaki örnek, bilgilerin nasıl alınacağını gösterir.[`ILogger`](../../../groupdocs.parser.options/ilogger) arayüz:

```csharp
// denemek
{
    // Logger sınıfının bir örneğini oluşturun
    Logger logger = new Logger();
    // Ayrıştırıcı ayarlarıyla Parser sınıfının bir örneğini oluşturun
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Metin çıkarmanın desteklenip desteklenmediğini kontrol edin
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Belge metnini yazdır
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // istisnayı yoksay
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Hata mesajını yazdır
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Olay mesajını yazdır
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Uyarı mesajını yazdır
        Console.WriteLine("Warning: " + message);
    }
}
```

### Ayrıca bakınız

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
