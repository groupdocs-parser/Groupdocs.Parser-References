---
title: GetText
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Belgeden bir metin çıkarır.
type: docs
weight: 150
url: /tr/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

Belgeden bir metin çıkarır.

```csharp
public TextReader GetText()
```

### Geri dönüş değeri

Bir örneğiTextReader çıkarılan metinle sınıf; `hükümsüz` metin çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Belgelerden metin ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Metni Doğru modda ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Örnekler

Aşağıdaki örnek, bir belgeden bir metnin nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Bir metni okuyucuya çıkarın
    using(TextReader reader = parser.GetText())
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

## GetText(TextOptions) {#gettext_1}

Metin seçeneklerini kullanarak belgeden bir metin sayfası çıkarır (ham hızlı metin çıkarma modunu etkinleştirmek için).

```csharp
public TextReader GetText(TextOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | TextOptions | Metin çıkarma seçenekleri. |

### Geri dönüş değeri

Bir örneğiTextReader çıkarılan metinle sınıf; `hükümsüz` metin çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Metni Doğru modda ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Metni Ham modda ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Örnekler

Aşağıdaki örnek, bir belgeden ham metnin nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Ham metni okuyucuya çıkarın
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // Belgeden bir metin yazdır
        // Metin çıkarma desteklenmiyorsa, bir okuyucu boştur
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Ayrıca bakınız

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

Belge sayfasından bir metin çıkarır.

```csharp
public TextReader GetText(int pageIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |

### Geri dönüş değeri

Bir örneğiTextReader çıkarılan metinle sınıf; `hükümsüz` metin sayfası çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Metni Doğru modda ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Örnekler

Aşağıdaki örnek, bir metnin belge sayfasından nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Belgenin metin çıkarmayı destekleyip desteklemediğini kontrol edin
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Belge bilgilerini al
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Belgenin sayfaları olup olmadığını kontrol edin
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Sayfalar üzerinde yinele
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // Bir sayfa numarası yazdır 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // Bir metni okuyucuya çıkarın
        using(TextReader reader = parser.GetText(p))
        {
            // Belgeden bir metin yazdır
            // Metin çıkarma özelliği desteğini daha önce kontrol ettiğimiz için boş denetimi yok sayıyoruz
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

## GetText(int, TextOptions) {#gettext_3}

Metin seçeneklerini kullanarak belge sayfasından bir metin çıkarır (ham hızlı metin çıkarma modunu etkinleştirmek için).

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |
| options | TextOptions | Metin çıkarma seçenekleri. |

### Geri dönüş değeri

Bir örneğiTextReader çıkarılan metinle sınıf; `hükümsüz` metin sayfası çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Metni Doğru modda ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Metni Ham modda ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Örnekler

Aşağıdaki örnek, ham metnin belge sayfasından nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Belgenin metin çıkarmayı destekleyip desteklemediğini kontrol edin
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // Belge bilgilerini al
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // Belgenin sayfaları olup olmadığını kontrol edin
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // Sayfalar üzerinde yinele
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // Bir sayfa numarası yazdır 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // Bir metni okuyucuya çıkarın
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // Belgeden bir metin yazdır
            // Metin çıkarma özelliği desteğini daha önce kontrol ettiğimiz için boş denetimi yok sayıyoruz
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ayrıca bakınız

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
