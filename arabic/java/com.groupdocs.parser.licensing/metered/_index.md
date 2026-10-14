---
title: "Metered"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر طرقًا لتعيين المفتاح Metered."
type: docs
weight: 11
url: /ar/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

يوفر طرقًا لتعيين المفتاح Metered.

في هذا المثال، سيتم محاولة تعيين المفتاح العام والخاص للعداد:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [Metered()](#Metered--) | ينشئ مثلاً جديداً للفئة [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | يضبط المفتاح العام والخاص للعداد. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | يسترجع مقدار الميجابايتات المعالجة. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | يسترجع عدد الاعتمادات المستهلكة. |
|
### Metered() {#Metered--}
```
public Metered()
```


ينشئ مثلاً جديداً للفئة [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


يضبط المفتاح العام والخاص للعداد.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | publicKey | java.lang.String | مفتاح عام. |
|
|  | privateKey | java.lang.String | مفتاح خاص |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


يسترجع مقدار الميجابايتات المعالجة.


**Returns:**
java.math.BigDecimal - قيمة مزدوجة تمثل كمية الاستهلاك.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


يسترجع عدد الاعتمادات المستهلكة.


**Returns:**
java.math.BigDecimal - قيمة مزدوجة تمثل ائتمان الاستهلاك.

