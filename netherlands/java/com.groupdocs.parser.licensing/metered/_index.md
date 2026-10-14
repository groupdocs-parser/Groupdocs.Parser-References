---
title: "Metered"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt methoden om een metered-sleutel in te stellen."
type: docs
weight: 11
url: /nl/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Biedt methoden om een metered-sleutel in te stellen.

In dit voorbeeld wordt geprobeerd om de metered openbare en privésleutel in te stellen:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Metered()](#Metered--) | Initialiseert een nieuw exemplaar van de [Metered](../../com.groupdocs.parser.licensing/metered) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Stelt de metered openbare en privésleutel in. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Haalt de hoeveelheid verwerkte MB's op. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Haalt het aantal verbruikte credits op. |
|
### Metered() {#Metered--}
```
public Metered()
```


Initialiseert een nieuw exemplaar van de [Metered](../../com.groupdocs.parser.licensing/metered) klasse.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Stelt de metered openbare en privésleutel in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | publicKey | java.lang.String | Een openbare sleutel. |
|
|  | privateKey | java.lang.String | Een privésleutel |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Haalt de hoeveelheid verwerkte MB's op.


**Returns:**
java.math.BigDecimal - Een double-waarde die de consumptiehoeveelheid vertegenwoordigt.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Haalt het aantal verbruikte credits op.


**Returns:**
java.math.BigDecimal - Een double-waarde die het consumptie‑credit vertegenwoordigt.

