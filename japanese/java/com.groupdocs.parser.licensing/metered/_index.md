---
title: "Metered"
second_title: "GroupDocs.Parser for Java API リファレンス"
description: "従量課金キーを設定するメソッドを提供します。"
type: docs
weight: 11
url: /ja/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

従量課金キーを設定するメソッドを提供します。

この例では、metered の公開鍵と秘密鍵を設定しようとします：

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [Metered()](#Metered--) | [Metered](../../com.groupdocs.parser.licensing/metered) クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | metered の公開鍵と秘密鍵を設定します。 |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | 処理された MB の量を取得します。 |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | 消費されたクレジット数を取得します。 |
|
### Metered() {#Metered--}
```
public Metered()
```


[Metered](../../com.groupdocs.parser.licensing/metered) クラスの新しいインスタンスを初期化します。


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


metered の公開鍵と秘密鍵を設定します。


**Parameters:**
| パラメータ | 型 | 説明 |
| --- | --- | --- |
|  | publicKey | java.lang.String | 公開鍵。 |
|
|  | privateKey | java.lang.String | 秘密鍵 |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


処理された MB の量を取得します。


**Returns:**
java.math.BigDecimal - 消費量を表す double 値。

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


消費されたクレジット数を取得します。


**Returns:**
java.math.BigDecimal - 消費クレジットを表す double 値。

