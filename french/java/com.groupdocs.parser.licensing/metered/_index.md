---
title: "Metered"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit des méthodes pour définir la clé de facturation à la consommation."
type: docs
weight: 11
url: /fr/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Fournit des méthodes pour définir la clé de facturation à la consommation.

Dans cet exemple, une tentative sera faite pour définir la clé publique et privée métrée :

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Constructors

| Constructor | Description |
| --- | --- |
|  | [Metered()](#Metered--) | Initialise une nouvelle instance de la classe [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Définit la clé publique et privée métrée. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Récupère la quantité de Mo traités. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Récupère le nombre de crédits consommés. |
|
### Metered() {#Metered--}
```
public Metered()
```


Initialise une nouvelle instance de la classe [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Définit la clé publique et privée métrée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | publicKey | java.lang.String | Une clé publique. |
|
|  | privateKey | java.lang.String | Une clé privée |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Récupère la quantité de Mo traités.


**Returns:**
java.math.BigDecimal - Une valeur double qui représente la quantité de consommation.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Récupère le nombre de crédits consommés.


**Returns:**
java.math.BigDecimal - Une valeur double qui représente le crédit de consommation.

