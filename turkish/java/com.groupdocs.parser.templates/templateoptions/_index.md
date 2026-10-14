---
title: "TemplateOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Şablon işlevselliğiyle ayrıştırma için kullanılan seçenekleri sağlar."
type: docs
weight: 17
url: /tr/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

Şablon işlevselliğiyle ayrıştırma için kullanılan seçenekleri sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | Yeni bir [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutunu alır. |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


Yeni bir [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | rectangleTolerance | double | Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutu. Bu, bir metin öğesi yüksekliğinin kesriyle ölçülür. |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


Dikdörtgen alan tarafından yakalandığında göz ardı edilen kenarın boyutunu alır. Bu, bir metin öğesi yüksekliğinin kesriyle ölçülür.


**Returns:**
double - 0 (kenar yok) ile 1 (tüm öğeyi yoksay) arasında bir double değeri.

