---
title: Parser
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Metin resimler kapsayıcı çıkarma ve ayrıştırma işlevselliğini kontrol eden ana sınıfı temsil eder.
type: docs
weight: 590
url: /tr/net/groupdocs.parser/parser/
---
## Parser class

Metin, resimler, kapsayıcı çıkarma ve ayrıştırma işlevselliğini kontrol eden ana sınıfı temsil eder.

```csharp
public sealed class Parser : IDisposable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Parser](parser#constructor_2)(DbConnection) | Yeni bir örneğini başlatır.[`Parser`](../parser) bir veritabanından veri ayıklamak için sınıf. |
| [Parser](parser#constructor)(EmailConnection) | Yeni bir örneğini başlatır.[`Parser`](../parser) uzak bir e-posta sunucusundan veri ayıklamak için sınıf. |
| [Parser](parser#constructor_4)(Stream) | Yeni bir örneğini başlatır.[`Parser`](../parser) sınıf. |
| [Parser](parser#constructor_7)(string) | Yeni bir örneğini başlatır.[`Parser`](../parser) sınıf. |
| [Parser](parser#constructor_3)(DbConnection, ParserSettings) | Yeni bir örneğini başlatır.[`Parser`](../parser) bir veritabanından veri ayıklamak için sınıf. |
| [Parser](parser#constructor_1)(EmailConnection, ParserSettings) | Yeni bir örneğini başlatır.[`Parser`](../parser) uzak bir e-posta sunucusundan veri ayıklamak için sınıf. |
| [Parser](parser#constructor_5)(Stream, LoadOptions) | Yeni bir örneğini başlatır.[`Parser`](../parser) ile sınıf[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_8)(string, LoadOptions) | Yeni bir örneğini başlatır.[`Parser`](../parser) ile sınıf[`LoadOptions`](../../groupdocs.parser.options/loadoptions) . |
| [Parser](parser#constructor_6)(Stream, LoadOptions, ParserSettings) | Yeni bir örneğini başlatır.[`Parser`](../parser) ile sınıf[`LoadOptions`](../../groupdocs.parser.options/loadoptions) ve[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |
| [Parser](parser#constructor_9)(string, LoadOptions, ParserSettings) | Yeni bir örneğini başlatır.[`Parser`](../parser) ile sınıf[`LoadOptions`](../../groupdocs.parser.options/loadoptions) ve[`ParserSettings`](../../groupdocs.parser.options/parsersettings) . |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Features](../../groupdocs.parser/parser/features) { get; } | Desteklenen özellikleri alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [Dispose](../../groupdocs.parser/parser/dispose)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [GeneratePreview](../../groupdocs.parser/parser/generatepreview)(PreviewOptions) | Sayfa önizlemesini alın. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes)() | Belgeden barkodları çıkarır. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_2)(int) | Belge sayfasından barkodları çıkarır. |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_1)(PageAreaOptions) | Özelleştirme seçeneklerini kullanarak belgeden barkodları çıkarır (barkodları içeren dikdörtgen alanı ayarlamak için). |
| [GetBarcodes](../../groupdocs.parser/parser/getbarcodes#getbarcodes_3)(int, PageAreaOptions) | Özelleştirme seçeneklerini kullanarak belge sayfasından barkodları çıkarır (barkodları içeren dikdörtgen alanı ayarlamak için). |
| [GetContainer](../../groupdocs.parser/parser/getcontainer)() | Ekler, ZIP arşivleri vb. içeren biçimlerle çalışmak için belgeden bir konteyner nesnesi çıkarır. |
| [GetDocumentInfo](../../groupdocs.parser/parser/getdocumentinfo)() | Belge hakkında genel bilgileri döndürür. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext)(FormattedTextOptions) | Belgeden biçimlendirilmiş bir metin çıkarır. |
| [GetFormattedText](../../groupdocs.parser/parser/getformattedtext#getformattedtext_1)(int, FormattedTextOptions) | Belge sayfasından biçimlendirilmiş bir metin çıkarır. |
| [GetHighlight](../../groupdocs.parser/parser/gethighlight)(int, bool, HighlightOptions) | Belgeden bir vurgu çıkarır. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks)() | Belgeden köprüleri çıkarır. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_2)(int) | Belge sayfasından köprüleri çıkarır. |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_1)(PageAreaOptions) | Özelleştirme seçeneklerini kullanarak belgeden köprüleri çıkarır (köprüleri içeren dikdörtgen alanı ayarlamak için). |
| [GetHyperlinks](../../groupdocs.parser/parser/gethyperlinks#gethyperlinks_3)(int, PageAreaOptions) | Özelleştirme seçeneklerini kullanarak belge sayfasından köprüleri çıkarır (köprüleri içeren dikdörtgen alanı ayarlamak için). |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages)() | Belgeden görüntüleri ayıklar. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_2)(int) | Belge sayfasından görüntüleri ayıklar. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_1)(PageAreaOptions) | (görüntüleri içeren dikdörtgen alanı ayarlamak için) özelleştirme seçeneklerini kullanarak görüntüleri belgeden çıkarır. |
| [GetImages](../../groupdocs.parser/parser/getimages#getimages_3)(int, PageAreaOptions) | Özelleştirme seçeneklerini kullanarak belge sayfasından görüntüleri çıkarır (resimleri içeren dikdörtgen alanı ayarlamak için). |
| [GetMetadata](../../groupdocs.parser/parser/getmetadata)() | Belgeden meta verileri çıkarır. |
| [GetStructure](../../groupdocs.parser/parser/getstructure)() | Belgeden yapılandırılmış bir metin çıkarır. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables)(PageTableAreaOptions) | Tabloları belgeden çıkarır. |
| [GetTables](../../groupdocs.parser/parser/gettables#gettables_1)(int, PageTableAreaOptions) | Tabloları belge sayfasından çıkarır. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext)() | Belgeden bir metin çıkarır. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_2)(int) | Belge sayfasından bir metin çıkarır. |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_1)(TextOptions) | Metin seçeneklerini kullanarak belgeden bir metin sayfası çıkarır (ham hızlı metin çıkarma modunu etkinleştirmek için). |
| [GetText](../../groupdocs.parser/parser/gettext#gettext_3)(int, TextOptions) | Metin seçeneklerini kullanarak belge sayfasından bir metin çıkarır (ham hızlı metin çıkarma modunu etkinleştirmek için). |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas)() | Metin alanlarını belgeden çıkarır. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_2)(int) | Metin alanlarını belge sayfasından çıkarır. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_1)(PageTextAreaOptions) | Özelleştirme seçeneklerini (normal ifade, büyük/küçük harf eşleştirme vb.) kullanarak belgeden metin alanlarını çıkarır. |
| [GetTextAreas](../../groupdocs.parser/parser/gettextareas#gettextareas_3)(int, PageTextAreaOptions) | Özelleştirme seçeneklerini (normal ifade, büyük/küçük harf eşleştirme vb.) kullanarak belge sayfasından metin alanlarını çıkarır. |
| [GetToc](../../groupdocs.parser/parser/gettoc)() | Belgeden içindekiler tablosunu çıkarır. |
| [ParseByTemplate](../../groupdocs.parser/parser/parsebytemplate)(Template) | Kullanıcı tarafından oluşturulan şablona göre belgeyi ayrıştırır. |
| [ParseForm](../../groupdocs.parser/parser/parseform)() | Belge formunu ayrıştırır. |
| [Search](../../groupdocs.parser/parser/search#search)(string) | *keyword* belgede. |
| [Search](../../groupdocs.parser/parser/search#search_1)(string, SearchOptions) | *keyword*arama seçeneklerini (normal ifade, eşleşme durumu vb.) kullanarak belgede. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo)(Stream) | Bir dosya hakkında genel bilgileri döndürür. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_2)(string) | Bir dosya hakkında genel bilgileri döndürür. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_1)(Stream, LoadOptions) | Bir dosya hakkında genel bilgileri döndürür. |
| static [GetFileInfo](../../groupdocs.parser/parser/getfileinfo#getfileinfo_3)(string, LoadOptions) | Bir dosya hakkında genel bilgileri döndürür. |

### Ayrıca bakınız

* ad alanı [GroupDocs.Parser](../../groupdocs.parser)
* toplantı [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
