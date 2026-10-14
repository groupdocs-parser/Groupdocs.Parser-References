---
title: "Metered"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供设置计量密钥的方法。"
type: docs
weight: 11
url: /zh/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

提供设置计量密钥的方法。

在本例中，将尝试设置 metered 公钥和私钥：

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Metered()](#Metered--) | 初始化一个新的 [Metered](../../com.groupdocs.parser.licensing/metered) 类的实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | 设置 metered 公钥和私钥。 |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | 检索已处理的 MB 数量。 |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | 检索已消耗的积分数量。 |
|
### Metered() {#Metered--}
```
public Metered()
```


初始化一个新的 [Metered](../../com.groupdocs.parser.licensing/metered) 类的实例。


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


设置 metered 公钥和私钥。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | publicKey | java.lang.String | 公钥。 |
|
|  | privateKey | java.lang.String | 私钥 |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


检索已处理的 MB 数量。


**Returns:**
java.math.BigDecimal - 表示消耗数量的 double 值。

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


检索已消耗的积分数量。


**Returns:**
java.math.BigDecimal - 表示消耗积分的 double 值。

