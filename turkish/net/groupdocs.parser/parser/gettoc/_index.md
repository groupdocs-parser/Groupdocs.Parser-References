---
title: GetToc
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Belgeden içindekiler tablosunu çıkarır.
type: docs
weight: 170
url: /tr/net/groupdocs.parser/parser/gettoc/
---
## Parser.GetToc method

Belgeden içindekiler tablosunu çıkarır.

```csharp
public IEnumerable<TocItem> GetToc()
```

### Geri dönüş değeri

İçindekiler tablosu öğeleri koleksiyonu; `hükümsüz` içindekiler tablosu çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [İçindekiler tablosunu çıkar](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents)
* [Metni içindekiler tablosuna göre ayıkla](https://docs.groupdocs.com/display/parsernet/Extract+text+by+table+of+contents+item)
* [Microsoft Office Word belgelerinden içindekiler tablosunu çıkarın](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+Microsoft+Office+Word+documents)
* [EPUB e-Kitaplarından içindekiler tablosunu çıkarın](https://docs.groupdocs.com/display/parsernet/Extract+table+of+contents+from+EPUB+eBooks)

### Örnekler

Aşağıdaki örnek, içindekiler tablosunun CHM dosyasından nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
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
 
    // içindekiler tablosunu al
    IEnumerable<TocItem> toc = parser.GetToc();
    
    // Öğeler üzerinde yineleme
    foreach (TocItem i in toc)
    {
        // Toc metnini yazdır
        Console.WriteLine(i.Text);
        // Sayfa dizininin bir değeri olup olmadığını kontrol edin
        if (i.PageIndex == null)
        {
            continue;
        }
        // Bir sayfa metnini ayıklayın
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ayrıca bakınız

* class [TocItem](../../../groupdocs.parser.data/tocitem)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->