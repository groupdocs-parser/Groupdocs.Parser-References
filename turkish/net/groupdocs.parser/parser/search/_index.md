---
title: Search
second_title: .NET API Başvurusu için GroupDocs.Parser
description: keyword belgede.
type: docs
weight: 200
url: /tr/net/groupdocs.parser/parser/search/
---
## Search(string) {#search}

*keyword* belgede.

```csharp
public IEnumerable<SearchResult> Search(string keyword)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| keyword | String | Aranacak anahtar kelime. |

### Geri dönüş değeri

Koleksiyonu[`SearchResult`](../../../groupdocs.parser.data/searchresult) nesneler; `hükümsüz` arama desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Arama metni](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Microsoft Office Word belgelerinde metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Microsoft Office Excel elektronik tablolarında metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint sunumlarında metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [PDF belgelerinde metin ara](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [E-postalarda metin ara](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [EPUB e-Kitaplarında metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [HTML belgelerinde metin ara](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Microsoft OneNote bölümlerinde metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Örnekler

Aşağıdaki örnek, bir belgede bir anahtar kelimenin nasıl bulunacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Bir anahtar kelime arayın:
    IEnumerable<SearchResult> sr = parser.Search("page number");
    // Aramanın desteklenip desteklenmediğini kontrol edin
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Arama sonuçlarını yinele
    foreach(SearchResult s in sr)
    {
        // Bir dizin ve bulunan metni yazdırın:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

### Ayrıca bakınız

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## Search(string, SearchOptions) {#search_1}

*keyword*arama seçeneklerini (normal ifade, eşleşme durumu vb.) kullanarak belgede.

```csharp
public IEnumerable<SearchResult> Search(string keyword, SearchOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| keyword | String | Aranacak anahtar kelime. |
| options | SearchOptions | Arama seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`SearchResult`](../../../groupdocs.parser.data/searchresult) nesneler; `hükümsüz` arama desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Arama metni](https://docs.groupdocs.com/display/parsernet/Search+text)
* [Microsoft Office Word belgelerinde metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Word+documents)
* [Microsoft Office Excel elektronik tablolarında metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint sunumlarında metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+Office+PowerPoint+presentations)
* [PDF belgelerinde metin ara](https://docs.groupdocs.com/display/parsernet/Search+text+in+PDF+documents)
* [E-postalarda metin ara](https://docs.groupdocs.com/display/parsernet/Search+text+in+Emails)
* [EPUB e-Kitaplarında metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+EPUB+eBooks)
* [HTML belgelerinde metin ara](https://docs.groupdocs.com/display/parsernet/Search+text+in+HTML+documents)
* [Microsoft OneNote bölümlerinde metin arama](https://docs.groupdocs.com/display/parsernet/Search+text+in+Microsoft+OneNote+sections)

### Örnekler

Aşağıdaki örnek, bir belgede normal ifadeyle nasıl arama yapılacağını gösterir:

Aşağıdaki örnek, sayfalarda bir metnin nasıl aranacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Büyük/küçük harf eşleştirmeli normal ifade ile arama yapın
    IEnumerable<SearchResult> sr = parser.Search("page number: [0-9]+", new SearchOptions(true, false, true));
    // Aramanın desteklenip desteklenmediğini kontrol edin
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Arama sonuçlarını yinele
    foreach(SearchResult s in sr)
    {
        // Bir dizin ve bulunan metni yazdırın:
        Console.WriteLine(string.Format("At {0}: {1}", s.Position, s.Text));
    }
}
```

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Sayfa numaralarıyla bir anahtar kelime arayın
    IEnumerable<SearchResult> sr = parser.Search("line", new SearchOptions(false, false, false, true));
    // Aramanın desteklenip desteklenmediğini kontrol edin
    if(sr == null)
    {
        Console.WriteLine("Search isn't supported");
        return;
    }
 
    // Arama sonuçlarını yinele
    foreach(SearchResult s in sr)
    {
        // Bir dizin, sayfa numarası ve bulunan metni yazdırın:
        Console.WriteLine(string.Format("At {0} (page {1}): {2}", s.Position, s.PageIndex, s.Text));
    }
}
```

### Ayrıca bakınız

* class [SearchResult](../../../groupdocs.parser.data/searchresult)
* class [SearchOptions](../../../groupdocs.parser.options/searchoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
