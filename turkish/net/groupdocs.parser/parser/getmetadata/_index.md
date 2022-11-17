---
title: GetMetadata
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Belgeden meta verileri çıkarır.
type: docs
weight: 120
url: /tr/net/groupdocs.parser/parser/getmetadata/
---
## Parser.GetMetadata method

Belgeden meta verileri çıkarır.

```csharp
public IEnumerable<MetadataItem> GetMetadata()
```

### Geri dönüş değeri

Meta veri öğeleri koleksiyonu; `hükümsüz` meta veri çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Belgelerden meta verileri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+documents)
* [Microsoft Office Word belgelerinden meta verileri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel elektronik tablolarından meta verileri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint sunumlarından meta verileri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Microsoft+Office+PowerPoint+presentations)
* [PDF belgelerinden meta verileri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+PDF+documents)
* [E-postalardan meta verileri ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+metadata+from+Emails)

### Örnekler

Aşağıdaki örnek, bir belgeden meta verilerin nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Belgeden meta verileri çıkar
    IEnumerable<MetadataItem> metadata = parser.GetMetadata();
    // Meta veri çıkarmanın desteklenip desteklenmediğini kontrol edin
    if(metadata == null)
    {
        Console.WriteLine("Metatada extraction isn't supported");
    }
 
    // Meta veri öğeleri üzerinde yineleme yapın
    foreach(MetadataItem item in metadata)
    {
        // Bir öğe adı ve değeri yazdır
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Value));
    }
}
```

### Ayrıca bakınız

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->