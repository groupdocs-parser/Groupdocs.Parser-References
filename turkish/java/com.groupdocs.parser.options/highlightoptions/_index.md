---
title: "HighlightOptions"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Arama senaryolarında bulunan metnin etrafındaki bir metin bloğunu vurgulamak için kullanılan seçenekleri sağlar."
type: docs
weight: 22
url: /tr/java/com.groupdocs.parser.options/highlightoptions/
---
**Inheritance:**
java.lang.Object
```
public class HighlightOptions
```

Vurgulama (arama senaryolarında bulunan metnin etrafındaki metin bloğu) çıkarmak için kullanılan seçenekleri sağlar.

[HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının bir örneği, [Parser.getHighlight(int, boolean, HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--HighlightOptions-) metodunda parametre olarak kullanılır.
Oradaki kullanım örneklerine bakın.

**Learn more:**

* [Extract highlights](../https://docs.groupdocs.com/display/parserjava/Extract+highlights)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Hiçbir sınırlama ayarlanmamış yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır. |
|
|  | [HighlightOptions(int maxLength)](#HighlightOptions-int-) | Sabit uzunlukta bir vurgulama çıkarmak için kullanılan yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır. |
|
|  | [HighlightOptions(Integer maxLength, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-boolean-) | Satır sınırlı bir vurgulama çıkarmak için kullanılan yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır. |
|
|  | [HighlightOptions(Integer maxLength, int wordCount)](#HighlightOptions-java.lang.Integer-int-) | Sabit kelime sayısı ile bir vurgulama çıkarmak için kullanılan yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır. |
|
|  | [HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)](#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-) | Yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getMaxLength()](#getMaxLength--) | Azami metin uzunluğunu alır. |
|
|  | [getWordCount()](#getWordCount--) | Azami kelime sayısını alır. |
|
|  | [isLineLimited()](#isLineLimited--) | Vurgulama çıkarımının bir metin satırının başlangıcı (veya sonu) tarafından sınırlanıp sınırlanmadığını gösteren değeri alır. |
|
|  | [setMaxLength(Integer maxLength)](#setMaxLength-java.lang.Integer-) | Maksimum metin uzunluğunu ayarlar. |
|
|  | [setWordCount(Integer wordCount)](#setWordCount-java.lang.Integer-) | Maksimum kelime sayısını ayarlar. |
|
|  | [setLineLimited(boolean lineLimited)](#setLineLimited-boolean-) | Vurgulama çıkarımının bir metin satırının başlangıcı (veya sonu) tarafından sınırlanıp sınırlanmadığını gösteren değeri ayarlar. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Hiçbir sınırlama ayarlanmamış şekilde [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının yeni bir örneğini başlatır. Ayrıştırıcıya geçmeden önce #setMaxLength(Integer).setMaxLength(Integer), #setWordCount(Integer).setWordCount(Integer), #setLineLimited(boolean).setLineLimited(boolean) öğelerinden en az birini ayarlayın.


### HighlightOptions(int maxLength) {#HighlightOptions-int-}
```
public HighlightOptions(int maxLength)
```


Sabit uzunlukta bir vurgulama çıkarmak için kullanılan yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | maxLength | int | Maksimum metin uzunluğu. |
|

### HighlightOptions(Integer maxLength, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, boolean isLineLimited)
```


Satır sınırlı bir vurgulama çıkarmak için kullanılan yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Maksimum metin uzunluğu. |
|
|  | isLineLimited | boolean | Vurgulama çıkarımının bir metin satırının başlangıcı (veya sonu) tarafından sınırlanıp sınırlanmadığını gösteren değer. |
|

### HighlightOptions(Integer maxLength, int wordCount) {#HighlightOptions-java.lang.Integer-int-}
```
public HighlightOptions(Integer maxLength, int wordCount)
```


Sabit kelime sayısı ile bir vurgulama çıkarmak için kullanılan yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Maksimum metin uzunluğu. |
|
|  | wordCount | int | Maksimum kelime sayısı. |
|

### HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited) {#HighlightOptions-java.lang.Integer-java.lang.Integer-boolean-}
```
public HighlightOptions(Integer maxLength, Integer wordCount, boolean isLineLimited)
```


Yeni bir [HighlightOptions](../../com.groupdocs.parser.options/highlightoptions) sınıfının örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Maksimum metin uzunluğu. |
|
|  | wordCount | java.lang.Integer | Maksimum kelime sayısı. |
|
|  | isLineLimited | boolean | Vurgulama çıkarımının bir metin satırının başlangıcı (veya sonu) tarafından sınırlanıp sınırlanmadığını gösteren değer. |
|

### getMaxLength() {#getMaxLength--}
```
public Integer getMaxLength()
```


Azami metin uzunluğunu alır.


**Returns:**
java.lang.Integer - Maksimum metin uzunluğunu temsil eden pozitif bir tamsayı değeri;  null  eğer metin uzunluğu sınırlı değilse.

### getWordCount() {#getWordCount--}
```
public Integer getWordCount()
```


Azami kelime sayısını alır.


**Returns:**
java.lang.Integer - Maksimum kelime sayısını temsil eden pozitif bir tamsayı değeri;  null  eğer kelime sayısı sınırlı değilse.

### isLineLimited() {#isLineLimited--}
```
public boolean isLineLimited()
```


Vurgulama çıkarımının bir metin satırının başlangıcı (veya sonu) tarafından sınırlanıp sınırlanmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer vurgulama çıkarımı bir metin satırının başlangıcı (veya sonu) tarafından sınırlanıyorsa; aksi takdirde,  false .

### setMaxLength(Integer maxLength) {#setMaxLength-java.lang.Integer-}
```
public void setMaxLength(Integer maxLength)
```


Maksimum metin uzunluğunu ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | maxLength | java.lang.Integer | Negatif olmayan bir tamsayı;  null  uzunluk sınırlamasını kaldırmak için. |
|

### setWordCount(Integer wordCount) {#setWordCount-java.lang.Integer-}
```
public void setWordCount(Integer wordCount)
```


Maksimum kelime sayısını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | wordCount | java.lang.Integer | Negatif olmayan bir tamsayı;  null  kelime sayısı sınırlamasını kaldırmak için. |
|

### setLineLimited(boolean lineLimited) {#setLineLimited-boolean-}
```
public void setLineLimited(boolean lineLimited)
```


Vurgulama çıkarımının bir metin satırının başlangıcı (veya sonu) tarafından sınırlanıp sınırlanmadığını gösteren değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | lineLimited | boolean | true  satır sınırlarıyla sınırlamak için. |
|

