---
title: GetDocumentInfo
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Belge hakkında genel bilgileri döndürür.
type: docs
weight: 70
url: /tr/net/groupdocs.parser/parser/getdocumentinfo/
---
## Parser.GetDocumentInfo method

Belge hakkında genel bilgileri döndürür.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Geri dönüş değeri

Uygulayan bir sınıf örneği[`IDocumentInfo`](../../../groupdocs.parser.options/idocumentinfo) arayüz.

### Notlar

**Daha fazla bilgi edin:**

* [Belge bilgilerini al](https://docs.groupdocs.com/display/parsernet/Get+document+info)
* [Kodlamayı algıla](https://docs.groupdocs.com/display/parsernet/Detect+encoding)

### Örnekler

Aşağıdaki örnek, belge bilgilerinin nasıl alınacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Belge bilgilerini al
    IDocumentInfo info = parser.GetDocumentInfo();

    Console.WriteLine(string.Format("FileType: {0}", info.FileType));
    Console.WriteLine(string.Format("PageCount: {0}", info.PageCount));
    Console.WriteLine(string.Format("Size: {0}", info.Size));
}
```

### Ayrıca bakınız

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
