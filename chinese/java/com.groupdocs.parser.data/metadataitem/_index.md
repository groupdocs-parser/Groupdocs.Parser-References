---
title: "MetadataItem"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示在容器项和元数据提取功能中使用的元数据项。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.parser.data/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

表示在容器项和元数据提取功能中使用的元数据项。

一个 [MetadataItem](../../com.groupdocs.parser.data/metadataitem) 类的实例用作 [Parser.getMetadata()](../../com.groupdocs.parser/parser#getMetadata--) 方法的返回值。
并作为 [ContainerItem.getMetadata()](../../com.groupdocs.parser.data/containeritem#getMetadata--) 集合中的一个项。请参阅那里的使用示例。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [MetadataItem(String name, String value)](#MetadataItem-java.lang.String-java.lang.String-) | 初始化一个新的 [MetadataItem](../../com.groupdocs.parser.data/metadataitem) 类实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getName()](#getName--) | 获取元数据项的名称。 |
|
|  | [getValue()](#getValue--) | 获取元数据项的值。 |
|
### MetadataItem(String name, String value) {#MetadataItem-java.lang.String-java.lang.String-}
```
public MetadataItem(String name, String value)
```


初始化一个新的 [MetadataItem](../../com.groupdocs.parser.data/metadataitem) 类实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 名称 | java.lang.String | 元数据项的名称。 |
|
|  | 值 | java.lang.String | 元数据项的值。 |
|

### getName() {#getName--}
```
public String getName()
```


获取元数据项的名称。


**Returns:**
java.lang.String - 表示元数据项名称的字符串值。

### getValue() {#getValue--}
```
public String getValue()
```


获取元数据项的值。


**Returns:**
java.lang.String - 表示元数据项值的字符串值。

