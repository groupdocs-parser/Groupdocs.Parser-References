---
title: "Metered"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Proporciona métodos para establecer la clave metered."
type: docs
weight: 11
url: /es/java/com.groupdocs.parser.licensing/metered/
---
**Inheritance:**
java.lang.Object
```
public final class Metered
```

Proporciona métodos para establecer la clave metered.

En este ejemplo, se intentará establecer la clave pública y privada de metered:

````
 ```

Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
  
``` 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Metered()](#Metered--) | Inicializa una nueva instancia de la clase [Metered](../../com.groupdocs.parser.licensing/metered). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Establece la clave pública y privada de metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Obtiene la cantidad de MB procesados. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Obtiene el recuento de créditos consumidos. |
|
### Metered() {#Metered--}
```
public Metered()
```


Inicializa una nueva instancia de la clase [Metered](../../com.groupdocs.parser.licensing/metered).


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Establece la clave pública y privada de metered.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | publicKey | java.lang.String | Una clave pública. |
|
|  | privateKey | java.lang.String | Una clave privada |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static BigDecimal getConsumptionQuantity()
```


Obtiene la cantidad de MB procesados.


**Returns:**
java.math.BigDecimal - Un valor double que representa la cantidad de consumo.

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static BigDecimal getConsumptionCredit()
```


Obtiene el recuento de créditos consumidos.


**Returns:**
java.math.BigDecimal - Un valor double que representa el crédito de consumo.

