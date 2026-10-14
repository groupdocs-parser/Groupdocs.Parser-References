---
title: "Metered"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce metodi per impostare la chiave a consumo."
type: docs
weight: 11
url: /it/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Fornisce metodi per impostare la chiave a consumo.

In questo esempio, verrà tentato di impostare la chiave pubblica e privata di metered:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Metered()](#Metered--) | Inizializza una nuova istanza della classe [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Imposta la chiave pubblica e privata di metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Recupera la quantità di MB elaborati. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Recupera il conteggio dei crediti consumati. |
|
### Metered() {#Metered--}
```
public Metered()
```


Inizializza una nuova istanza della classe [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Imposta la chiave pubblica e privata di metered.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | publicKey | java.lang.String | Una chiave pubblica. |
|
|  | privateKey | java.lang.String | Una chiave privata |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Recupera la quantità di MB elaborati.


**Returns:**
java.math.BigDecimal - Un valore double che rappresenta la quantità di consumo.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Recupera il conteggio dei crediti consumati.


**Returns:**
java.math.BigDecimal - Un valore double che rappresenta il credito di consumo.

