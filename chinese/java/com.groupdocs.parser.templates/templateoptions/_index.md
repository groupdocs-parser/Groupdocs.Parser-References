---
title: "TemplateOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于模板功能解析的选项。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.parser.templates/templateoptions/
---
**Inheritance:**
java.lang.Object
```
public class TemplateOptions
```

提供用于模板功能解析的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TemplateOptions(double rectangleTolerance)](#TemplateOptions-double-) | 初始化 [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangleTolerance()](#getRectangleTolerance--) | 获取在矩形区域捕获时被忽略的边框大小。 |
|
### TemplateOptions(double rectangleTolerance) {#TemplateOptions-double-}
```
public TemplateOptions(double rectangleTolerance)
```


初始化 [TemplateOptions](../../com.groupdocs.parser.templates/templateoptions) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangleTolerance | double | 在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。 |
|

### getRectangleTolerance() {#getRectangleTolerance--}
```
public double getRectangleTolerance()
```


获取在矩形区域捕获时被忽略的边框大小。它以文本项高度的比例来衡量。


**Returns:**
double - 从 0（无边框）到 1（忽略整个元素）的 double 值。

