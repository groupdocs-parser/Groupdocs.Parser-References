---
title: Metered
second_title: GroupDocs.Parser for Java API Reference
description: Provides methods to set metered key.
type: docs
weight: 11
url: /java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Provides methods to set metered key.

In this example, an attempt will be made to set metered public and private key:

```

 	Metered metered = new Metered();
 	metered.setMeteredKey("PublicKey", "PrivateKey");
  
```
## Constructors

| Constructor | Description |
| --- | --- |
| [Metered()](#Metered--) | Initializes a new instance of the [Metered](../../com.groupdocs.parser.licensing/metered) class. |
## Methods

| Method | Description |
| --- | --- |
| [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Sets metered public and private key. |
| [getConsumptionQuantity()](#getConsumptionQuantity--) | Retrieves amount of MBs processed. |
| [getConsumptionCredit()](#getConsumptionCredit--) | Retrieves count of credits consumed. |
### Metered() {#Metered--}
```
public Metered()
```


Initializes a new instance of the [Metered](../../com.groupdocs.parser.licensing/metered) class.

### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Sets metered public and private key.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | java.lang.String | A public key. |
| privateKey | java.lang.String | A private key |

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Retrieves amount of MBs processed.

**Returns:**
java.math.BigDecimal - A double value that represents the consumption quantity.
### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Retrieves count of credits consumed.

**Returns:**
java.math.BigDecimal - A double value that represents the consumption credit.
