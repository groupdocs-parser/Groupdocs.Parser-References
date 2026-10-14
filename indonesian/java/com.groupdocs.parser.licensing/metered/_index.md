---
title: "Metered"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan metode untuk mengatur kunci metered."
type: docs
weight: 11
url: /id/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Menyediakan metode untuk mengatur kunci metered.

Dalam contoh ini, akan dilakukan percobaan untuk mengatur kunci publik dan privat metered:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Metered()](#Metered--) | Menginisialisasi sebuah instance baru dari kelas [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Mengatur kunci publik dan privat metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Mengambil jumlah MB yang diproses. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Mengambil jumlah kredit yang dikonsumsi. |
|
### Metered() {#Metered--}
```
public Metered()
```


Menginisialisasi sebuah instance baru dari kelas [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Mengatur kunci publik dan privat metered.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | publicKey | java.lang.String | Sebuah kunci publik. |
|
|  | privateKey | java.lang.String | Sebuah kunci privat |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Mengambil jumlah MB yang diproses.


**Returns:**
java.math.BigDecimal - Nilai double yang mewakili kuantitas konsumsi.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Mengambil jumlah kredit yang dikonsumsi.


**Returns:**
java.math.BigDecimal - Nilai double yang mewakili kredit konsumsi.

