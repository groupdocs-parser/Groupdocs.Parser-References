---
title: "Metered"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "사용량 기반 키를 설정하는 메서드를 제공합니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

사용량 기반 키를 설정하는 메서드를 제공합니다.

이 예제에서는 메터드 public 및 private 키를 설정하려고 시도합니다:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Metered()](#Metered--) | 새 인스턴스를 초기화합니다 [Metered](../../com.groupdocs.parser.licensing/metered) 클래스. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | metered public 및 private 키를 설정합니다. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | 처리된 MB 양을 검색합니다. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | 소모된 크레딧 수를 검색합니다. |
|
### Metered() {#Metered--}
```
public Metered()
```


새 인스턴스를 초기화합니다 [Metered](../../com.groupdocs.parser.licensing/metered) 클래스.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


metered public 및 private 키를 설정합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | publicKey | java.lang.String | 공개 키입니다. |
|
|  | privateKey | java.lang.String | 개인 키입니다 |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


처리된 MB 양을 검색합니다.


**Returns:**
java.math.BigDecimal - 소비량을 나타내는 double 값.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


소모된 크레딧 수를 검색합니다.


**Returns:**
java.math.BigDecimal - 소비 크레딧을 나타내는 double 값.

