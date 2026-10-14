---
title: "Metered"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt Methoden zum Setzen des Metered‑Schlüssels bereit."
type: docs
weight: 11
url: /de/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Stellt Methoden zum Setzen des Metered‑Schlüssels bereit.

In diesem Beispiel wird versucht, den metered öffentlichen und privaten Schlüssel zu setzen:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Metered()](#Metered--) | Initialisiert eine neue Instanz der [Metered](../../com.groupdocs.parser.licensing/metered) Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Setzt den metered öffentlichen und privaten Schlüssel. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Ruft die Menge der verarbeiteten MBs ab. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Ruft die Anzahl der verbrauchten Credits ab. |
|
### Metered() {#Metered--}
```
public Metered()
```


Initialisiert eine neue Instanz der [Metered](../../com.groupdocs.parser.licensing/metered) Klasse.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Setzt den metered öffentlichen und privaten Schlüssel.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | publicKey | java.lang.String | Ein öffentlicher Schlüssel. |
|
|  | privateKey | java.lang.String | Ein privater Schlüssel |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Ruft die Menge der verarbeiteten MBs ab.


**Returns:**
java.math.BigDecimal - Ein double-Wert, der die Verbrauchsmenge darstellt.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Ruft die Anzahl der verbrauchten Credits ab.


**Returns:**
java.math.BigDecimal - Ein double-Wert, der das Verbrauchsguthaben darstellt.

