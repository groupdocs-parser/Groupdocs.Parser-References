---
title: "ExternalResourceLoadingArgs"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于 方法的数据。"
type: docs
weight: 17
url: /zh/java/com.groupdocs.parser.options/externalresourceloadingargs/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceLoadingArgs
```

提供用于 [ExternalResourceHandler.onLoading(ExternalResourceLoadingArgs)](../../com.groupdocs.parser.options/externalresourcehandler#onLoading-ExternalResourceLoadingArgs-) 方法的数据。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [ExternalResourceLoadingArgs(String uri)](#ExternalResourceLoadingArgs-java.lang.String-) | 使用矩形区域初始化 [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getUri()](#getUri--) | 获取外部资源的 URI。 |
|
|  | [setUri(String uri)](#setUri-java.lang.String-) | 获取外部资源的 URI。 |
|
|  | [isSkipped()](#isSkipped--) | 获取指示是否必须跳过外部资源加载的值。 |
|
|  | [setSkipped(boolean skipped)](#setSkipped-boolean-) | 设置指示是否必须跳过外部资源加载的值。 |
|
|  | [getData()](#getData--) | 获取用户数据。 |
|
|  | [setData(byte[] data)](#setData-byte---) | 设置用户数据。 |
|
### ExternalResourceLoadingArgs(String uri) {#ExternalResourceLoadingArgs-java.lang.String-}
```
public ExternalResourceLoadingArgs(String uri)
```


使用矩形区域初始化 [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | uri | java.lang.String | 外部资源的 URI。 |
|

### getUri() {#getUri--}
```
public String getUri()
```


获取外部资源的 URI。


**Returns:**
java.lang.String - 表示外部资源 URI 的字符串值。

### setUri(String uri) {#setUri-java.lang.String-}
```
public void setUri(String uri)
```


获取外部资源的 URI。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | uri | java.lang.String | 表示外部资源新 URI 的字符串值。 |
|

### isSkipped() {#isSkipped--}
```
public boolean isSkipped()
```


获取指示是否必须跳过外部资源加载的值。


**Returns:**
boolean - 如果必须跳过外部资源加载则为 true；否则为 false。

### setSkipped(boolean skipped) {#setSkipped-boolean-}
```
public void setSkipped(boolean skipped)
```


设置指示是否必须跳过外部资源加载的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | skipped | boolean | 如果必须跳过外部资源加载则为 true；否则为 false。 |
|

### getData() {#getData--}
```
public byte[] getData()
```


获取用户数据。


**Returns:**
byte[] - 包含外部资源用户内容的字节数组。如果未设置则为 null。

### setData(byte[] data) {#setData-byte---}
```
public void setData(byte[] data)
```


设置用户数据。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | data | byte[] | 包含外部资源用户内容的字节数组。如果未设置则为 null。 |
|

