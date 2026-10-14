---
title: "TemplateLinkedPositionEdges"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Metin alanının arandığı bağlantılı alanın kenarlarını sağlar."
type: docs
weight: 16
url: /tr/java/com.groupdocs.parser.templates/templatelinkedpositionedges/
---
**Inheritance:**
java.lang.Object
```
public class TemplateLinkedPositionEdges
```

Bağlı alanın metin alanının arandığı kenarlarını sağlar. [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) sınıfı, [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition) sınıfında kullanılır.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)](#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-) | Yeni bir [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) sınıf örneği başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isEmpty()](#isEmpty--) | Örneğin boş olup olmadığını gösteren değeri alır. |
|
|  | [isLeft()](#isLeft--) | Bağlı alandan sola doğru bir alanın aranıp aranmadığını gösteren değeri alır. |
|
|  | [isTop()](#isTop--) | Bağlı alandan yukarı doğru bir alanın aranıp aranmadığını gösteren değeri alır. |
|
|  | [isRight()](#isRight--) | Bağlı alandan sağa doğru bir alanın aranıp aranmadığını gösteren değeri alır. |
|
|  | [isBottom()](#isBottom--) | Bağlı alandan aşağı doğru bir alanın aranıp aranmadığını gösteren değeri alır. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Kenarların dize temsilini sınıf eşdeğerine dönüştürür. |
|
| [toString()](#toString--) |  |
### TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom) {#TemplateLinkedPositionEdges-boolean-boolean-boolean-boolean-}
```
public TemplateLinkedPositionEdges(boolean left, boolean top, boolean right, boolean bottom)
```


Yeni bir [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) sınıf örneği başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | sol | boolean | Bağlı alandan sola doğru bir alanın aranıp aranmadığını gösteren değer. |
|
|  | üst | boolean | Bağlı alandan yukarı doğru bir alanın aranıp aranmadığını gösteren değer. |
|
|  | sağ | boolean | Bağlı alandan sağa doğru bir alanın aranıp aranmadığını gösteren değer. |
|
|  | alt | boolean | Bağlı alandan aşağı doğru bir alanın aranıp aranmadığını gösteren değer. |
|

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Örneğin boş olup olmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer örnek boşsa (tüm alanlar false); aksi takdirde,  false .

### isLeft() {#isLeft--}
```
public boolean isLeft()
```


Bağlı alandan sola doğru bir alanın aranıp aranmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer bir alan bağlı alandan sola doğru aranıyorsa; aksi takdirde,  false .

### isTop() {#isTop--}
```
public boolean isTop()
```


Bağlı alandan yukarı doğru bir alanın aranıp aranmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer bir alan bağlı alandan yukarı doğru aranıyorsa; aksi takdirde,  false .

### isRight() {#isRight--}
```
public boolean isRight()
```


Bağlı alandan sağa doğru bir alanın aranıp aranmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer bir alan bağlı alandan sağa doğru aranıyorsa; aksi takdirde,  false .

### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Bağlı alandan aşağı doğru bir alanın aranıp aranmadığını gösteren değeri alır.


**Returns:**
boolean -  true  eğer bir alan bağlı alandan aşağı doğru aranıyorsa; aksi takdirde,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static TemplateLinkedPositionEdges parse(String s)
```


Kenarların dize temsilini sınıf eşdeğerine dönüştürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | s | java.lang.String | Dönüştürülecek kenarları içeren bir dize. |
|

**Returns:**
[TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) - An instance of [TemplateLinkedPositionEdges](../../com.groupdocs.parser.templates/templatelinkedpositionedges) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
