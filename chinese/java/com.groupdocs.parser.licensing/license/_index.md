---
title: "许可证"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示 GroupDocs.Parser 许可证。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.parser.licensing/license/
---
**Inheritance:**
java.lang.Object
```
public final class License
```

表示 GroupDocs.Parser 许可证。

本例演示了如何设置许可证。

````
 ```

// 初始化 License 类
License license = new License();
// 设置 .lic 文件的路径
license.setLicense("C:\\GroupDocs.Parser.for.Java.lic");
 
``` 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [License()](#License--) | 初始化 [License](../../com.groupdocs.parser.licensing/license) 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [setLicense(String filePath)](#setLicense-java.lang.String-) | 为组件授权。 |
|
|  | [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | 为组件授权。 |
|
### License() {#License--}
```
public License()
```


初始化 [License](../../com.groupdocs.parser.licensing/license) 类的新实例。


### setLicense(String filePath) {#setLicense-java.lang.String-}
```
public final void setLicense(String filePath)
```


为组件授权。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filePath | java.lang.String | 许可证文件的绝对路径。 |
|

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


为组件授权。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 许可证流。 |
|

