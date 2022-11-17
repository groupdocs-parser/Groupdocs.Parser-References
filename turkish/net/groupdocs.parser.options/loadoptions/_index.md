---
title: LoadOptions
second_title: .NET API Başvurusu için GroupDocs.Parser
description: Bir dosyayı açmak için kullanılan seçenekleri sağlar.
type: docs
weight: 450
url: /tr/net/groupdocs.parser.options/loadoptions/
---
## LoadOptions class

Bir dosyayı açmak için kullanılan seçenekleri sağlar.

```csharp
public sealed class LoadOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Yeni bir örneğini başlatır.[`LoadOptions`](../loadoptions) boş olan sınıf [`Password`](./password) ,[`FileFormat`](./fileformat) eşittirUnknown ve varsayılan kodlamalar. |
| [LoadOptions](loadoptions#constructor_1)(FileFormat) | Yeni bir örneğini başlatır.[`LoadOptions`](../loadoptions) class ile boş[`Password`](./password) ve varsayılan kodlamalar. |
| [LoadOptions](loadoptions#constructor_4)(string) | Yeni bir örneğini başlatır.[`LoadOptions`](../loadoptions)class ile[`FileFormat`](./fileformat) eşittirUnknown ve varsayılan kodlamalar. |
| [LoadOptions](loadoptions#constructor_2)(FileFormat, string) | Yeni bir örneğini başlatır.[`LoadOptions`](../loadoptions) parola ve varsayılan kodlamalar ile sınıf. |
| [LoadOptions](loadoptions#constructor_3)(FileFormat, string, Encoding, Encoding) | Yeni bir örneğini başlatır.[`LoadOptions`](../loadoptions) özel kodlamalara sahip sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DefaultAnsiEncoding](../../groupdocs.parser.options/loadoptions/defaultansiencoding) { get; } | Kodlama tespiti için kullanılan varsayılan ANSI kodlamasını alır. |
| [Encoding](../../groupdocs.parser.options/loadoptions/encoding) { get; } | Belgenin kodlamasını alır. |
| [FileFormat](../../groupdocs.parser.options/loadoptions/fileformat) { get; } | Dosya biçimini alır. |
| [Password](../../groupdocs.parser.options/loadoptions/password) { get; } | Parolayı alır. |

### Notlar

Bu sınıfın bir örneği parametre olarak kullanılır.[`Parser`](../../groupdocs.parser/parser) sınıf kurucuları:

* [`Parser`](../../groupdocs.parser/parser/parser)
* [`Parser`](../../groupdocs.parser/parser/parser)

Oradaki kullanım örneklerine bakın.

**Daha fazla bilgi edin:**

* [Belirli dosya formatlarını yükleme](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Parola korumalı belgeleri yükleme](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)

### Ayrıca bakınız

* ad alanı [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* toplantı [GroupDocs.Parser](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->