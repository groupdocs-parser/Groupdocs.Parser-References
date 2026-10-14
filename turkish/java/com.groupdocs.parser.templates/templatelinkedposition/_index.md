---
title: "TemplateLinkedPosition"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Bağlantılı alanı kullanan bir şablon alan konumunu sağlar."
type: docs
weight: 15
url: /tr/java/com.groupdocs.parser.templates/templatelinkedposition/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
```
public class TemplateLinkedPosition extends TemplatePosition
```

Bağlantılı alanı kullanan bir şablon alan konumunu sağlar.

Aşağıdaki örnek, fatura numarası alanının bilindiği durumu gösteren kodu sunar
"Invoice number" dizesinin sağında konumlandırılmışsa aşağıdaki kod kullanılır:

````
// Create a regex template field to find "Invoice Number" text
 TemplateField invoice = new TemplateField(new TemplateRegexPosition("Invoice Number"), "Invoice");

 // Create a related template field associated with "Invoice" field and extract the value on the right of it
 TemplateField invoiceNumber = new TemplateField(
     new TemplateLinkedPosition("invoice", new Size(100, 15), new TemplateLinkedPositionEdges(false, false, true, false)),
     "InvoiceNumber");
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-) | [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-) | UPPER CASE adıyla [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) sınıfının yeni bir örneğini başlatır. |
|
|  | [TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)](#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-) | [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getLinkedFieldName()](#getLinkedFieldName--) | Bağlantılı alan adını alır. |
|
|  | [getSearchArea()](#getSearchArea--) | Bir alanın arandığı bölgenin boyutunu alır. |
|
|  | [isAutoScale()](#isAutoScale--) | Bağlantılı alan boyutu tarafından  SearchArea  ölçeklendirilip ölçeklendirilmediğini gösteren değeri alır. |
|
|  | [getEdges()](#getEdges--) | Bir alanın arandığı bağlantılı alanın kenarlarını alır. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges)
```


[TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Bağlantılı alanın adı. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Bir alanın arandığı bölgenin boyutu. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Bir alanın arandığı bağlantılı alanın kenarları. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale)
```


UPPER CASE adıyla [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Bağlantılı alanın adı. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Bir alanın arandığı bölgenin boyutu. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Bir alanın arandığı bağlantılı alanın kenarları. |
|
|  | autoScale | boolean | Bağlantılı alan boyutu tarafından searchArea ölçeklendirilip ölçeklendirilmediğini gösteren değer. |
|

### TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName) {#TemplateLinkedPosition-java.lang.String-com.groupdocs.parser.data.Size-com.groupdocs.parser.templates.TemplateLinkedPositionEdges-boolean-boolean-}
```
public TemplateLinkedPosition(String linkedFieldName, Size searchArea, TemplateLinkedPositionEdges edges, boolean autoScale, boolean useUpperCaseName)
```


[TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | linkedFieldName | java.lang.String | Bağlantılı alanın adı. |
|
|  | searchArea | [Size](../../com.groupdocs.parser.data/size) | Bir alanın arandığı bölgenin boyutu. |
|
|  | edges | [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) | Bir alanın arandığı bağlantılı alanın kenarları. |
|
|  | autoScale | boolean | Bağlantılı alan boyutu tarafından searchArea ölçeklendirilip ölçeklendirilmediğini gösteren değer.\\ |
|
|  | useUpperCaseName | boolean | Bir  name  değerinin UPPER CASE'e dönüştürülüp dönüştürülmediğini gösteren değer. |
|

### getLinkedFieldName() {#getLinkedFieldName--}
```
public String getLinkedFieldName()
```


Bağlantılı alan adını alır.


**Returns:**
java.lang.String - Bağlantılı alan adını temsil eden büyük harfli bir dize değeri.

### getSearchArea() {#getSearchArea--}
```
public Size getSearchArea()
```


Bir alanın arandığı bölgenin boyutunu alır.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the area where a field is searched.

### isAutoScale() {#isAutoScale--}
```
public Boolean isAutoScale()
```


Bağlantılı alan boyutu tarafından  SearchArea  ölçeklendirilip ölçeklendirilmediğini gösteren değeri alır.


**Returns:**
java.lang.Boolean - {code true} eğer  SearchArea  bağlantılı alan boyutu tarafından ölçeklendirilmişse; aksi takdirde  false .

### getEdges() {#getEdges--}
```
public TemplateLinkedPositionEdges getEdges()
```


Bir alanın arandığı bağlantılı alanın kenarlarını alır.


**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that represents the edges of the linked field where a field is searched.

### scale(double factor) {#scale-double-}
```
public TemplatePosition scale(double factor)
```


Mevcut konumun bir kopyasını, tüm koordinatları verilen faktörle ölçeklendirilmiş şekilde oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| faktör | double |  |

**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition)
