---
title: "Metered"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Предоставляет методы для установки почасового ключа."
type: docs
weight: 11
url: /ru/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Предоставляет методы для установки почасового ключа.

В этом примере будет предпринята попытка установить metered публичный и приватный ключ:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Metered()](#Metered--) | Инициализирует новый экземпляр класса [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Устанавливает metered публичный и приватный ключ. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Получает количество обработанных МБ. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Получает количество использованных кредитов. |
|
### Metered() {#Metered--}
```
public Metered()
```


Инициализирует новый экземпляр класса [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Устанавливает metered публичный и приватный ключ.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | publicKey | java.lang.String | Публичный ключ. |
|
|  | privateKey | java.lang.String | Приватный ключ |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Получает количество обработанных МБ.


**Returns:**
java.math.BigDecimal - Значение типа double, представляющее количество потребления.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Получает количество использованных кредитов.


**Returns:**
java.math.BigDecimal - Значение типа double, представляющее потребляемый кредит.

