---
title: GetTables
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Tabloları belgeden çıkarır.
type: docs
weight: 140
url: /tr/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

Tabloları belgeden çıkarır.

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | PageTableAreaOptions | Tablo çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) nesneler; `hükümsüz` tablo çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, tabloların tüm belgeden nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgenin tablo çıkarmayı destekleyip desteklemediğini kontrol edin
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Tabloların düzenini oluştur
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Tablo çıkarma için seçenekler oluşturun
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Belgeden tabloları çıkar
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // Tablolar üzerinde yineleme
    foreach (PageTableArea t in tables)
    {
        // Satırları yinele
        for (int row = 0; row < t.RowCount; row++)
        {
            // Sütunlar üzerinde yinele
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // Tablo hücresini al
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // Tablo hücre metnini yazdır
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### Ayrıca bakınız

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

Tabloları belge sayfasından çıkarır.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |
| options | PageTableAreaOptions | Tablo çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) nesneler; `hükümsüz` tablo çıkarma desteklenmiyorsa.

### Örnekler

Aşağıdaki örnek, tabloların belge sayfasından nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using (Parser parser = new Parser(filePath))
{
    // Belgenin tablo çıkarmayı destekleyip desteklemediğini kontrol edin
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // Tabloların düzenini oluştur
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // Tablo çıkarma için seçenekler oluşturun
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // Belge bilgilerini al
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // Belgenin sayfaları olup olmadığını kontrol edin
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // Sayfalar üzerinde yinele
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // Bir sayfa numarası yazdır 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // Belge sayfasından tabloları çıkar
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // Tablolar üzerinde yineleme
        foreach (PageTableArea t in tables)
        {
            // Satırları yinele
            for (int row = 0; row < t.RowCount; row++)
            {
                // Sütunlar üzerinde yinele
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // Tablo hücresini al
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // Tablo hücre metnini yazdır
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### Ayrıca bakınız

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
