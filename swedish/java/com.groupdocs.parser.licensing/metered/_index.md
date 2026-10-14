---
title: "Metered"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller metoder för att ställa in mätad nyckel."
type: docs
weight: 11
url: /sv/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Tillhandahåller metoder för att ställa in mätad nyckel.

I det här exemplet kommer ett försök att göras för att ställa in metered offentliga och privata nycklar:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey(\"PublicKey\", \"PrivateKey\");
  
``` 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Metered()](#Metered--) | Initierar en ny instans av klassen [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Ställer in metered offentliga och privata nycklar. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Hämtar mängden MB som bearbetats. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Hämtar antalet krediter som förbrukats. |
|
### Metered() {#Metered--}
```
public Metered()
```


Initierar en ny instans av klassen [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Ställer in metered offentliga och privata nycklar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | publicKey | java.lang.String | En offentlig nyckel. |
|
|  | privateKey | java.lang.String | En privat nyckel |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Hämtar mängden MB som bearbetats.


**Returns:**
java.math.BigDecimal - Ett dubbelvärde som representerar konsumtionsmängden.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Hämtar antalet krediter som förbrukats.


**Returns:**
java.math.BigDecimal - Ett dubbelvärde som representerar konsumtionskrediten.

