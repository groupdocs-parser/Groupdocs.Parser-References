---
title: "页面条码区域"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示用于在基于模板的解析功能中表示条码值的页面条码区域。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.parser.data/pagebarcodearea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageBarcodeArea extends PageArea
```

表示用于在基于模板的解析功能中表示条码值的页面条码区域。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)](#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | 初始化 [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getValue()](#getValue--) | 获取条码值。 |
|
|  | [getCodeTypeName()](#getCodeTypeName--) | 获取条码类型的名称。 |
|
|  | [getConfidence()](#getConfidence--) | 获取已解析条形码的置信度水平。 |
|
|  | [getAngle()](#getAngle--) | 获取条形码的角度。 |
|
### PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle) {#PageBarcodeArea-java.lang.String-java.lang.String-int-double-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageBarcodeArea(String value, String codeTypeName, int confidence, double angle, Page page, Rectangle rectangle)
```


初始化 [PageBarcodeArea](../../com.groupdocs.parser.data/pagebarcodearea) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 条形码的值。 |
|
|  | codeTypeName | java.lang.String | 条形码的类型名称。 |
|
|  | confidence | int | 已解析条形码的置信度水平。 |
|
|  | angle | double | 条形码的角度。 |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | 包含条形码区域的页面。 |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | 包含条形码区域的矩形区域。 |
|

### getValue() {#getValue--}
```
public String getValue()
```


获取条码值。


**Returns:**
java.lang.String - 表示条形码页面区域值的字符串。

### getCodeTypeName() {#getCodeTypeName--}
```
public String getCodeTypeName()
```


获取条码类型的名称。


**Returns:**
java.lang.String - 表示条形码类型名称的字符串。

### getConfidence() {#getConfidence--}
```
public int getConfidence()
```


获取已解析条形码的置信度水平。


**Returns:**
int - 表示已解析条形码置信度的整数值（0-100）。

### getAngle() {#getAngle--}
```
public double getAngle()
```


获取条形码的角度。


**Returns:**
double - 表示条形码角度的数值（0-360）。

