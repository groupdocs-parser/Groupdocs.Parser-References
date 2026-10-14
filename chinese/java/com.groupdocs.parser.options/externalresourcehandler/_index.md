---
title: "ExternalResourceHandler"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于外部资源加载的处理程序。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.parser.options/externalresourcehandler/
---
**Inheritance:**
java.lang.Object
```
public class ExternalResourceHandler
```

提供用于外部资源加载的处理程序。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExternalResourceHandler()](#ExternalResourceHandler--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [onLoading(ExternalResourceLoadingArgs args)](#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-) | 在任何外部资源加载之前调用。 |
|
### ExternalResourceHandler() {#ExternalResourceHandler--}
```
public ExternalResourceHandler()
```


### onLoading(ExternalResourceLoadingArgs args) {#onLoading-com.groupdocs.parser.options.ExternalResourceLoadingArgs-}
```
public void onLoading(ExternalResourceLoadingArgs args)
```


在任何外部资源加载之前调用。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | args | [ExternalResourceLoadingArgs](../../com.groupdocs.parser.options/externalresourceloadingargs) | 用于控制外部资源加载的数据。 |
|

