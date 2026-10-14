---
title: "FormattedTextOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Biçimlendirilmiş metin çıkarımı için kullanılan seçenekleri sağlar."
type: docs
weight: 21
url: /tr/java/com.groupdocs.parser.options/formattedtextoptions/
---
**Inheritance:**
java.lang.Object
```
public class FormattedTextOptions
```

Biçimlendirilmiş metin çıkarımı için kullanılan seçenekleri sağlar.

Bir [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sınıfının örneği, [Parser.getFormattedText(FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-FormattedTextOptions-) metodunda parametre olarak kullanılır.
ve [Parser.getFormattedText(int, FormattedTextOptions)](../../com.groupdocs.parser/parser#getFormattedText-int--FormattedTextOptions-) metodları. Oradaki kullanım örneklerine bakın.

**Learn more:**

* [Extract formatted text from document](../https://docs.groupdocs.com/display/parserjava/Extract+formatted+text+from+document)
* Extract a document text as [HTML](../https://docs.groupdocs.com/display/parserjava/HTML)
* Extract a document text as [Markdown](../https://docs.groupdocs.com/display/parserjava/Markdown)
* Extract a document text as [Plain text](../https://docs.groupdocs.com/display/parserjava/Plain+text)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [FormattedTextOptions()](#FormattedTextOptions--) | Hiçbir mod ayarlanmamış şekilde [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sınıfının yeni bir örneğini başlatır. |
|
|  | [FormattedTextOptions(FormattedTextMode mode)](#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-) | Yeni bir [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sınıfı örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getMode()](#getMode--) | Biçimlendirilmiş metin çıkarma modunu alır. |
|
|  | [setMode(FormattedTextMode mode)](#setMode-com.groupdocs.parser.options.FormattedTextMode-) | Biçimlendirilmiş metin çıkarma modunu ayarlar. |
|
### FormattedTextOptions() {#FormattedTextOptions--}
```
public FormattedTextOptions()
```


Hiçbir mod ayarlanmamış şekilde [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sınıfının yeni bir örneğini başlatır.


### FormattedTextOptions(FormattedTextMode mode) {#FormattedTextOptions-com.groupdocs.parser.options.FormattedTextMode-}
```
public FormattedTextOptions(FormattedTextMode mode)
```


Yeni bir [FormattedTextOptions](../../com.groupdocs.parser.options/formattedtextoptions) sınıfı örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | Biçimlendirilmiş metin çıkarma modu. |
|

### getMode() {#getMode--}
```
public FormattedTextMode getMode()
```


Biçimlendirilmiş metin çıkarma modunu alır.


**Returns:**
[FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) - [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enumeration that contains a formatted text extraction mode.

### setMode(FormattedTextMode mode) {#setMode-com.groupdocs.parser.options.FormattedTextMode-}
```
public void setMode(FormattedTextMode mode)
```


Biçimlendirilmiş metin çıkarma modunu ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | mode | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) | [FormattedTextMode](../../com.groupdocs.parser.options/formattedtextmode) enum'ı, biçimlendirilmiş metin çıkarma modu içerir. |
|

