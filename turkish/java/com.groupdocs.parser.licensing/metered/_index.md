---
title: "Metered"
second_title: "GroupDocs.Parser for Java API Referansı"
description: "Ölçümlü anahtarı ayarlamak için yöntemler sağlar."
type: docs
weight: 11
url: /tr/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Ölçümlü anahtarı ayarlamak için yöntemler sağlar.

Bu örnekte, ölçümlü genel ve özel anahtar ayarlamaya çalışılacaktır:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Metered()](#Metered--) | [Metered](../../com.groupdocs.parser.licensing/metered) sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Ölçümlü genel ve özel anahtarı ayarlar. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | İşlenen MB miktarını alır. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Harcanan kredi sayısını alır. |
|
### Metered() {#Metered--}
```
public Metered()
```


[Metered](../../com.groupdocs.parser.licensing/metered) sınıfının yeni bir örneğini başlatır.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Ölçümlü genel ve özel anahtarı ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | publicKey | java.lang.String | Bir genel anahtar. |
|
|  | privateKey | java.lang.String | Bir özel anahtar |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


İşlenen MB miktarını alır.


**Returns:**
java.math.BigDecimal - Tüketim miktarını temsil eden bir double değeri.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Harcanan kredi sayısını alır.


**Returns:**
java.math.BigDecimal - Tüketim kredisini temsil eden bir double değeri.

