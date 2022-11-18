---
title: GetTextAreas
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Metin alanlarını belgeden çıkarır.
type: docs
weight: 160
url: /tr/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

Metin alanlarını belgeden çıkarır.

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### Geri dönüş değeri

Koleksiyonu[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) nesneler; `hükümsüz` metin alanları çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Metin alanlarını ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Örnekler

Aşağıdaki örnek, tüm metin alanlarının tüm belgeden nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Metin alanlarını ayıklayın
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // Metin alanları çıkarmanın desteklenip desteklenmediğini kontrol edin
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Sayfadaki metin alanlarını yinele
    foreach(PageTextArea a in areas)
    {
        // Bir sayfa dizini, dikdörtgen ve metin alanı değeri yazdırın:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Ayrıca bakınız

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

Özelleştirme seçeneklerini (normal ifade, büyük/küçük harf eşleştirme vb.) kullanarak belgeden metin alanlarını çıkarır.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | PageTextAreaOptions | Metin alanı çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) nesneler; `hükümsüz` metin alanları çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Metin alanlarını ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Örnekler

Aşağıdaki örnek, sol üst köşeden yalnızca rakam içeren metin alanlarının nasıl çıkarılacağını gösterir:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Metin alanı çıkarma için kullanılan seçenekleri oluşturun
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // Bir sayfanın sol üst köşesinden yalnızca rakam içeren metin alanlarını çıkarın:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // Metin alanları çıkarmanın desteklenip desteklenmediğini kontrol edin
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // Sayfadaki metin alanlarını yinele
    foreach(PageTextArea a in areas)
    {
        // Bir sayfa dizini, dikdörtgen ve metin alanı değeri yazdırın:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### Ayrıca bakınız

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

Metin alanlarını belge sayfasından çıkarır.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |

### Geri dönüş değeri

Koleksiyonu[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) nesneler; `hükümsüz` metin alanları çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Metin alanlarını ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Örnekler

Bir belge sayfasından metin alanlarını çıkarmak için aşağıdaki yöntem kullanılır:

```csharp
// Parser sınıfının bir örneğini oluşturun
using(Parser parser = new Parser(filePath))
{
    // Belgenin metin alanları çıkarmayı destekleyip desteklemediğini kontrol edin
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
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
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // Bir sayfa numarası yazdır 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // Sayfadaki metin alanlarını yinele
        // Metin alanları çıkarma özelliği desteğini daha önce kontrol ettiğimiz için boş denetimi görmezden geliyoruz
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // Bir dikdörtgen ve metin alanı değeri yazdırın:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### Ayrıca bakınız

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

Özelleştirme seçeneklerini (normal ifade, büyük/küçük harf eşleştirme vb.) kullanarak belge sayfasından metin alanlarını çıkarır.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| pageIndex | Int32 | Sıfır tabanlı sayfa dizini. |
| options | PageTextAreaOptions | Metin alanı çıkarma seçenekleri. |

### Geri dönüş değeri

Koleksiyonu[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) nesneler; `hükümsüz` metin alanları çıkarma desteklenmiyorsa.

### Notlar

**Daha fazla bilgi edin:**

* [Metin alanlarını ayıklayın](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Ayrıca bakınız

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* ad alanı [GroupDocs.Parser](../../parser)
* toplantı [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
